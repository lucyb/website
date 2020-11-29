---
layout: post
title:  "Mob programming remotely during a pandemic"
date:   2020-11-30 18:39:00 +0100
categories: post
excerpt_separator: <!-- more -->
---

> "Mob programming is a software development approach where the whole team works on the same thing, at the same time, in the same space, and at the same computer."
-- Woody Zuill

The team I'm in had been using mob programming as a technique for a while before COVID-19 caused us all to work remotely. We'd gather around a large TV screen, set up someone's laptop, find a few keyboards, share some cookies and start a timer. It was a highly collaborative and enjoyable way of working. Occasionally, someone would work from home and we'd set them up on a screen in the corner, and to be honest that didn't work so well. Then suddenly, we all had to work remote and things changed.

<!-- more -->

* [What is mob programming?](#what-is-mob-programming)
* [Dealing with change](#dealing-with-change)
    * [Working during a pandemic](#working-during-a-pandemic)
* [How does that work remotely?](#how-does-that-work-remotely)
    * [Getting started](#getting-started)
    * [Technology considerations](#technology-considerations)
* [References](#references)

# What is mob programming?

While pair programming has become fairly standard within the software development industry, mob programming is less common (for now at least). In mob programming a group of people will get together to work on the same piece of code at the same time. It's really a way of solving problems collaboratively. 

Typically, one person is nominated as a 'driver', a typist who is responsible for following the mob's ideas and writing it down as code. This driver role is rotated around the mob, swapping every few minutes or several times a day, depending on how the mob decides to work.

The mobs I've been in have typically been multi-disciplinary, with software engineers, platform engineers, architects, quality analysts, business analysts, designers, product owners, etc, being involved as needed. 

There are many benefits to this approach. For starters, everyone needed to solve the problem is in the room or can be easily. There's no waiting, no handovers and no blockers. There are more eyes, so fewer bugs. There are no silos, as the knowledge is constantly shared. We keep each other honest, no cutting corners, no poorly named variables or missing tests. The design has instant feedback from the group - fixing one of the common bugbears of pull requests where someone points out a more preferable solution at the end of the development.

Knowledge and experience is shared extremely efficiently. We all learn about the domain and about good software practices and patterns. We learn new things about our chosen language and increase our knowledge of the tools we use. We share decisions and gain a shared understanding.

In my experience, it's resulted in higher quality code and a better solution, with less rework and fewer bugs. It's also delivered more value to the customer more quickly.

# Dealing with change

Criticisms of mob programming are quite common. It doesn't look or sound like it would be an efficient way of working. Personally, I think it is and [many others have found the same](https://mobprogramming.org/). In agile ways of working, teams are multi-disciplinary and autonomous, which makes them well suited to mob programming (if they agree of course, since by definition it's up to them to decide how to work). It's equally valid for a team to decide to mob all the time or just with certain pieces of work.

As with any change, it's good to measure its effects. So, to understand if mob programming is working for you, try running some experiments and measure the change in cycle/lead times and defect rates. This can also be used to help reassure the rest of the business that it's the right thing to be doing.

Since it's a change to the team way of working, consider conducting regular [team health checks](https://engineering.atspotify.com/2014/09/16/squad-health-check-model/), in particular checking on psychological safety, and continuing to conduct regular team retros.

I've found these points particularly important to remember in the transition to remote working, during a pandemic. This wasn't like any normal remote working situation, as both the business and individual team members dealt with a lot of change in a very stressful environment. Even though the team I was in was mob programming before the pandemic hit, it wasn't the same afterwards. So regular health checks and retros became key for the team, while our focus on delivering value quickly became key for the business. This allowed us to adapt and improve our ways of working for the new situation.

## Working during a pandemic

COVID-19 has affected everyone in different ways and at different times. The collaborative environment of a mob, with high psychological safety, has enabled us to provide extra support to each other when needed. It has also provided a high degree of resilience as people have needed to drop out at short notice or just take a step back for different reasons.

A disadvantage of mob programming is that it requires synchronous working. Whereas, a major advantage of remote working is the asynchronous working opportunities that it affords. In the case of COVID-19, asynchronous working has been essential as people dealt with many, varied real-life things. In my team we've experimented with using a wolf-pack technique, whereby we'll come together frequently as a full mob for short periods of time, then find some tasks to enable people to work by themselves. A divide and conquer approach.

# How does that work remotely?

Mob programming remotely works just as well as in the office, in fact probably better in my experience. We are still co-located, just virtually. I have much more control over my environment now -  controlling things like the noise levels, my own keyboard and chair. It's easier to ensure I'm always facing the screen directly and not at a weird angle that I regret later. Obviously, there have been times when that's not been the case, for example the noise levels when my neighbours were having building work done was frustrating and I found my room got unpleasantly warm during the summer. Sometimes ignoring Slack messages while in a mob has been challenging too.

Overall, remote mob programming works well and offers more flexibility, but has required some adaptation too. In the following sections, I'll describe some of the tools and practices I've used to adjust to mob programming remotely during a pandemic.

## Getting started

Firstly, communicate. Lots. Don't assume that people know what you are thinking. Speak up when something's bothering you, and listen with kindness and curiosity when other people are speaking.

Use any waiting time for relaxed chatter. Check in with people and ask questions! There's less opportunity for informal water cooler chat when remote, so create some opportunities.

Take lots of breaks. More than you'd expect. Mob programming is tiring, even when not remote. Zoom's 40 minute call limit on the free tier is really useful for enforcing this. In my experience, a ten minute break every 40 mins is not unreasonable, it's intense work and it means Slack messages and emails can easily be ignored while you work because the next break isn't far off. That break can be used for some important thinking time too - I'm sure I solve more problems by going off to make a cup of tea than sitting at the computer.

### Structuring mob programming sessions

This is how I'd recommend structuring a mob programming session:

1. Set a goal for a session. Even better, write it down somewhere
2. Agree how you're going to work before you start (e.g when you'll take breaks and swap drivers), but expect this to evolve over the session. Mention anything that might get in the way (i.e if you need to dropout soon for a meeting or that you're puppy sitting for the day so might experience interruptions).
3. Reflect at the end of the session. Agree what you're going to do more, or less, of next time.

## Technology considerations

When selecting any tools, I would recommend focusing on those that facilitate communication and reduce friction, especially when swapping drivers.

- Audio quality
    - A headset or a good quality mic is an essential if on calls for any length of time
    - Choose a tool that handles lag, feedback and background noise well. For example, MS Teams is particularly bad for audio quality and for people talking over each other. I've personally had a lot of success with Zoom, but other solutions are available.
- Video
    - It's helpful, but not essential, to see people when mob programming. I've found it really aids communication. However, I also take breaks where I'll turn off video for a bit, just to combat 'zoom fatigue'.
    - Two screens are extremely useful. I have video feeds of people on a laptop screen, with code on the main monitor that's directly facing me. This has the advantage of not needing to look at people directly all of the time, helping to avoid 'zoom fatigue' and increasing concentration.
- Screen share
    - Pick a tool with high quality resolution and the ability to annotate/draw on the screen.
    - Being able to remote control someone's computer is a significant advantage, as it allows for effortless swapping. This is especially useful for including people on code bases they don't usually work on.
    - Zoom is particularly good at all these points.
    - Note: this isn't necessarily required if using something like [VS Code Live Share](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare), where you are able to see someone else move around a code base, make edits and run tests, etc.
- Development environment / IDE
    - [VS Code Live Share](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare) is extremely useful, although less good for Java devs. It enables collaborative editing. It allows you to run tests or even use the terminal on someone else's computer. It's even possible to watch someone step through code without screen share. 
    - Pushing code onto a WIP branch, or using tools like [mob.sh](http://mob.sh), can remove the need to share the same environment.
- Swapping the person typing (aka the 'driver')
    - This tends to end up being less frequent when remote, because it's not as simple as plugging in another keyboard, although using something like Zoom remote control can mean it's every 5-10 minutes. Often I've found that people prefer to use their own machines and that swapping time drifts to every 40 mins - 1 hour or even longer.
    - Tools like [mob.sh](http://mob.sh) can make switching much quicker and easier. Sometimes a simple timer is all that's needed though.
- A virtual whiteboard
    - Essential for sharing thoughts and recording tasks. Use mind maps for breaking down problems and diagrams for potential solutions.
- Slack, or other team chat application
    - Try sharing links to the video/audio call in a shared team Slack channel, along with the goal of the session. This makes it easy for others to know what the mob is working on and to drop by (product owner with an update or fellow dev you haven't seen in a while). Having a public goal makes the intention of the session explicit, keeping the group honest and focused.

The preferred tools in my team are Zoom, VS Code Live Share and Miro (a virtual whiteboard). We haven't settled on a particular timer yet. I'm keen to try out mob.sh, as my colleagues have had success with it in other teams.

# References

**About mob programming**

[https://www.agilealliance.org/resources/experience-reports/mob-programming-agile2014/](https://www.agilealliance.org/resources/experience-reports/mob-programming-agile2014/) (article)

[https://leanpub.com/mobprogramming](https://leanpub.com/mobprogramming) (book)

[https://www.youtube.com/watch?v=SHOVVnRB4h0](https://www.youtube.com/watch?v=SHOVVnRB4h0) (talk)

[https://www.youtube.com/watch?v=p_pvslS4gEI](https://www.youtube.com/watch?v=p_pvslS4gEI) (time-lapse of a day mob programming)

**The benefits of mob programming in detail**

[https://philippe.bourgau.net/3-long-term-benefits-of-mob-programming-that-make-it-cost-effective/](https://philippe.bourgau.net/3-long-term-benefits-of-mob-programming-that-make-it-cost-effective/)

**Tips and experiences from a mob programming practitioner (and my colleague)**

[https://hatwell.github.io/tips-for-remote-pairing/](https://hatwell.github.io/tips-for-remote-pairing/)

**More tips for remote mob programming**

[https://proagile.se/blog/remote-mob-programming-insights-captured-during-a-webinar-with-woody-zuill](https://proagile.se/blog/remote-mob-programming-insights-captured-during-a-webinar-with-woody-zuill)
