.. title: Baby steps challenge
.. slug: baby-steps-challenge
.. date: 2021-12-25 20:24:57 UTC+01:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
.. status: draft

technical agile coaching
I was recently co-facilitating a refactoring workshop with Peter. We did the baby steps challenge: The participants worked in pairs to refactor a rather small piece of code (Parrot Kata, for those interested). As an extra challenge, they should break up each change into as many meaningful steps as possible. Peter has this tool that counts commits and displays a score board - he wrote a whole blog post about it: [http://blog.code-cop.org/2021/09/baby-steps-push-challenge.html] - which turns the exercise into a competition between the pairs.

At the end of the workshop we had a mini retro, and most participants repeated the same things - interesting how small you can go, fun challenge, etc. etc. Only one of them named the elefant in the room: why on earth should we make such small steps? Changing the accessibility of one variable after another, instead of doing all five of them in one commit, that's nowhere near realistic. So, what's the point?

First, I have to congratulate this participants to NOT nod along with all the others. It's not easy to go against the majority of the group. For most people it's also difficult to give critical feedback, especially to someone in a position of authority. So: Thank you for your courage to speak up and voice your concerns!

Second, I find this is an excellent question, because there's many layers to the answer. 

It is obviously an exercise of refactoring, and of looking at refactorings. Instead of letting the IDE do all the work for us, we have to analyse the problem, plan out the steps, think about the most sensible order of the steps to keep the tests green throughout. This gives us a deeper understanding of what we are actually doing, why we are doing it, and what is involved in this step.

Taking extremely small steps also forces us to take a step back, be clear about what we want, and communicating it clearly to our partner. It never hurts to practise communication.

Adrian Bolboaca [https://blog.adrianbolboaca.ro/2013/03/taking-baby-steps/] also mentions focus: Stay focussed on one task and see it through to the end. The smaller the step you take, the easier it is to complete it before you get distracted or interrupted.

Yet another reason for taking extremely small steps is that restrictions spark creativity. Programming is a creative task, so everything that forces us to light that creative spark again is helpful.

Additionally, they experience that the tiniest steps will ultimately lead to their goal. They experience that it's not necessarily much slower than taking bigger steps. They experience how good it feels to have the safety that nothing can go terribly wrong, because the last working version of the code is, literally, only a step away.

A completely different reason is to re-calibrate our sense of what an appropriatly sized step looks like. Up to now, we worked in steps of size X - whatever that may be. Someone comes along and tells us to work in smaller steps. Well, X-1 is a smaller step. We're told to go even smaller, so we try X-2, and we feel really good about it. But what we should be doing is X/2 or X/10. But that's not even on our radar!

By forcing forcing ourselves to take the smallest possible steps, we get a better view of what is possible, we widen our frame of reference. Suddenly, X/2 is not only on the radar, it doesn't even look all that small anymore. Because we have not only X to compare it to, but also Y, the smalles possible step.

I come across this problem over and over again: trying to compare something without a proper frame of reference. Without knowing what to compare it with. And I will write more about that another time. For now I want to conclude by listing the very different, but important points I want you to take home from this story:

* Voicing concern in front of a crowd takes courage. Do it more often.
* Restrictions force creativity.
* Comparison needs a frame of reference, or it doesn't make any sense.
