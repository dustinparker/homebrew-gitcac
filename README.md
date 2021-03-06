Mac OS X gitcac tap
===================

Quickstart
----------

    [ -e /usr/local/bin/brew ] || ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
    brew tap dustinparker/gitcac
    brew install gitcac
    exec bash -l

The installer will prompt you for your password a couple of times to run
privileged actions. This is necessary to install CACKey and alter the system
$PATH.

Caveats
-------

`curl` and `git` from homebrew might conflict. If you run into problems, try removing them first:

    brew rm curl
    brew rm git

Updates
-------

To receive updates to gitcac, use:

    brew update
    brew upgrade

If you only want to update gitcac and nothing else:

    brew upgrade /usr/local/Library/Taps/dustinparker/gitcac/*.rb

or

    brew upgrade cackey gitcac{-curl,-git,}