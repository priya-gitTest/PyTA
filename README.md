# PyTA

*Python for Text Analytics (or Textual Analysis or Text Analysis or whatever)*

## Introduction

Welcome to the repository for PyTA, which in keeping with Pythonic tradition is pronounced *pie-ta* ("pie" as in the dessert, and not, as the phonetic spelling might suggest to some, the genre of religious painting). This repository was specifically designed for this workshop, and so please feel free to clone it or download it as well as to make comments and recommendations for revision. That is, welcome to open access scholarship which is modelled on the spirit  and practices of open source software development, where everyone can, and sometimes does, make an important contribution. Some big, and some bigger than they first appear. (Starting, no matter how small, is always better than not starting.)

The documents and scripts in this repository were developed, and are still in the process of development, not only as a path for you and others to follow, but also as a record of my own progress. Everywhere you look, you will actually see an almost infinite series of contributions from unseen others who have helped me either directly, by responding to questions on fora like [StackOverflow][], or indirectly by publishing notes on their blogs or creating repositories like this one or the one created by Charles Pence in the [previous workshop][]. (You can find me on StackOverflow [here][].)

As the name of this repository confirms, in this workshop, we are not going to be operating at just any command line, but mostly in the Python interactive shell. There are a number of powerful scripting languages available to digital humanists, each of which has its particular strengths, and each of which also has its peculiarities, confusions, or moments of hair-pulling. For our purposes, I have decided to use Python for one, principled reason: its NLP library, known as the NLTK (natural language toolkit), is remarkably powerful, remarkably easy to use, and used not only by a large number of scholars and scientists but also a diverse range of scholars and scientists, so there is lots of documentation available. 

(Speaking of documentation, the NLTK has a terrific book, _Natural Language Processing with Python_, which is available from O'Reilly both in paper -- I will bring my copy to show -- but if you buy it as an ebook, you get a PDF, an ePub, and a Kindle version associated with your account that you can download at any time. In the mean time, here's a link to the book on the [O'Reilly Store][] and the obligatory link to [Amazon][]. The authors of the book are also the developers of the NLTK, and, in that open access vein described above, they also maintain a [web version of the book][].)

* **Nota bene**: O'Reilly has made it possible for those attending the workshop to get the ebook for 50% off. Once you find [the book][], which is normally $38, all you need to do is put it in the shopping cart, and enter the coupon code **MBBGS** at checkout, to buy the complete ebook set for $19. (I use all three versions: the PDF and `epub` on my computer, the PDF on my iPad, and the `mobi` version on my Kindle.)

It should be noted that there are other languages out there, and that they may be either better suited to the kind of work you want to do or to the way your brain works. If you already know you want to work with lots of texts and you are oriented towards statistics, then [R][] might be something for you to explore. Similarly, if like Charles, you are interested in having an interactive web site that works readily with a database of materials, then  [Ruby][] may be a better choice for you, because of Rails. The same goes for other languages. In general, it's been my experience that the languages are not as hard as getting your brain to think in terms that let you do computation on things like texts which are used to thinking about in other ways. My journey took me briefly through Perl, before taking up Python. I like Ruby a lot -- it's a beautiful language, but it came down to the NLTK for me and the robustness of some of the other Python libraries. I have used R, and liked it, and I use it when working with large data sets, of which I do not have many. 

## Installation(s)

While preparing separate installation instructions for Mac and Windows users, I came across [Anaconda][], which has the version of Python with which we will be working as well as all the libraries upon which we will be calling. And, perhaps more importantly, it is an *All-in-One* solution. I downloaded and installed Anaconda on the Mac Mini in my kitchen, and, while it's a large download at 1.25GB, it it does the job. Follow the instructions provided on Continuum.io's site, and you should have what you need in short order. On our kitchen computer, Anaconda placed a *Launcher* icon on the desktop, which I moved to the Dock. Starting the *Launcher* opens a somewhat confusing window, but iPython (now Jupyter) notebooks are an option, and I will be providing users with a notebook from which to work. (It is, in fact, here in this repository.)

With that noted, if you are interested in how I install and setup Python on my workhorse laptop, then a complete description is available in the [Mac Installations][]. 

My apologies to the Linux users in the crowd: I just assumed you have enough nerdery to get this done on your own, but do let me know if this is a foolish assumption on my part.
 

[StackOverflow]: http://stackoverflow.com
[here]: http://stackoverflow.com/users/1457672/john-laudun
[previous workshop]: https://github.com/cpence/text-mining-workshop
[O'Reilly Store]: http://shop.oreilly.com/product/9780596516499.do
[Amazon]: http://amzn.to/1OMa1Gx
[web version of the book]: http://www.nltk.org/book/
[the book]: http://shop.oreilly.com/product/9780596516499.do
[R]: https://www.r-project.org
[Ruby]: https://www.ruby-lang.org/en/
[Anaconda]: http://docs.continuum.io/anaconda/install
[Mac Installations]: https://github.com/johnlaudun/PyTA/blob/master/Installation-Mac.md


# Useful Python Scripts for Texts #


## Upfront ##


This collection of "Useful Python Scripts for Texts" (UPST) was originally constructed for teaching students in an honors academic writing course. Like a lot of open source software, it has two characteristics:

1. it is free to share with others, and
2. it is indebted to more people than I can thank here.

The latter is especially true since I am entirely self-taught when it comes to coding in Python and each of these scripts is the product of a lot of scrutinizing of other scripts and copying of code until I understood how things worked and could write it myself. 

As a way to thank my many teachers, I have tried here to comment the scripts as thoroughly as I could, in the hope that I can help others in the same way I was helped.

All of this work is hereby in the [public domain][].


## Usage ##

In order to make these scripts as easy to use as possible, they are designed to be run from the command line. In the case of the latter, output can be captured from `stdout` by simply sending the results to a text file of the user's own naming:

    python pythonscript.py > output.txt

Yup, it's just that easy. 

[public domain]: http://creativecommons.org/publicdomain/