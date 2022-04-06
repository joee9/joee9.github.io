---
layout: post
title:  Spotify Stats
date:   2022-04-05 11:09:09 -0400
categories: projects 
---

<!-- I have always been very interested in music. In fact, I've played the violin since before I was seven years old.  -->

# Introduction and Motivation

Since I started using Spotify in high school, one of my favorite times of year has been when I receive my Spotify Wrapped in December. I love knowing what I have listened to the most: albums, artists, and tracks. I discovered in late 2021 that I could, in fact, use the public Spotify API to learn information about my listening history, and from then on, I have been working on this project: [spotifystats](https://github.com/joee9/spotifystats/). This program automatically collects user listening data and creates an `.html` recap containing top artists, albums, and songs, including the number of times each was listened to, complete with album artwork and links to the relevant Spotify pages. I hope in this article to show my thought process behind the development of this project, what I aim to do, how I hope to improve it in the future, and what I've learned along the way.

# Setup

*Note*: throughout this discussion, I will use the Linux command line. Personally, I have an installation of WSL2 on Windows 11, so I can run code and develop within an Ubuntu environment quite easily. I will assume that this is familiar to the reader and that (if following along) the reader also has access to a Linux command line.


To effectively use this program, there are a few prerequisites. First, you will need an installation of python. For ease of use (mostly just in terms of dependencies) I use [anaconda python](https://www.anaconda.com/products/distribution). Anaconda comes installed with almost every commonly used scientific python package, has an easy to use package manager (`conda`), and takes care of most all dependencies and path issues that I have dealt with using straightforward `pip` and `python3`. To install Anaconda, use
{% highlight bash %}
wget ANACONDA-URL
{% endhighlight %}
