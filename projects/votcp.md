---
title: VOT-CP
layout: page
---

[VOT-CP (VOT coding and predictions)](https://github.com/llcit/vot-cp)

## Inspiration

Voice onset time (VOT) is an acoustic measurement often used in linguistic research. However, obtaining such measurements is a task done by hand, slowing the research process for many linguists. As such, taking advantage of pre-existing resources, with the help of the Tech Center's staff, I created a Python library that helps automate the VOT measurement collection process. To access this tool, go to https://github.com/llcit/vot-cp.

## What it does

This took takes as input a sound file with natural speech and a time-aligned textgrid file segmented at the word and phone level, and it returns a new textgrid file with an additional tier that marks VOT of voiceless stops. This library makes use of [AutoVOT](https://github.com/mlml/autovot)'s capabilities as well as [PraatIO](https://github.com/timmahrt/praatIO) and [Parselmouth](https://parselmouth.readthedocs.io/en/stable/).

## How we built it

This project was the result of a summer internship with the Language Flagship Technology Innovation Center (Tech Center). I constructed this library in collaboration with [Dr. Richard Medina](https://clt.manoa.hawaii.edu/richard-medina/). 

## Challenge we ran into

How this project facilitates the collection of VOT data, there are some limitations with this program. For example, as it stands:
- The project only works on word initial stops.
- Accurate alignment is necessary for precise VOT results.
- Some restrictions on naming convenctions exists.

For more details, review the documentation for the project.
