.. How Do I Web Scale? 101 slides file, created by
   hieroglyph-quickstart on Sat Aug 24 22:35:00 2013.

.. DEFINITIONS

.. |br| raw:: html

    <br/>

===================================
“Your Web App Is Not Web Scale” 101
===================================

Seh Hui, Leong |br| August 2013, Webcamp KL

.. figure:: /_static/1658521615_9c3aa234d6_b.jpg
    :class: fill

    CC-BY-SA http://www.flickr.com/photos/47598386@N00/1658521615/

.. toctree::
   :maxdepth: 2


.. slide::
    :level: 2

    .. raw:: html

        <iframe width="640" height="360" src="http://www.youtube.com/embed/b2F-DItXtZs?feature=player_detailpage" frameborder="0" allowfullscreen></iframe>

.. rst-class:: title-fill

OMG Scaling Unicorn Magic!
==========================


… unless when it is not
-----------------------

Why You Don't Need Scale… At First
----------------------------------

Why?
----

* Because complexity will kill you sooner

    * Troubleshooting
    * Time spent learning or writing tools
    * Initial set up time
    * Security audits and checking

* Popular web frameworks makes it easier

What You Really Need To Do First
--------------------------------

* Monitoring!
* Munin

Know Thy Enemy
--------------

* Concurrent connections ()
* Request-to-response time
* Development time (and sometimes cost)


.. rst-class:: title-fill

Scaling Up A Simple Web App 101
===============================

(The Hand-Wavey Edition)

.. figure:: /_static/7533805968_b639d68a00_b.jpg
    :class: fill

    CC-BY-ND http://www.flickr.com/photos/65488604@N02/7533805968/

Where You Start
---------------

Static Content – Someone Else Can Handle It
-------------------------------------------

Adding A New Server
-------------------

Let's Scale Horizontally!
-------------------------


.. rst-class:: title-fill

More Tricks
===========

.. figure:: /_static/552152780_aa81e34d1a_b.jpg
    :class: fill

    CC-BY-NC http://www.flickr.com/photos/44124453791@N01/552152780/

More Reads Than Writes
----------------------

Some Request Needs Long Processing Time?
----------------------------------------

* Async
* RabbitMQ

What About NoSQL?
-----------------

* Using NoSQL database ≠ scalable solution
* Right tool for the right job

Congratulations! You're Now Smarter!
====================================

.. figure:: /_static/6966069023_5512204921_b.jpg
    :class: fill

    CC-BY http://www.flickr.com/photos/sylvainkalache/6966069023/

Today You've Learned
====================

* Scaling should not be your first priority, monitoring is
* Your three main reason to scale
* How to scale a simple web app
* Additional weapons to make things speedier

Tweet Me Maybe
==============

:Email: felixleong@gmail.com
:Facebook: http://facebook.com/leongsh/
:Twitter: http://twitter.com/felixleong/

**Code, Demo, Presentation**

http://github.com/felixleong/wckl_webscale_talk/

**License**

`Creative Commons Attribution-ShareAlike 3.0 Unported License`_.

.. _Creative Commons Attribution-ShareAlike 3.0 Unported License: http://creativecommons.org/licenses/by-sa/3.0/deed.en_US
