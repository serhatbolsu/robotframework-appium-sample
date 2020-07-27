Appium Testing Sample with Robot Framework and AppiumLibrary
============================================================

.. contents::

Overview
--------
In this sample framework, you will find test cases for iOS and Android.
Test cases are written for sample applications under `demoapp`_ folder.

- Test suite for iOS and Android Locators
- Test suite for iOS and Android  Mobile Web Testing
- Test suite for iOS and Android  Basic Interactions
- Test suite for iOS and Android  Selectors

Generated results
-----------------
After `running tests`_ you will get report and log in HTML format. Example
files are also visible online in case you are not interested in running
the demo yourself:

- `report.html`_
- `log.html`_

Running Sample
==============
Preconditions
-------------

Install `Robot Framework`_ and `AppiumLibrary`_

The simplest way is using `pip`_ package manager::

  pip install -r requirements.txt


Device Setup
------------
After installing the library, you still need to setup an simulator/emulator or real device to use in tests.
iOS and Android have separate paths to follow, and those steps better explained in `Appium Driver Setup Guide`_.
Please follow the **Driver-Specific Setup** according to platform.


Running tests
-------------

Test cases are located in the ``tests`` folder. They can be
executed using the ``robot`` command::

    robot  tests/*.test.robot

You can also run an iOS or Android case file/test::

    robot tests/android_basic_interactions.test.robot
    robot --test "Should find elements by ID" tests


TODO
----
There are much more to improve, here is the list of things to come

- Circle.ci build pipeline
- SauceLabs Execution Support
- More coverage from library methods


.. _Robot Framework: http://robotframework.org
.. _Robot Framework User Guide: http://robotframework.org/robotframework/#user-guide
.. _Appium Driver Setup Guide: http://appium.io/docs/en/about-appium/getting-started/?lang=en
.. _AppiumLibrary: https://github.com/serhatbolsu/robotframework-appiumlibrary
.. _pip: http://pip-installer.org
.. _download: https://github.com/serhatbolsu/robotframework-appium-sample/archive/master.zip
.. _source code: https://github.com/robotframework/WebDemo.git
.. _demoapp: https://github.com/serhatbolsu/robotframework-appium-sample/demoapp
.. _report.html: https://github.com/serhatbolsu/robotframework-appium-sample/report.html
.. _log.html: https://github.com/serhatbolsu/robotframework-appium-sample/log.html
