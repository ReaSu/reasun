.. title: How To Test Text Output In JUnit
.. slug: how-to-test-text-output-in-junit
.. date: 2022-06-08 18:34:43 UTC+02:00
.. status: draft
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text

I had this plan of programming Langton's Ant. It's a two-dimensional cellular automaton: a set of rules that are apllied in a two dimensional plane. Imagine the plane to be covered with square balck and white tiles. We place an ant on an arbitrary tile, and have it walk around according to the following rules: When the ant is on a white tile, it will turn right, and move to the adjacent tile. When it is on a black tile, the ant will instead turn left and move to the next tile. Whenever the ant leaves a tile, that tile will switch colours. Langton's Ant, as all cellular automata, is interesting because a small set of simple rules leads to complex behaviour.

I wanted to program Langton's Ant for several reasons: I wanted to have something easy to try out programming techniques. I wanted to have quick success after some rather frustrating experiences recently. And finally I wanted to use the result in fibre crafts.

Have I tried new techniques and learned many things? Yes. I got familiar with Eclipse, my new IDE of choice. I tried assertJ instead of the standard assertions that come with JUnit5. And I learned that simple things are not necessarily easy. 

I expected this to be an easy practice piece, a little étude, if you will. Reader, I have failed miserably. There are so many decisions to make! How do I model that plane - does it emerge as the ant moves around, or do I start with a fixed size? If I do the latter - what happens when the ant moves off the borders? Will the program stop, or does the ant re-appear on the opposite side of the grid? Do I need a plane at all, or will a list of visited tiles do, each with its position in relation to the other tiles and the current colour? Where should the behaviour be, with the ant or with the tile?
