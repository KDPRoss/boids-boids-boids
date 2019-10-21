# boids-boids-boids

Little boids simulation in JavaScript attempting to
replicate shoals of bait fish. It uses the classic
heuristics:

* Separation (no boid should be too close to any other).
* Alignment (boids try to fly in the same direction as
  nearby ones are).
* Cohesion (boids try to stay with one another).

## Future Work

I hacked this together fairly quickly; I'd call this 'Matt
Parker style' code (although, to be fair, I'm not importing
libraries in a loop body). Some obvious improvements that
could be made:

* Boids currently have 360-degree vision, which is nonstandard.
* Use quadtrees to do KNN (rather than the
  uniform-partitioning scheme that I tossed together).
* Use some linear-algebra library to handle vectors and
  associated maths (rather than hand-coded component-wise
  implementations).

## Resources

* See [the Wikipedia page](https://en.wikipedia.org/wiki/Boids)
  for more info about Reynold's classic Siggraph 1987 paper.
* Here's
  [a video where I discuss the implementation](https://youtu.be/KkFfhVhwsmQ)
  (at a very high level).
* Because of the magic of JS, you can
  [run it in your browser](http://tinyurl.com/yyun6wqf); you
  *know* that you have CPU cycles to spare!
