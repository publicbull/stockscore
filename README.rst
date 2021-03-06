Stock Score
===========
.. image:: https://img.shields.io/badge/python-v3-green.svg
   :target: https://www.python.org

.. image:: https://www.codefactor.io/repository/github/jackmoody11/stockscore/badge
   :target: https://www.codefactor.io/repository/github/jackmoody11/stockscore

.. image:: https://api.codacy.com/project/badge/Grade/d2108117522f4fe498530c6f7185108e
   :target: https://www.codacy.com/project/jacklaytonmoody/stockscore/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=jackmoody11/stockScores&amp;utm_campaign=Badge_Grade_Dashboard

.. image:: https://travis-ci.com/jackmoody11/stockscore.svg?branch=master
    :target: https://travis-ci.com/jackmoody11/stockscore

.. image:: https://img.shields.io/github/license/mashape/apistatus.svg?style=popout
   :target: https://github.com/jackmoody11/stockscore/blob/master/LICENSE

Stock Score is a python script to score stocks based on specified
criteria. The goal of this project is to provide a stock screening
system for various types of stock classifications (growth, momentum, value, etc.).

Similar to how one might rank the best options when they are deciding
where to go to dinner, Stock Score lets investors choose what screens
they want to run. Then, this script takes care of the rest,
showing which stocks performed best under the given screens.

Prerequisites
~~~~~~~~~~~~~

- You can get the latest version of Python 3 here_ (this should come with the latest version of pip)
- All dependencies are contained in `requirements.txt` (more on that directly below)

Getting Started
~~~~~~~~~~~~~~~

To clone this repository, run the following:

::

    git clone https://github.com/jackmoody11/stockscore

It's nice to have virtualenv installed

::

   pip install virtualenv

Change working directory to project folder

::

    cd my/path/to/stockscore

Create a virtual environment
For Mac users:
::

    python3 -m virtualenv env 

For Windows users:
::
    
    py -m virtualenv env # for Windows users


Make a virtual environment with :code:`python3 -m venv my-env`.
Then, in order to activate the virtual environment run the following:

For Mac users:

::

    source my-env/bin/activate

For Windows users:

::

    .\my-env\Scripts\activate

Then use :code:`pip install -r requirements.txt` to install required modules.

Run the program!
----------------
To make sure that everything is working, while in the working directory of the stockScore project, run :code:`python3 stock_score.py`.

*Note*: Make sure you are using :code:`python3`, because older versions of python do not support f strings.

Here is an example output of what you can expect to see when you run the program:

Terminal output:

.. image:: /media/terminal_output.png


Top 5 stocks output:

.. image:: /media/top5_output.png


Running the tests
-----------------

All tests can be run by simply running
::

    pytest

from the command line.


In order to run a specific test (like test_fundamental_functions.py), run
::

    pytest tests/test_fundamental_functions.py


For more information on how to use pytest (like how to select a few tests),
`look here`_ for the official pytest docs.

Deployment
----------

In order to make code styling simple, this project uses black_. To make sure your pull request follows the format, run :code:`black stockscore` while working in the main :code:`stockscore` directory.

This project is very simple to deploy to a live system. To change which tests you are using, change which functions are added to the suites (this is the name used in both files) of :code:`fundamental_functions.py` and :code:`technical_functions.py`.

Built With
----------

Python 3 and some great third party modules (see `requirements.txt`_ for more details).

Contributing
------------

Please read the `code of conduct`_ for details on how to positively contribute to this project.

Versioning
----------

This project uses `SemVer`_ for versioning. For the versions available, see the
`tags on this repository`_.


License
-------

This project is licensed under the MIT License - see the `LICENSE`_
file for details

Acknowledgments
---------------

-  Hat tip to Benjamin Graham's *Intelligent Investor*. If you haven't already, read this book!
-  Also, I recommend reading *Common Stocks and Uncommon Profits* by Philip Fisher.

Notes
-----

- *Note that the screens included in this project are not exclusive and do not guarantee any sort of returns. I assume no liability for investment decisions you make and am not a professional adviser. Please do your due diligence before making investment decisions and consult with a professional as necessary.*



.. _here: https://docs.python.org/3/installing/
.. _look here: https://pytestguide.readthedocs.io/en/latest/
.. _Dropwizard: http://www.dropwizard.io/1.0.2/docs/
.. _Maven: https://maven.apache.org/
.. _ROME: https://rometools.github.io/rome/
.. _black: https://github.com/ambv/black
.. _`requirements.txt`: https://github.com/jackmoody11/stockScores/blob/master/requirements.txt
.. _`code of conduct`: CODE_OF_CONDUCT.md
.. _SemVer: http://semver.org/
.. _tags on this repository: https://github.com/jackmoody11/stockScores/tags
.. _LICENSE: https://github.com/jackmoody11/stockScores/blob/master/LICENSE
