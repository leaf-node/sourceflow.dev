---
title: "swirlnet"
date: 2017-02-15
layout: page
categories: [apps]
image: assets/img/swirlnet-icon.png
---

This page demonstrates an evolved neural network balancing an inverted double
(or jointed) pendulum. Click the arrows below the simulation to gently or
forcefully push the upper and lower pendula.

{% include swirlnet-demo.html %}

This network was trained using [swirlnet](https://github.com/leaf-node/swirlnet),
a neuroevolution library, and [phyzzie](https://github.com/leaf-node/phyzzie), a
physics simulation and Web display framework. Phyzzie uses Chipmunk-js for 2D
physics, and swirlnet is based on
[NEAT](http://www.cs.ucf.edu/~kstanley/neat.html) (NeuroEvolution of Augmenting
Topologies) ([white
paper](http://nn.cs.utexas.edu/downloads/papers/stanley.ec02.pdf)). I wrote
both of these libraries in JavaScript so they could be run server-side and
displayed on the Web.

I've made some [tweaks to the NEAT
algorithm](https://github.com/leaf-node/swirlnet/blob/master/VS-NEAT.md). If you
would like to take a look at the evolutionary algorithm in my source code, you
could start by looking at the [code for
reproduction](https://github.com/leaf-node/swirlnet.make-population/blob/master/src/reproduction.js).

The code is split up into multiple git repos and can be [installed via
npm](https://github.com/leaf-node/swirlnet/blob/master/README.md).

I wrote a library for [multi-core network
evolution](https://github.com/leaf-node/swirlnet-solver-async) that sends genomes
to subprocesses. You can try out the single threaded and multi-core variants of
XOR in the [swirlnet repository](https://github.com/leaf-node/swirlnet), or run
the [code for this demo](https://github.com/leaf-node/swirlnet-demos).

