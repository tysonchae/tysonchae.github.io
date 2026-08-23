---
title: "Where My Work Ends"
tags: [team, culture, retro]
---

# Where My Work Ends

When you've been leading a project, or even just owning a piece of it, sooner or later the release date lands on top of your vacation. The obvious right answer is to stay involved, close out everything you can, and leave with your part handled. It rarely goes that cleanly.

People rotate in and out. Someone joins to help with one piece, that piece grows, and eventually they know it better than I do. Then staffing shifts and they're pulled off, then back on, then off again. After a few rounds of that, I couldn't always tell you which parts I actually touched.

## Being the one left behind

A teammate left for vacation without handing anything off. The developer who stayed had to assemble the commits and prep the release build. Mostly code he hadn't written, and he was the one who'd have to press the button.

You could see it on him.

So I offered to go through it together. We walked the commits one by one and checked the release build against them to make sure nothing had been dropped. It wasn't hard work. It just mattered a lot whether he did it alone or not.

What struck me afterward was that he never needed technical help. He demonstrates outstanding technical proficiency and operates at a level well above my own. He could read the code fine. What he didn't have was the sense that if the call turned out to be wrong, he wasn't going to eat it by himself. Sitting there looking at the same screen gave him that.

Release stress almost never comes from the difficulty of the work. It comes from carrying it alone.

## The last-commit trap

When the teammate came back from vacation, he said something like: you wrote the last commit, so you'd know better than me. I don't know that part.

That one stuck with me. It sounds reasonable and it isn't true, and more importantly it points the wrong way.

Whoever touched something last is not automatically the person who understands it. He had read someone else's code fast enough to get a build out — that's it. Why it was designed that way, what got tried and thrown away, where it's fragile: only the original author knows any of that. What the code does, you can read. Why it ended up like that disappears unless someone writes it down.

The bigger problem is what that sentence sets up. Nobody asked him to take on that risk. He covered for someone who wasn't there. Treating that as a transfer of ownership means **the person who filled the gap gets stuck with it for filling it.** Do that a few times and people stop reaching into anyone else's area. What you lose is worth far more than one piece of code.

## What I landed on

**My code isn't the boundary.**
If I was part of how something got built, I should care about it through to the end. Even when most of what's shipping came from someone else, I want to look at it, and I want whoever's shipping it to feel steady going in. That's part of the job.

**Start from them, not from me.**
"I should take a look at this" lands as an inspection no matter how carefully you say it, and the moment it reads as distrust, the intent stops mattering. So I start with what do you need from me before I'm gone. Then checking things is a response to a request, and it turns into two people looking at the same screen.

**Build ownership you can hand off, not ownership you hold.**
Just resolving to see everything through doesn't scale. Add a couple more projects and I'm either the bottleneck or I'm burned out. Getting things to a state where they run without me — that's the actual job.

Which means what needs writing down isn't an explanation of the code. It's why the decisions went the way they did, where the sharp edges are, how to roll back, and what has to happen before someone should call me. Ownership that only lives in my head leaves when I do.

**Attach the checking to the process, not to a person.**
A release checklist, rollback criteria, post-deploy verification steps — once those exist on paper, nobody is auditing anybody. You're both just reading the same document. What we did going through those commits was really an improvised version of that checklist.

**Being the shield is the most useful thing I can offer.**
There are areas where the other person knows more than I do. Me reading their code adds nothing technical. What I can add is context, history, and cover. The strongest reassurance you can leave before vacation isn't a code review — it's saying that if this breaks, it's on me. And it counts for more said in front of the team than said one-on-one.

## What's still unfinished

If this stays a private standard I hold myself to, nothing about the team changes. You just end up with one person who covers more and one who still doesn't, and that gap turns into quiet resentment eventually.

So it has to become a team norm instead of a personal one. A one-page handoff before vacation: what's in flight, what's risky, how to roll back, when to call. And a rule that a release has a named owner, not just a last committer. You can fix the problem that way without making it about a person.

And I owe the developer who got left holding it a conversation. That was never yours to carry alone. I think that lands harder than the stress did — being treated like it was just his to deal with is the part that sticks.
