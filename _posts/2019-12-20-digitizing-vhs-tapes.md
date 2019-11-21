---
title: My Eight Year Quest to Digitize 45 Video Tapes
---

I've carried this box of video tapes around for the last eight years. They've moved with me through four different apartments and one house. They're VHS tapes from the home videos my family made throughout my childhood. I refused to throw them away until I digitized them. And not just digitized them, but digitized them so well.

I finally completed the project last year. Even though it's a web server, I don't have to pay for web hosting. My only cost is 

## That doesn't sound so hard

If you're wondering why it took so long, I don't blame you. I thought it would be an easy project too. These are family artifacts, and I'm not willing to throw away the tapes until I'm confident that I've captured all of the data accurately. But once you start doing it, you realize that capturing the data accurately isn't as simple as it seems. There's metadata on the tapes. Some of the tapes have labels that give clues about the dates. There's ordering to the clips that's also important for establishing dates. If someone says the date in clip A then the date in clip C, you know that clip B must be between dates A and C. But if you naively approach it the way I originally did, just saving the clip as "Michael plays with water balloons.mp4" then you lose that metadata.

## The result

There are . It's 513 separate clips. Each clip shows the date, which tape it came from.

## Accepting this quest

Back around 2010, my mom told me that she had digitized all of our old home videos. She bought some device that converted VHS to DVD, so she ran all of the old home videos through it. The problem was that there was only one copy, so to watch any of it, you still had to 

And watching it, I realized that there were clips missing. I asked for the full original set of VHS tapes. My dad still had an old VCR. I thought it would be as simple as buying some kind of cable to connect the VCR to my computer and I'd be done.

## Part 1: Digitizing

Second try with video capture software
Try three with different combinations of VCRs and capture devices
Try four with digitization company, EverPresent
  * A long rant on EverPresent
    * Gave me a hard drive when I specifically said I didn't want one
    * Charged a different price than what I was quoted
    * Published easily discoverable videos
    * Gotta admit, quality was great

## Part 2: Editing

The problem with home videos is that 90% of the footage is boring, 8% is entertaining, and 2% is amazing. That means that after you digitize the tapes, there's still lots of work to do.

* First try of editing everything in Adobe Premiere Elements
  * Lose data, lots of starting and stopping.
* python scene detect
* I remembered that I'm a programmer
  * process-home-videos

## Part 3: Sharing

People also don't want to read through a bunch of video files.

* Put the zips on Google Cloud Storage
* Failure of ClipBucket
* MediaGoblin
  * Realized I can transcode ahead of time
  * Faster if the client can hit GCS directly
  * Realized I don't actually want to give MediaGoblin access to Google Cloud Storage
* In retrospect, MediaGoblin was also a bad choice
  * No longer actively maintained
  * Hard to contribute to their repo
* If I were to do this again, I'd do everything with a static site generator
  * I don't need a web server for anything except for user authentication
  * I'd just need something that can consume my YAML file, then generate pages for each video

## The final workflow


## Tips for anyone about to try this

* Capture as much metadata as possible
* It will be *really* difficult and expensive for you to achieve the same quality capture as a company that does dedicated video digitization (but steer clear of XX company)
* Capture as much of the data in an application-agnostic format
  * Clip descriptions, time codes, dates, etc.
  * If you keep it in an application specific format (or worse, throw it away), it's difficult for you to reproduce the work if you decide on a different solution.

## Source code

| Repository  | Description |
|-------------|-------------|
| [MediaGoblin](https://github.com/mtlynch/mediagoblin) | Mirror of the MediaGoblin core repo + Circle CI configuration. [mtlynch-custom](https://github.com/mtlynch/mediagoblin/tree/mtlynch-custom) has custom fixes for my instance (replaces their old video player and trims some parts of their UI that I don't need). |
| [mediagoblin-docker](https://github.com/mtlynch/mediagoblin-docker) | Docker image for MediaGoblin. Depends on the MediaGoblin repo. |
| [process-home-videos](https://github.com/mtlynch/process-home-videos) | Python scripts for chopping up raw video files into clips and then publishing those clips to MediaGoblin. |

TODO: How do people annotate with frame numbers?

---

*Cover art by [Loraine Yow](https://www.linkedin.com/in/lolo-ology/).*