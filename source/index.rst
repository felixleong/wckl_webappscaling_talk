.. Scaling Your Web App – The Basics slides file, created by
   hieroglyph-quickstart on Sat Aug 24 22:35:00 2013.

.. DEFINITIONS

.. |br| raw:: html

    <br/>

=================================
Scaling Your Web App – The Basics
=================================

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

.. figure:: /_static/scaling-magic.png
    :class: fill


… unless when it is not
-----------------------

.. figure:: /_static/scaling-stupidz.png
    :class: fill

Why You Don't Need Scale… At First
----------------------------------

* Because **complexity will kill you sooner**

    * Initial set up time
    * Time spent learning and/or writing tools
    * Troubleshooting
    * Security audits and checking

* Besides, popular web frameworks makes it easier

What You Really Need To Do First
================================

.. figure:: /_static/munin.png
    :class: fill

Know Thy Enemy
--------------

* Traffic/Concurrent connections
* Request-to-response time *(look out for tasks that clogs your WSGI threads)*
* Development time *(and sometimes cost)*
* CPU load
* … and more intertwining factors

When To Scale?
--------------

* Identify the key bottleneck contributor
* Look for slow requests or DB queries and optimize those first
* Adding new servers should always be **the last resort to buy time** *(i.e. too complex to solve in short notice)*
* Yes, servers are cheaper than developers, but all costs stacks

.. rst-class:: title-fill

Scaling Up A Simple Web App 101
===============================

(The Hand-Wavey Edition)

.. figure:: /_static/7533805968_b639d68a00_b.jpg
    :class: fill

    CC-BY-ND http://www.flickr.com/photos/65488604@N02/7533805968/

Where You Start
---------------

.. figure:: /_static/basic-setup.png
    :class: fill

Delegating Static Content Duties
--------------------------------

.. figure:: /_static/setup-with-cdn.png
    :class: fill

Adding A New Server
-------------------

.. figure:: /_static/setup-with-dbserver.png
    :class: fill

Let's Scale Horizontally!
-------------------------

.. figure:: /_static/setup-with-loadbalancer.png
    :class: fill

.. rst-class:: title-fill

More Tricks
===========

.. figure:: /_static/552152780_aa81e34d1a_b.jpg
    :class: fill

    CC-BY-NC http://www.flickr.com/photos/44124453791@N01/552152780/

More Reads Than Writes
----------------------

.. figure:: /_static/setup-with-multipledb.png
    :class: fill

Some Request Needs Long Processing Time?
----------------------------------------

* Use cases
    * Reports *(especially one that uses a lot of data)*
    * Blocking requests due to third-party services *(like email, notification)*
    * Media transcoding *(e.g. coverting video)*
* Add asychronous requests to your web app/API

Setting Up with Background Workers
----------------------------------

.. figure:: /_static/setup-with-mq.png
    :class: fill

What About NoSQL?
-----------------

* Using NoSQL database ≠ scalable solution
* **Right tool for the right job**
    * Document-oriented stores
    * Column-oriented stores
    * Graph databases
    * Key-value stores
* Fast at querying data that suits the domains of the NoSQL database

Congratulations! You're Now Smarter!
====================================

.. figure:: /_static/6966069023_5512204921_b.jpg
    :class: fill

    CC-BY http://www.flickr.com/photos/sylvainkalache/6966069023/

Today You've Learned
====================

* Scaling should not be your first priority, monitoring is
* When do you really need to scale
* How to scale a simple web app
* Additional weapons to make things speedier

Tweet Me Maybe
==============

:Email: felixleong@gmail.com
:Facebook: http://facebook.com/leongsh/
:Twitter: http://twitter.com/felixleong/

**Presentation**

http://github.com/felixleong/wckl_webscale_talk/

**License**

`Creative Commons Attribution-ShareAlike 3.0 Unported License`_.

.. _Creative Commons Attribution-ShareAlike 3.0 Unported License: http://creativecommons.org/licenses/by-sa/3.0/deed.en_US
