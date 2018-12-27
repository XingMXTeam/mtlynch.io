---
title: What I Learned About Upwork from a  Bumbling Scammer
layout: single
author_profile: true
read_time: true
comments: true
share: true
related: true
sidebar:
  nav: main
classes: wide
tags:
- upwork
- isitketo
- outsourcing
excerpt: How I solved the mystery of the worst scammer I've ever encountered.
header:
  teaser: images/upwork-scammer/profile-stitching.png
  og_image: images/upwork-scammer/profile-stitching.png
---

For years, I've hired freelancers through a site called Upwork. The site attracts many different professionals, so I've used it to find everything from [cartoonists](https://mtlynch.io/how-to-hire-a-cartoonist/) to software developers to [copy editors](https://mtlynch.io/editor/). Some were great, some were disastrous, but none of them had ever tried to scam me outright.

That is, until I met Lizzie.

{% include image.html file="lizzie-r-profile.png" alt="Screenshot of Lizzie R's Upwork profile page" max_width="450px" img_link="true" fig_caption="Lizzie's freelancer profile on Upwork" %}

I needed writers for a [keto diet website](https://isitketo.org) I'm building. As a native English speaker living in the US, Lizzie seemed like a potential match.  [Her profile](https://www.upwork.com/o/profiles/users/_~019b8bbe4e49ebe61c/) was free of loud grammatical errors, an alarmingly rare quality among writers for hire. And best of all, she only charged $10/hr.

Okay, I know what you're thinking: for $10/hr, she's *obviously* a scammer. Or a terrible writer. Most writers on Upwork bill $30-60/hr, so why would anyone accept such a low rate?

But that's part of the adventure of Upwork. Some of the best people I've worked with advertised suspiciously cheap rates because they wanted to build a good rating history. Lizzie had only worked a few jobs, but she had perfect reviews on all of them.

If she turned out to be talented, I'd have a great writer at a phenomenal price. If she delivered something terrible, I'd at least get to see what $10/hr writing looked like.

# Exchanging $50 for a blank document

Upon receiving my job offer, Lizzie readily accepted. I assigned her three reports and provided [instructions](https://docs.google.com/document/d/1Uy19xtf_PFW0LJ2Zj6cSkH2dhHED8PCjHCtup1_IQ_4/edit?usp=sharing) on how to write them.

I set a limit of five hours and told her that if she wasn't done at the 4.5-hour mark, she should spend the last 30 minutes putting all of her progress into our shared Google Doc.

The next day, Upwork reported that Lizzie billed me the full five hours, but the Google Doc was empty. She hadn't sent me any messages, either.

# Intrusive surveillance to the rescue

Checking Lizzie's timesheet, I realized she had logged her hours using Work Diary, Upwork's official spyware tool. It captures images of the freelancer's screen, records their keystrokes, and sends all of the information to both Upwork and the client.

Work Diary creeps me out. I never require freelancers to run it, but Lizzie chose to run it instead of simply invoicing me for her hours. This meant that I didn't have any results, but I did have screenshots showing how she spent the five hours she billed to me.

{% include image.html file="workdiary-dashboard.png" alt="Screenshot of Work Diary dashboard" max_width="800px" class="img-border" img_link="true" fig_caption="Overview of Lizzie's activities in Work Diary" %}

In early screenshots, she was writing a document about mantras in Hinduism. It definitely had nothing to do with my project, but she was charging me for it.

{% assign fig_caption = 'Lizzie bills me for time writing an article on mantras for another client' %}

{% include image.html file="workdiary-2.jpg" alt="Screenshot of Lizzie R's WorkDiary history" max_width="800px" img_link="true" fig_caption=fig_caption %}

Later, she switched gears and started writing an article about tarot cards. Unless there's a new trend in the keto world that integrates tarot readings into food selection, this didn't seem like it related to my project either.

{% include image.html file="workdiary-4.jpg" alt="Screenshot of Lizzie R's WorkDiary history" max_width="800px" img_link="true" fig_caption="Lizzie bills me for another client's article about tarot cards" %}

# What's going on here?

Then, things got a bit more interesting. A screenshot showed Lizzie using Upwork's messaging interface to talk to her other clients:

{% include image.html file="workdiary-5.jpg" alt="Screenshot of Lizzie R's WorkDiary history" max_width="800px" img_link="true" fig_caption="A screenshot showing Lizzie messaging her other clients" %}

It  confused me at first because it showed two people talking, but neither of them was Lizzie. Oh! She was logged in as a different Upwork user under the name, "Abi Hensley."

A quick search on Upwork turned up [Abi's profile](https://www.upwork.com/o/profiles/users/_~012951f3927669080e). Sure enough, it had the exact same text and hourly rate as Lizzie:

{% include image.html file="abi-h-profile.png" alt="Screenshot of Abi H's Upwork profile" max_width="715px" img_link="true" fig_caption="Upwork profile for &quot;Abi H.&quot; with identical text to &quot;Lizzie R.&quot;" %}

That explained why she had four different web browsers pinned to her taskbar. She probably used a separate browser for each Upwork identity.

{% include image.html file="many-browsers.jpg" alt="Screenshot of Lizzie's desktop showing Firefox, Chrome, IE, and Opera" max_width="800px" class="img-border" img_link="true" fig_caption="Screenshot of Lizzie's desktop showing four different web browsers installed" %}

# Who is Grace?

One of the screenshots showed Lizzie's Documents folder:

{% include image.html file="workdiary-6.jpg" alt="Screenshot of Lizzi's documents folder" max_width="800px" class="img-border" img_link="true" fig_caption="Work Diary screenshot shows Lizzie's Documents folder" %}

It revealed several files with the name "Grace" in the title:

* "Grace Application Letter"
* "Grace CV"
* "Grace Intenship [*sic*] letter"

Finally, there was a PDF whose filename was "Grace" followed by what looked like a last name. The full name was unique enough that Google had only a single matching result: a Facebook profile of a schoolteacher in Kenya:

{% include image.html file="grace-facebook.png" alt="Screenshot of Lizzie R's WorkDiary history" max_width="504px" img_link="true" fig_caption="Lizzie's true identity, potentially" %}

# It's 9 PM. Do you know where you are?

There was another subtle clue buried in the screenshots: the time zone.

Upwork captured this image at 6:15 PM Greenwich Mean Time, but the freelancer's clock showed 9:17 PM.

{% include image.html file="time-comparison.jpg" alt="Screenshot of Lizzie's desktop" max_width="715px" img_link="true" fig_caption="Lizzie's clock is three hours ahead of Greenwich Mean Time" %}

What time zone could that be? Sure enough, it was the time zone for Nairobi, Kenya:

{% include image.html file="utc-to-nairobi.png" alt="6:15 PM UTC matching 9:15 PM in Nairobi, Kenya" max_width="758px" img_link="true" %}

Not to sound like a [birther](https://en.wikipedia.org/wiki/Barack_Obama_citizenship_conspiracy_theories), but between the Kenyan name and the Kenyan time zone, it seemed like "Lizzie" might, in fact, be Kenyan.

# What about that profile?

I took another look at the Upwork profile that led me to hire Lizzie in the first place. A few Google searches showed that Lizzie had plagiarized the whole thing &mdash; it was a mashup of a [LinkedIn profile](https://www.linkedin.com/in/laraflanagan/) and another [profile right from Upwork](https://www.upwork.com/o/profiles/users/_~017434da88fc78860a/).

{% include image.html file="profile-stitching.png" alt="Sources from which Lizzie stole her profile" max_width="800px" class="img-border" img_link="true" fig_caption="Lizzie created her profile by stitching together two others" %}

# Is this a trick?

The scam seemed so clumsy and obvious that I feared it was step one of a more elaborate con. Why upload screenshots proving she didn't do the work when she could have just sent me a regular invoice for $50? And then why bill me and withhold the reports? Naturally, that would prompt me to check the screenshot history.

In movies, the con-man always lets their victim *think* that they've uncovered the scam, but allowing the victim to expose the dummy fraud is all part of the *actual* fraud. Then, just as they believe they've gained the upper hand, the victim falls face-first into the real scam. Was there another layer of deceit here?

{% assign fig_caption = '"' | append: "I've locked Danny Ocean in a room next to my vault and paid his friend to guard him. Now he can *never* heist me!" | append: '"' | markdownify | remove: "<p>" | remove: "</p>" %}

{% include image.html file="oceans-eleven.jpg" alt="Still of George Clooney in Ocean's Eleven" max_width="800px" fig_caption=fig_caption img_link="true" %}

# How did Upwork miss this?

It struck me that Upwork forces freelancers to install invasive spyware, presumably to catch fraud, yet they ignored many huge indicators of fraud:

* Two freelancers used the same computer and IP while claiming to be in cities 2,000 miles apart.
* Two freelancers had exactly identical profiles.
* A freelancer plagiarized large sections of their profile from a more established user on the same site.
* Both freelancers claim to live in the US but have their clocks set to Nairobi time and likely have Kenyan IP addresses.

# Results, finally

As soon as I saw the screenshots, I closed the contract and reported the fraud to Upwork. Lizzie saw the contract end but was not privy to any of my comments about her.

The next day, Lizzie messaged me asking why I closed the contract. She made no mention of the unusual hours she billed me, but she attached a Word document containing my three completed reports.

This was her report on whether Coca-Cola is compatible with the keto diet:

>**Coca-Cola**
>
>***Short Description***
>
>Coca Cola is not keto because it contains high sugar content and not fats.
>
>***Detailed Description***
>
>According to the nutritional value of Coca Cola, it is not keto-friendly. It has 10.6 g of net carbs
for every serving **[Ed: Actual net carb count is 39 g]**. In addition, it has no fat and protein content. Perhaps, you can consider other
variations of Coca Cola like Coke Zero or the Diet Coke.

The grammar was decent, but it further confirmed Lizzie was not a native speaker. The loudest giveaway was the definite article before "Diet Coke." Americans never say, "I'd love a refreshing glass of **the** Diet Coke."

{% assign fig_caption = '"' | append: "Three glasses of the Diet Coke, please." | append: '"' | markdownify | remove: "<p>" | remove: "</p>" %}

{% include image.html file="three-glasses.jpg" alt="Still of Inglorious Basterds bar shootout scene" max_width="270px" img_link="true" fig_caption=fig_caption %}

# How Upwork handles fraud

Two days after I reported Lizzie's account as fraudulent, Upwork closed my support ticket with this note:

>Based on your report, I have examined the account and taken action as defined in our Terms of Service. In order to protect the confidentiality of all of our members’ accounts, I won’t be able to report back with the outcome of our investigation.

Won't be able to report the outcome? I expected them to close all of Lizzie's fake accounts, an outcome that should be highly visible to me.

It has now been three weeks since I reported Lizzie to Upwork. The profiles went private a few days after my report, but Upwork still shows them as active and accepting job offers:

* [Lizzie Ruprecht](https://www.upwork.com/o/profiles/users/_~019b8bbe4e49ebe61c/)
* [Abi Hensley](https://www.upwork.com/o/profiles/users/_~012951f3927669080e)

Upwork did refund my $50, which was nice.

# Why isn't my feedback showing up?

In my post-job feedback for Lizzie, I called out her profile as fraudulent. I was careful to avoid any accusations based on speculation. My review focused on objective facts: Lizzie billed me for unrelated work, and her Work Diary revealed that she was operating duplicate Upwork profiles.

Curiously, Upwork translated this into, "No feedback given":

{% include image.html file="lizzie-feedback.jpg" alt="Upwork shows I left no feedback for Lizzie" max_width="697px" img_link="true" fig_caption="Upwork hides my comments about Lizzie's fraudulent account in her Upwork profile." %}

# Warning other clients

The day I discovered Lizzie's shenanigans, I contacted one of her other clients. He had hired Lizzie through her "Abi" profile to write sales copy. He responded that he was still awaiting work from her but followed up with me a few days later to say he terminated her contract as well.

Tellingly, Upwork never notified this client of the fraud even though they had "examined the account and taken action" while he still had an open contract with Lizzie/Abi.

# Upwork's cross-contamination problem

Upwork client lists are private, so I shouldn't be able to contact one of my freelancer's other clients. But Lizzie bled enough information into her screenshots that I found contact information for the other guy who hired her.

This brings up another interesting problem with Upwork's Work Diary feature: cross-contamination.

What if a freelancer applied to work for you and ended their cover letter with this note:

>By the way, I routinely run software that sends captures of my entire screen to undisclosed third-parties. Hope you're cool with that!

You'd probably reject this candidate immediately. But that's what every Upwork user says implicitly if they track their time with Work Diary.

As the client, there's nothing you can do to prevent this. Clients can either require their freelancers to use Work Diary or make it optional, but there's no option to forbid it. Even if you could, other clients might still require it.

If a freelancer you hired ever happens to check messages from you while billing for another client or leave open a window containing your work, Work Diary will leak your private information to several additional parties. These kinds of leaks are unavoidable with automatic, whole-screen captures.

# Final thoughts

This experience has shown me some of Upwork's warts. On the one hand, they missed many red flags that I expect them to catch and did little to prevent continued abuse. On the other hand, it does say something that this is the first time I've hired a fraudster in all my years on Upwork.

While I've never been in love with Upwork, alternative platforms like Fiverr or Freelancer.com have been even worse for me. I'll continue using Upwork, but this episode has given me another reason to be conservative about granting freelancers access to private data.

{% include ads.html title="isitketo_writers" %}