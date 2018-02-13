# Homebrew
| Useful Links   |                            |
|----------------|----------------------------|
| Website        | https://brew.sh/           |
| Formulae       | http://formulae.brew.sh/   |

## Overview

Homebrew is a package manager for macOS (formerly Mac OS). Homebrew allows you
to install programs easily from the command line. For example, to install Visual
Studio Code, all you need to do is: `brew cask install visual-studio-code`. Much
nicer than having to find a download link!

## Installing Homebrew

Open a Terminal and execute:

    /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

You may be asked for your administrator password, enter it when that prompt
appears.

You will also need to add `/usr/local/bin` to your `PATH`. See [these
instructions](https://stackoverflow.com/a/10343891/2319844) if you don't know
how to do this.

## Using Homebrew

To install a *formulae* (package):

    brew install <package_name>
where `<package_name>` is the name of the package you want to install.

If it is a UI application such as Visual Studio Code, you may need to use:

    brew cask install <package_name>
where `<package_name>` is the name of the package you want to install.
