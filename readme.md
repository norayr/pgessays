Script to download and make epub from Paul Graham's essays
==============================
originally taken from [this](https://gist.github.com/norayr/94eb86cc9d4f85ff75ec) gist fork.

this actually works, but fails with a couple of essays. I do not know why, decided to publish it, you can may be improve it.

I do not know python, but I was able to do two changes:

* change BeautifulSoup to bs4 in import section
* change the table width to 435 by viewing Paul's page source.

Requirements
============

I have emerged genshi, beautifulsoup, lxml in my funtoo system.
I had also to download, unpack and put in the same directory python-epub-builderfrom [here](https://code.google.com/p/python-epub-builder/) on google code.

I include it with pgessays.py distribution.

Python-epub-builder requires epubcheck jar file, which checks epub for errors.
I was unable to make any of downloaded epubcheck versions work on my systems. It does not matter, because epub is already created before the check.

Running
=======

Run python, or <code>python2 pgessays.py</code>

As I said it'll fail, but will create the book.

You can convert it to let's say moby if you have Calibre installed with

<code>ebook-convert <name>.epub <name>.mobi</code>

or similar commands. Enjoy.

Read
=====
In any case I am distributing the result in essays directory.
In epub and mobi format.
