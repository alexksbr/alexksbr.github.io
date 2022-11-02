---
layout: post
title: “Agile” and a Developers Search for Meaning
categories: [Essay]
excerpt: An essay about the mindset behind Agile methodologies
---

I started professional software development sometime between 2013 and 2016. It was at a time where Agile methodologies like Scrum were something that teams and organizations "just did". It somehow morphed into a standard practice that was a default choice in software development. On the surface, Agile made sense to me, especially after I heard stories about this scary "waterfall". Instead of planning everything up front and then developing software that companies ship to their customers only afterward, we had shorter feedback cycles and could incorporate customer feedback much earlier. My gut told me this was a good thing (spoiler alert: today, I still think it is).

Nevertheless, it was too superficial to assume that Agile methodologies are a good idea simply because it was the default choice for most teams I worked in. I tried to understand the mindset and look at critical voices. I wanted to dig deeper.

# Software development is an inherently complex field

Before we discuss "Agile" as a mindset and its methodologies, let's take a step back. The Cynefin Framework categorizes problems into five buckets: simple, complicated, complex, chaotic, and disorder. Its purpose as a sense-making framework is to contextualize problems and choose appropriate solution strategies that best suites the problem at hand.

![Cynefin Framework](/assets/2022-11-02/cynefin.jpg)
Source: [Wikipedia](https://upload.wikimedia.org/wikipedia/commons/thumb/a/ab/Cynefin_framework_2022.jpg/800px-Cynefin_framework_2022.jpg)

The first section contains **clear** or **simple** problems. In this area, clear cause-and-effect relationships are predictable and repeatable. Therefore, after categorizing the problem, we have existing best practices or checklists to solve it. **Complicated** problems are a little more difficult. That is because they require experts to analyze it. Nevertheless, after analyzing the problem, we can follow a plan to solve it. We are in the realm of good practices instead of undisputed *best* practices since experts might have differing views on which plan to follow.

There are some problems where we can only determine the cause-and-effect relationship in hindsight. Enter the space of **complex** problems. Here we have unpredictable outcomes and must conduct experiments to determine what works and doesn't. There are also **chaotic** problems where we cannot establish cause and effect in the first place. In this space, it is essential to recognize it and find novel practices that might move the problem out of the chaotic zone. The space of **confusion** or **disorder** sits in the middle. That means our problem should reside in one of the other spaces, but we have difficulty determining which one. That is dangerous because people start to solve problems with the methods and tools they are most comfortable with, not those that fit the most to the current situation.

Software development lives in the space of complex problems. Why is that? First, we do not know beforehand how our users will use the system's features and in what combination they will use them. Often this leads to changes our users want to see that only become obvious after they start using the system. Second, we do not know what the best approach to solving the problem is in the first place. On top of that, we operate on top of a fast-changing software development ecosystem, where new frameworks and versions of dependencies appear daily. All of the reasons above make it very hard to predict what will happen after we start developing our system.

Martin Fowler [argues](https://www.martinfowler.com/articles/newMethodology.html) that software development is primarily a design activity, a creative process that is hard to plan. In contrast to plan-driven approaches used in civil engineering, highly predictable and plannable "construction work" is only a fraction of software development activities.

Classical approaches in software development heavily relied on up-front plans and up-front design. That completely neglects the complex nature we are dealing with. It treats software development as a complicated problem without considering the unpredictability of user needs, the evolution of the software development ecosystem, and the interdependency between the two.

# The promise of "Agile"

There is a difference between adaptive and predictive planning. While *predictive* planning aims to plan out iterations until the next milestone, with *adaptive* planning, we only focus on the upcoming iteration. Since we only plan one iteration and do that just in time, adaptive planning has the advantage that we can always use the most current information available. We might have made predictive plans on the least amount of information out of whatever knowledge was available at the beginning of the project. Agile methodologies are adaptive and heavily rely on the concept of iterations.

More than twenty years ago, the Agile Manifesto captured the mindset behind this shift with the following statements:
- **Individuals and interactions** over processes and tools
- **Working software** over comprehensive documentation
- **Customer collaboration** over contract negotiation
- **Responding to change** over following a plan

The following describes my interpretation of the agile mindset and what it promises.

**Agile is about responding to change**
If I'd ask you, "What is agile all about?" then responding to change would probably be one of the first things that come to mind. If we face uncertainty, it makes sense to work in small increments and decrease the amount of up-front planning since the plan would need to change soon anyway. It only makes sense to conduct experiments, fail as fast as possible and learn from the assumptions we have made. A consequence of this line of thought is that we want to deliver our system early and regularly to get feedback as fast as possible.

> "No plan survives contact with the enemy."

But what changes do we need to respond to in the first place? First, requirements change. They change because it is much easier to argue about a system, its features, and the usage workflow when customers can try out the system and experience it in the first place. Even when our users would perfectly know about the features and how they will use them, we would still need to factor in changing requirements. The reason for that is that the world around us also evolves. Our company might decide to enter a new market... or new competitors emerge, which could accelerate our project deadlines. Changes in the business world are [highly unpredictable](https://en.wikipedia.org/wiki/Fooled_by_Randomness), as every serious stock trader would tell you.

Second, we have to deal with an evolving software development ecosystem. Operating Systems, Container Orchestrators, Cloud-Environments, Frameworks, and Libraries are only examples of tools we use in our day-to-day development. All of them evolve independently and sometimes in unexpected directions. Some of them have security issues that need to be fixed urgently. On top of that, new tools emerge, often in an unpredictable way. Few people could have predicted the impact of Docker before it was released and widely adopted.

**Agile is about people**
As we have discussed above, software development is creative work. As with other creative work, individuals are not replaceable and make unique contributions to the software project. Each individual has a background, experiences, strengths, and weaknesses which can uniquely and positively impact a software project. Therefore, it makes sense to see people as first-class citizens in the software development process instead of treating them like replaceable gears in a factory - as classical, plan-based approaches often do.

**Agile is a mindset**
After the ending of World War II, inhabitants of the Melanesian islands in the south pacific practiced something that western observers later called "Cargo Cult". During the war, Allied forces dropped packaged equipment and food items onto military bases stationed on the islands. It profoundly impacted the islanders since the military shared some of the goods with them - increasing their standard of living significantly. After the war, when the military bases were removed from the islands, inhabitants were short of supply and the abundance it brought.
They believed that western technology (such as airplanes, headsets, and landing towers) worshipped spiritual entities, which then dropped equipment and food packages onto the island. What happened was that the islanders began to build their own airplanes, headsets, and landing towers out of straw and practiced military formations with wooden weapons as a spiritual act. The spiritual worship did not result in packages being dropped from the air.

The message here is that it is also worthless to implement Agile methodologies without adopting their principles and worldview. Using processes like Scrum or XP only works as far as the holding beliefs are adapted as well. Otherwise, you will land on an island full of buzzwords without embracing Agile as what it truly is: a mindset.

Out of that mindset follow the practices: we write tests and embrace continuous delivery because it makes it easier for us to deliver working software faster and more often. We hold daily stand-ups to find out if team members can help each other to clear away impediments because we believe that Agile is about people first. We conduct experiments to see what works and what doesn't work. And we want to release software more often because it helps us collaborate with our customers in the first place.

# "Agile" is no means to an end
A journey to the meaning of "Agile" should not neglect the critics and look for circumstances where it might not work as well. One [opinion from a former Google Engineering Director](https://www.quora.com/Why-do-some-developers-at-strong-companies-like-Google-consider-Agile-development-to-be-nonsense/answer/David-Jeske?share=1) argues that it does not work well for products with a small and straightforward API but complex internal components behind. Think of things like Google Bigtable. It is hard to iteratively improve software based on user feedback when the API is small and stable, and the things that change most often are internal APIs. However, this misses a critical angle: the API is only one of many observable behaviors from users. We may find that users have special requirements for performance or storage efficiency, so we must adapt internal algorithms to reach those goals. In addition, only because we do not have to evolve a small and straightforward API, it does not mean that working in smaller iterations is a bad idea in the first place. It gives confidence to teams that they can ship working software. It helps product owners to reprioritize certain things during development, especially when there is no up-front plan. Those systems require a more sophisticated up-front design, which is consistent with the mindset we discussed above. If done right, we can see the up-front design as more of a vision or "best guess" and keep it useful and flexible enough. But this is a topic for another blog post.

One of the fundamental problems with "Agile" lies in its adoption. Superficial adoption of the methodologies and thinking it is a silver bullet is a significant obstacle. We need a deep understanding of the mindset behind the methods - by all involved stakeholders, not only technical but also from leadership positions.

What is essential for teams is to have a safe space to try things out, potentially fail and have the room to learn from them. Leadership and management have to embrace that. It is fundamental not to see those methodologies as a control mechanism but as a mindset that helps to deliver features faster, embrace people as creatives and make room for experimentation and growth.

# References
- ["The New Methodology"](https://www.martinfowler.com/articles/newMethodology.html) by Martin Fowler
- [The "Manifesto for Agile Software Development"](http://agilemanifesto.org/)
- ["The Cynefin Framework"](https://www.youtube.com/watch?v=N7oz366X0-8) by David Snowden