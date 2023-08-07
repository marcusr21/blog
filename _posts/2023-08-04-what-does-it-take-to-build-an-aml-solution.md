---
layout: post
title: "What does it take to build an AML Solution?"
date: 2023-08-04 12:00
social: assets/article_images/2023-08-04-what-does-it-take-to-build-an-aml-solution/banner.png
---

What does it take to build a full AML solution from the ground up? A team of 30 developers? With 3 QAs, a Product Owner, Product Manager, Scrum Master, Project Manager and 3 UX and UI experts?

What if I told you, that it took 3 developers (1 x backend, 1 x frontend & 1 x full-stack), 1 QA, 1 UX and 1 Product Manager, four months to build and release a secure AML ID Checks, integrated into an existing app whilst working with a brand-new partner and vendor for the first time?

![Would you believe me?]({{site.baseurl}}/assets/article_images/2023-08-04-what-does-it-take-to-build-an-aml-solution/what_if_told_you.jpeg)

## Shaping Up
In 2022, I was introduced to the development framework called [Shape Up by Basecamp](https://basecamp.com/shapeup). For those who haven't read it, or come across it before, I'd definitely recommend reading into it. 

_The book is free to download, the website is incredible, please take a look! (Not an ad!)._

When you're working in small teams, you might find your developers distracted by endless meetings and never truly "delivering" anything. 
I know I've experienced this feeling using Scrum (the default framework for most development teams).

Shape Up's concept at its core, is delivering a piece of work, end-to-end, in a timeframe allocated. The default is six weeks, the development team focus on **only** building this piece of work, no bugs or distractions, and at the end they deliver a feature or product or whatever was decided.

At the end of the intense development cycle, there is a cool-down of two weeks to focus on BAU tasks and allowing the developers to take on some stretch and personal development tasks.

The piece of work, before it reaches the developers, has been "shaped-up" by a core team of a PM, UX (who will be part of the development team) and a Senior Developer, who'll offer input on "what's possible". The Shaping Up process happens before it reaches the development team, meaning a fully fleshed out project reaches them, they can ask questions, breakdown tasks and work away whilst delivering regular updates.

## Keep It Simple! 

It's easy to want every feature possible. Who doesn't want an all singing and all dancing solution? Trust me, as a developer, I would love to deliver this for you.

The reality is though, we have limited resource, limited time and an ever-growing list of key features.

![Don't make it harder than it needs to be!]({{site.baseurl}}/assets/article_images/2023-08-04-what-does-it-take-to-build-an-aml-solution/shouldnt_be_hard.png)

This is where we really rely on our Product Manager to be objectively clear. What are the **Must-Have's** and what are the **Nice to Have's**? 

When we're developing, we can truly focus on these deliverables and avoid the classic case of chasing a rabbit down a hole, finding a solution for something that isn't even scope? We've all become obsessed with fixing an obscure issue, spending a week fixing, testing before realising that it's not required or no added value has been gained.

If we start finding that either we're ahead of the curve with development, or slipping behind, we can revisit this list and understand where to focus our efforts. 

Within our AML build, from Day 1 we knew **_exactly_** what was required, with a full project plan, the must-haves and a list of "nice to haves". Our incredible UX had already begun mocking up some screens that we could validate and, as the backend developer, I had already been provided with our vendors API. 

All of this hard work, and keeping it simple, means we can hit the ground running and divide up tasks to work on as a team. You could even think of these tasks as slices... 

## Working in Slices, Instead of Silo's

When building a solution with a decoupled backend and frontend, it's very easy for one to be waiting on the other to complete work. Previously, when we've worked in Scrum, we have found that the frontend is typically waiting for work for half the sprint, followed by a flurry to complete it
and get it tested by QA before the end of the sprint.

What does this result in? Wasted resource waiting to complete their stories & tasks, 
an angry QA who is rushing to validate and raise bugs, stressed DevOps who need to complete the pipeline
and finally, a reduced velocity (if you're doing Scrum).

![Working in Silo's]({{site.baseurl}}/assets/article_images/2023-08-04-what-does-it-take-to-build-an-aml-solution/backend-frontend-mismatch.png)

Enter, "working in slices".

Rather than a "frontend" team, a "backend" team we work as one. We analyse the requirement, create the _"Scopes"_ (large pieces of work), before breaking these down into tasks. The entire team is responsible for delivering _Scopes_.
Tasks are assigned to the individual developer, but with consistent and constant communication we work together.

Take for instance, AML Checks. We know that an accountant needs to execute a "Basic" check. Frontend will take the screens from UX, whilst backend is creating the API call for both sending and receiving data. 
We work together, iterating over data structure and requirements until we have something that we're happy with. 
But, rather than waiting on backend to decide the data structure for `GET` and `POST` and write all their tests (~4 days worth of work) before frontend gets started, within 3 hours we have a general data structure, some test data and a clear path forward.

![Working in Slices]({{site.baseurl}}/assets/article_images/2023-08-04-what-does-it-take-to-build-an-aml-solution/backend-frontend-aligned.png)

By the end of Wednesday, we have a full working MVP for a "Basic check", a core requirement. This is by no means the finished version, we iterated over and over again for 2 weeks and the base calls had data added and removed. Most importantly, our stakeholders within the business can see **_clear progress_**.

## Maintaining the Momentum

It's very easy to start a Sprint or a "Development cycle" which you tell the team will be "intensive but worthwhile".

But when the inevitable bugs, or questions, or sickness and absence kicks in, how do you maintain momentum?

We were a small team, three developers, a QA and a UX, everyone has their part to play and everyone takes accountability.

First, **communicate**. 95% of issues that occur in business come down to communication. Something got lost in translation, the priority wasn't set high enough or even, the person wasn't told.
Communication is critical for humans to survive and thrive, the same goes for development teams. If you're going away, tell the team and make sure they're aware of where we got up to.
When you've completed a task or API, tell the team (including your QA!). If the environment has changed, tell the team! 
If something can't be achieved, tell your lead developer, and we'll engage our vendor and Product Manager.

Second, **_communicate_**. I can't stress this enough people. We are a remote first team, and meet every 2 weeks. But, daily stand-ups, "dev-only" Slack chats with regular calls and "huddles" makes it feel like you're working together all the time.

_Side note, case in point. As lead backend, I was struggling to understand why a bug was occurring. I got my frontend and QA into a call quickly, watched **exactly** what was happening and within 30 minutes, we had a solution ready for QA._

Third, leave no stone unturned. Just because your frontend is a React developer, doesn't mean they're silo'd to that technology.
Our core application is built from PHP and VueJS, I asked our frontend "can you take a look", within three days he'd both fixed the issue, and refactored the code into something extendable.

There will be days when it gets tough and feels like a chore, that happens. But being the inspiring person in a room and helping the team helps you to regain the momentum. 
Remember though, planning has taken place so development is completed, way before Go Live.

## Bringing It All Together

So, what does it take to build a fully working AML Checks solution in four months?

Well, after leading the team for four months I can tell you:
- Trust and teamwork.
- Accountability and responsibility.
- An incredible vendor, who'll answer your calls and questions no matter how stupid.
- Clear requirements from Product Manager.
- Proper planning from Day 1 with an achievable Go To Market date.
  - Pen test plan.
  - Alpha and Beta plan.
  - Go-live plan.
- Cutting edge and clear UX Figma designs.
- A development framework which free's the developers to do what they do best.
- Regular communication and collaboration.

Tick this list off, and your dev team can achieve anything in the world. We proved ourselves wrong and I couldn't be prouder to lead the team.