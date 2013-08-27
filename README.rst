Scaling Your Web App – The Basics - Webcamp KL, August 2013
===========================================================

Generating the presentation slides
----------------------------------

1. Create a virtualenv instance.

   .. note::

        All commands below are prepended with an expected bash prompt.
        
        * "$" indicates a normal bash prompt, virtualenv is not activated
        * "(.env)$" indicates a bash prompt with virtualenv activated

   .. code-block:: bash

        $ virtualenv .env
        $ source .env/bin/activate
        (.env)$

2. Install the required packages.

   .. code-block:: bash

        (.env)$ pip install -r requirements.txt


3. Edit source/index.rst, it's a `ReStructured Text`_ document.

4. Once you make the edits, you can generate the new slide show with the
   following command.

   .. code-block:: bash

        (.env)$ make slides

.. _ReStructured Text: http://docutils.sourceforge.net/rst.html
