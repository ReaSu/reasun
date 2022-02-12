.. title: Baby Steps Challenge
.. slug: baby-steps-challenge
.. date: 2022-02-12 15:24:57 UTC+01:00
.. tags: agile coaching,refactoring,programming
.. category: 
.. link: 
.. description: 
.. type: text

.. figure:: /images/baby-steps.jpg
  :figwidth: 50%
  :align: right
  :alt: elephant calf walking next to grown elephant

  Image by `Kirsi Kataniemi <https://pixabay.com/users/kikatani-35407/>`_
 
I recently co-facilitated a refactoring workshop with `Code Cop Peter Kofler <http://code-cop.org>`_, where a participant asked an interesting question. I used to read people's blogs or listen to their talks, and they always started with "recently someone asked/mentioned/said this thing and so I thought I'd write something/give this talk about it." I used to think they just make this stuff up to have a better intro. And look at me now! 

It was really a participant's question, I swear! But I still lied for the sake of sounding like those interesting people: it wasn't "recently", it was last year. Writing this post took so much longer than anticipated, because the more I thought about it, the more things came to my mind. It needed a lot of refactoring. For you non-coders: refactoring code is much like revising a text. You move bits around and maybe change some words, so it all becomes more coherent and less repetitive. The thing you don't want to change is the meaning, or, in the case of code, what it does. I love doing it with code, but not so much with texts. I hope you can still follow my train of thought. So here goes:

.. END_TEASER 

In this workshop, participants worked in pairs to refactor a piece of code (Parrot Kata, for those interested). To spice things up, they were given the extra challenge to do it in baby steps: to break each change into as many smaller steps as possible, and commit after each change. For the non-coders: "commit" in this context can be read as "upload the changed code". There's more to it, but that's not relevant here. It takes basically no time at all to do it. Most programmers should do it more often.

Peter came up with this cool tool that counts commits for each pair and displays a score board - check out his blog post about it `here <http://blog.code-cop.org/2021/09/baby-steps-push-challenge.html>`_. This adds an element of gamification on top of the challenge by turning it into a competition between the pairs.

At the end of the workshop we had a mini retro, as usual. Most participants repeated the same things as usual - it's eye-opening how much you can break up an already easy step, it's interesting how small you can go, fun challenge, etc. etc. Only one of them named the elephant in the room: why on earth should we make such small steps? Changing the accessibility of one variable after another, instead of doing all five of them in one commit, that's nowhere near realistic. So, what's the point?

First, I want to congratulate this participant on NOT nodding along with all the others. Giving well-founded, critical feedback after a workshop seems to be difficult for most people. Otherwise I'd get more of it. But it's even harder to voice concerns when you go against the majority of the group. So: thank you, dear participant, for your courage to speak up and voice your concerns! 

Second, I find this is an excellent question, because there's so many reasons why everyone should try baby steps from time to time. Honestly, I was surprised just how many reasons I could find when thinking about it for a bit. Here's what I came up with:

It's obviously an exercise in refactoring, and in looking at refactorings. Instead of letting the IDE do all the work for us, we have to analyse the problem, plan out the steps, think about the most sensible order of those steps to keep the tests green (the code woring) throughout. This gives us a deeper understanding of what we are actually doing, why we are doing it, and what is involved in this step.

Taking extremely small steps also forces us to take a step back, be clear about what we want, and communicating it clearly to our partner. It never hurts to practise communication.

Adrian Bolboaca, the father of Code Retreats in Europe, also `mentions <https://blog.adrianbolboaca.ro/2013/03/taking-baby-steps/>`_ focus: Stay focussed on one task and see it through to the end. The smaller the step you take, the easier it is to complete it before you get distracted or interrupted.

Yet another reason for taking extremely small steps is that restrictions spark creativity. It's easy to forget in the everyday grind, but programming is in essence a creative task. It's refreshing to remind ourselves of this from time to time. It helps to fall in love with programming all over again.

Additionally, there's the experience of the compound effect: that even the tiniest steps will ultimately lead to a big change. This can scale - we don't have to re-write all our code, it will become better if we keep doing small changes. 

Think twice, cut once. Take time to save time. Many figures of speech that are founded in crafts apply to code as well: It doesn't necessarily take longer to take many small steps, because big steps are more prone to error. 

We also shouldn't discard how good it feels to have the safety that nothing can go terribly wrong, because the last working version of the code is, literally, only a step away.

The reason that actually made me write this whole post is of an entirely different nature: The baby step challenge helps us to calibrate our sense of what an appropriatly sized step looks like. The problem is not that our workshop participants (or any programmer, for that matter!) is too stupid to refactor in small steps. The problem is that *small* has no meaning of it's own. Even the smallest elephant is huge compared to a mouse! Adjectives like *small* or *big* make sense only in relation to something else, to a norm, or on a scale. In order to understand what *small* means in refactoring, we have to see where the lower end of that scale is. This Baby Step Challenge allows us the explore exactly that. It's not something we do in our everyday work, there's no time for it. That's why Coding Dojos and Code Retreats are so valuable.

I come across this problem over and over again: trying to compare something without a proper frame of reference. Without knowing what to compare it to. But this is another story that shall be told another time. Here's the **TL;DR:**

* Voicing concern in front of a crowd takes courage. Do it more often.
* Small steps can take you far.
* Restrictions force creativity.
* Comparison needs a frame of reference. 

Have I missed any reasons for taking things one small step at a time? Let me know in the comments!

I mean it! You don't have to log in, you can comment anonymously. But if you happen to have a matrix account, feel free to use it.
