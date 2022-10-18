.. title: Ant in C Minor
.. slug: ant-in-c-minor
.. date: 2022-10-04 17:52:31 UTC+02:00
.. tags: langton, programming
.. category: 
.. link: 
.. description: 
.. type: text

.. figure:: /images/ant-in-c-minor.png
  :figwidth: 50%
  :align: right
  :alt: Musical notation of middle C in treble clef.


I managed to get an ant working in C. You can view the source code here: `Auntie Ant <https://github.com/ReaSu/Auntie_Ant/tree/c-with-smoke>`_.

Do I think it is a masterpiece of engineering? Not at all. (I'd call it C major if it were!) But it works, and I have learned a lot from it.

.. END_TEASER

C was the first language I'd learned at uni. I liked it a lot, and couldn't understand why anyone would ever want to use anything else. (Then I learned other languages, and now I know!) I was surprised at how much I'd forgotten - and how quickly it all came back.

Coding
------
The first challenge was the following: I had this two-dimensional array that represented the grid. I wanted to initialise it, and I wanted to get that code out of the way, in its own procedure. In an object oriented language, I'd have a class for the grid, and call a methods on an instance. How do you call a method on an array in C? You don't. Instead, pass a reference as a parameter to the function or procedure. It seemes almost like calls are backwards: Instead of ``grid.initialise()`` we have ``initialise(grid)``. I remember now how confused I was about the exact same thing, just the other way round, when learning OO. Funny how perception changes.

The next challenge came with compiling. I had done that from the command line hundreds of times, but that knowledge was buried under a huge pile of other stuff, and took some dusting to restore.

I'd expected to have a hard time getting to grips with pointers again. I remember well how difficult I found them. And yes, I had to look up the details again. But skimming the section on arrays and pointers in a textbook was enough to remind me. Interestingly, they make much more sense now than they did before! It feels like when I was first learning C, I'd tried to understand the lie of the land by walking around in it, and now I have more of a bird's eye perspective.

Testing and Design
------------------
For testing, I used `Smoke <https://github.com/SamirTalwar/smoke>`_ because comparing the program's output to expected output is exactly what I needed. My first attempt showed me just how little I'm used to outside-in testing. I started with what I thought was the easiest possible version: the output is a grid with size 1x1, the ant is on that one field, and it's facing north. I wrote a test for that, and then some code, wonderful.

Next I thought it might actually be nice to parameterise the size of the grid. I decided to use a command line argument because why not. New test, new code, new test is green - but the first test broke. I fixed that, then thought it might actually be nice to have non-square grids, so what if the first command line argument stands for the width, and the second one for the height. New test, more code, fidget around until all tests are green again. The code started to look messier than I'd liked.

The further I went with this, the uglier the code became. What if the program is called without any arguments? Or only one, where it's expecting two? I can use default values, sure. But I definitely want to be able to have an argument for the number of steps. So now we have three arguments. But I can omit the first two and use a default size. But then how would I know if the argument was for the size or for the number of steps? I know that it's possible to deal with that. But I noticed that with every new idea, I had to either adjust all previous tests, or write code that was useful only to pass the tests, not to actually get me closer to the finished product. And I didn't like that.

This is a very small code base - no more than 100 lines of code at that point - and already I had created a monster that was hard to change. No wonder people give up on TDD if this is their first experience! I decided to abandon the pile of mud and start over. The problem, I knew, was not TDD, or outside-in vs. inside-out, but the way I approached it.

Before my second attempt, I spent some time thinking about the 'user interface'. I put that in inverted commas, because there's not much of a UI going on at all. But still, someone (me) was going to invoke the program, and my customer (moi, again) insisted that steps and size of the grid had to be customisable. 

Instead of command line arguments, I decided to ask for user input at the start of the program. One, because it's much more user friendly, and two through ten, because I found it easier to test and write. If I ever wanted to give users more ways to customise the output, I'd know exactly what code to change.

The lesson I learned (again) is this: Save time by taking the time to think about the (user) interface before you write code. This is especially true with outside-in testing, but doesn't hurt either way.

Wrap-up
-------
I'm deliberately limiting myself to three items here:

Room for improvement
====================

* There is no error handling whatsoever. Input parameters are not validated, nor is there anything to prevent the ant from falling off the edge of its world (resulting in a segmentation fault).
* I made some bad design choices: e.g. why should the grid know which direction the ant is facing? That's entirely unnecessary, and forces me to use structs where a simple type would be enough. I think. I believe I was influenced by a version I did in Java a while back, where I ended up without an actual ant object.
* My functions and procedures could be shorter, and putting them in (a) header file(s) wouldn't hurt readability either.

Things I'm happy with
=====================
* I'm glad I started with C. It's good to know that the memory wasn't lost, merely hidden under a pile of other stuff.
* I'm surprised how much I learnt apart from language specifics, about how I approach this problem.
* I'm happy to have persevered, and I'm looking forward to more ants.

But first: knit.
