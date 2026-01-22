---
layout: post_comment
title: A little game about knowledge
categories: tech
comment_id: '115938039738751975'
---
Science is incredibly effective and usually, once a hypothesis is widely accepted enough it will be considered truth (at least for the purpose of science communication or teaching). But what does it mean to come up with a hypothesis? How can we predict how the world we are observing will behave? And where can the scientific method lead us to convictions that are not in accordance with the ground truth?

Together with [Andrei](https://github.com/andcov), I started to develop a little game about different scenarios or riddles, for which in order to solve the level, the players have to build a model which correctly predicts the scenarios physics.

> Be aware: The website sometimes takes long to load, we will try to optimize this in the future

You can find the game under this URL: <https://jon011235.github.io/foundation-of-science-game>
and the source code under <https://github.com/jon011235/foundation-of-science-game>.

We are eager for some players and feedback and will continue to develop the game further.

## Tech stack
For those interested:

Every Level is a python class and you can also play this game locally (for instance with the `terminal_interface.py` in the repository). There are even some levels that are not integrated in the website at the time of writing, as they require additional features.

The interface is build through [marimo](https://marimo.io) which allows to build [jupyter notebook](https://jupyter.org/) like notebooks, but it is easy to export them to static files with the help of [WASM](https://webassembly.org/) (the infrastructure for python used is [pyodide](https://pyodide.org/)). Furthermore marimo notebooks are reactive and keep the state of all cells consistent, which is really nice.

The interface then just loads the level and you're ready to play.
The front page is built using jekyll (like this blog), which is a bit of an overkill for just one HTML site.

Really cool what frameworks and tools exist today!

While we have used a lot of LLM assistant, especially for the interface all the concepts and ideas are our own.