# TurboGears
| Useful Links      |                                                                            |
|-------------------|----------------------------------------------------------------------------|
| Website           | http://turbogears.org/                                                     |
| Documentation     | https://turbogears.readthedocs.io/en/latest/turbogears/minimal/index.html# |

## Overview

TurboGears is a flexible web framework written in Python. TurboGears takes
advantage of many well-known, reliable libraries such as SQLAlchemy, Kajiki, and
Bootstrap.

## Getting Started on an Existing TurboGears Project

1. TurboGears projects are Python projects. You will need to [install Python
   3](./Python3.md#installing-python-3) if you haven't already.

2. Now, clone the repository using [Git](./Git.md).

3. Now, you need to install the application and its dependencies. If you do not
   want to install all of the packages in `~/.local`, you can use a [Python
   Virtual environment](./Python-Virtual-Environment.md). If you choose to do
   so, remove `--user` from the following commands.

   Note, make sure you are using the proper version of pip. You need to use
   pip version 3 or greater.

   1. Install the application and its dependencies:

          $ pip install -e . --user

   2. If you do not have `gearbox` installed:

          $ pip install --user tg.devtools

   3. Setup the application:

          $ cp development.ini.sample development.ini
          $ gearbox setup-app

   4. Now you can serve the application:

          $ gearbox serve --reload --debug

   5. To view the application, go to your web browser and navigate to
      `localhost:8080` to view the website.
