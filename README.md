# emacs-visual-notifications

[![Marmalade](https://img.shields.io/badge/marmalade-available-8A2A8B.svg)](https://marmalade-repo.org/packages/emacs-visual-notifications)  
[![License](https://img.shields.io/badge/LICENSE-GPL%20v3.0-blue.svg)](https://www.gnu.org/licenses/gpl.html)
[![Gratipay](http://img.shields.io/gratipay/myTerminal.svg)](https://gratipay.com/myTerminal)

A utility to create visual notifications in emacs

## Installation

### Manual

Save the file *emacs-visual-notifications.el* to disk and add the directory containing it to `load-path` using a command in your *.emacs* file like:

    (add-to-list 'load-path "~/.emacs.d/")

The above line assumes that you've placed the file into the Emacs directory '.emacs.d'.

Start the package with:

    (require 'emacs-visual-notifications)

### Marmalade

If you have Marmalade added as a repository to your Emacs, you can just install *emacs-visual-notifications* with

    M-x package-install emacs-visual-notifications RET

## Usage

Currently, the following notifications are supported

1. flash once

    (emacs-visual-notification-flash-once 1)

The above code flashes the screen only once for *1* second

2. flash for a particular number of times

    (emacs-visual-notification-flash 3
        1
        2)

The above code flashes the screen *3* times, the flash lasts for *1* second and the gap between two flashes is *2* seconds

3. flash until user interaction **(coming soon)**

    (emacs-visual-notification-flash-until-active 1
        2)

The above code flashes the screen until the user performs any gesture. The flash lasts for *1* second and the gap between two flashes is *2* seconds.
