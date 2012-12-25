urlextractor v0.1
============

Python URL Extractor - extract URLs from text

*** Warning: This code works but is extremely hacky, patches welcome ***

Extract a URL from free-form text

Converts this:

"The website google.com is often used to search the internet, I used it to discover news.ycombinator.com which in turn led me to www.paulgraham.com/articles.html"

To:

[((12, 22), 'google.com'), ((83, 103), 'news.ycombinator.com'), ((128, 160), 'www.paulgraham.com/articles.html')]

(use parseText(textstring) to use it)

This was originally written for a hackday as something better than twitter-text-python to automatically identify URLs in user written text for automated linking.

Rather than simply search for "http" it looks for TLDs and attempts to construct URLs around them. It largely works through regexs which while not strictly conforming to RFCs tend to be pretty accurate for real life usage.

At some point I plan to tidy it up into a nice package with tests, commenting and a general better structure.

:copyright: (c) 2012 by Imran Ghory
:license: MIT Licene

