# Flycheck bashate Checker

[![License GPL 3](https://img.shields.io/badge/license-GPL_3-green.svg)](http://www.gnu.org/licenses/gpl-3.0.txt)
[![MELPA](http://melpa.org/packages/flycheck-bashate-badge.svg)](http://melpa.org/#/flycheck-bashate)
[![Build Status](https://travis-ci.org/alexmurray/flycheck-bashate.svg?branch=master)](https://travis-ci.org/alexmurray/flycheck-bashate)

Integrate [bashate](https://github.com/alexmurray/bashate) with
[flycheck](http://www.flycheck.org) to automatically check the
style of your bash scripts on the fly.

## Installation

### MELPA

The preferred way to install `flycheck-bashate` is via
[MELPA](http://melpa.org) - then you can just <kbd>M-x package-install RET
flycheck-bashate RET</kbd>

To enable then simply add the following to your init file:

```emacs-lisp
(eval-after-load 'flycheck
  '(progn
     (require 'flycheck-bashate)
     (flycheck-bashate-setup)))
```

### Manual

If you would like to install the package manually, download or clone it and
place within Emacs' `load-path`, then you can require it in your init file like
this:

```emacs-lisp
(require 'flycheck-bashate)
(flycheck-bashate-setup)
```

NOTE: This will also require the manual installation of `flycheck` if you have
not done so already.

## License

Copyright © 2016 Alex Murray

Distributed under GNU GPL, version 3.
