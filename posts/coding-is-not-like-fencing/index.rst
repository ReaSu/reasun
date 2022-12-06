.. title: Coding is not like Fencing
.. slug: coding-is-not-like-fencing
.. date: 2022-12-06 17:55:01 UTC+01:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text

.. figure:: /images/solothurner-fechtbuch.jpg
  :figwidth: 50%
  :align: right
  :alt: two 16th century drawings of fencing

  Image from `Solothurner Fechtbuch <https://commons.wikimedia.org/wiki/File:S_554_021.tif>`_ 

In the `last post </posts/coding-is-like-fencing/>`_ I wrote about how very tangible the results of the "artificial" exercise were at the fencing practice I obsered. Witnessing this made reflect on the deliberate practice we as software crafters do. I want to get to the bottom of this, and tease out the differences between the two kinds of practice.

.. END_TEASER

In the software crafting community we stress the importance of deliberate practice. The idea behind it is that writing software is a skill like playing a musical instrument or a sport. Deliberate practice is bread and butter for professional athletes and musicians, while a performance is the cherry on top. Software development is like constant performance, and is lacking the foundation of deliberate practice. Fencers pracitce specific movements in isolation before using them in bouts. Musicians practice specific runs before incorporating them in a piece. In deliberate practice you slow down, and focus all your attention on a given aspect of your skill. By slowing down you take the time to do it very exactly, as near perfect as possible. You commit a certain movement to muscle memory. Once you can perform it with confidence, you can add other elements, like speed, or more context. We want to do that with parts of writing software too. We practice to talk about code and to communicate our intentions when working in a pair or ensemble. We practice writing tests first, code later. We practice refactoring code that follows a specific anti-pattern or smell. The pieces of code or problem descriptions we practice on are called *Katas*. When we come together to practice as a group, we call that a *dojo*. Someone really liked the martial arts simile. When a dojo lasts for a whole day or more, we call it a *code retreat*. So much about definitions and parallels between music, sports, and coding.

The fencing practice can be broken down and generalised like this:
- there's a clearly defined problem within a larger context and this problem can be practiced in isolation
- many repetitions are possible within a short timeframe
- feedback is available after each repetition
- improvement can be expected within the given timeframe
- the problem can then be placed back into its usual context, and the benefit of the practice is immediately noticeable.

How does this compare to the kind of deliberate practice we do in dojos or at retreats? Many Katas are so general, they are a canvas to practice whatever you need or want to. Some - especially refactoring katas - target a very specific problem, so let's stick with them for the moment. They often contain several instances of the same code smell, so the refactoring can be repeated more than once when solving the kata once. Solving the same kata again adds more repetitions. The timeframe is often longer than it was in the fencing lesson I observed, but it's still possible to do a few repetitions within an hour. So far, there are clear parallels.

Feedback, I think, is where we start to deviate from the above. There is feedback from the tests, of course - they show if the refactoring was successful, or if nasty bugs have crept in. Provided that they are good tests. When writing tests is part of the exercise, then they are only as good as you made them. Let's assume that the tests are good, because we're practicing refactoring, not writing tests. These tests give feedback about the outcome, but they don't say much about the process. Isn't it the process we want to practice? Did you really get to your goal in a way that will work consistently? Was the success down to luck, or to your abilities? 

In dojos or at retreats, pairing partners can be a valuable source of feedback. Not all pairs are created equal, though, and sometimes both partners are equally lost, which renders improvements much more difficult.

The biggest difference, however, is the last part: Usually, when we practice, we don't get the chance to immediately try out the new skills in their natural habitat. It can happen, especially in trainings where practice sessions are immediately followed by work on production code. However, this isn't usually the case in dojos or at code retreats. We can't transfer the new skills to a non-artificial context, and may even loose them before we have a chance to use them. No retrospective - as important as they are - can replace this.

There's the idea that taking the time to practice with katas is like taking the time to thoroughly sharpen your axe before you cut down a tree. It seems to me it's more like sharpening a random set of cutting implements. Chances are that at one point, sooner or later, most of them will come in handy. And when the time of the fillet knive has come we can confidently pull it out of our toolbag - if we remember that we have it. And if we can find it. And if it's not blunted again by time.

Doing katas is not like the fencing practice, it's half of fencing practice at most. Do we need the other half? What would that look like? And is it true that it's up to each participant what and how much they learn at a dojo/retreat?

I think best while writing, and a lot of thinking has been going on while writing this. Chances are there will be a part three, dealing with the questions above.
