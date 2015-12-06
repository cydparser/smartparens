# Smartparens
[![MELPA](http://melpa.org/packages/smartparens-badge.svg)](http://melpa.org/#/smartparens)
[![MELPA Stable](http://stable.melpa.org/packages/smartparens-badge.svg)](http://stable.melpa.org/#/smartparens)
[![Build Status](https://travis-ci.org/Fuco1/smartparens.png?branch=master)](https://travis-ci.org/Fuco1/smartparens)
[![Gratipay](http://img.shields.io/gratipay/Fuco1.svg)](https://www.gratipay.com/Fuco1/)
[![Paypal logo](https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CEYP5YVHDRX8C)

Smartparens is minor mode for Emacs that *deals with parens pairs and tries to be smart about it*. It started as a unification effort to combine functionality of several existing packages in a single, compatible and extensible way to deal with parentheses, delimiters, tags and the like. Some of these packages include [autopair](https://github.com/capitaomorte/autopair), [textmate](http://code.google.com/p/emacs-textmate/), [wrap-region](https://github.com/rejeep/wrap-region), [electric-pair-mode](http://www.emacswiki.org/emacs/ElectricPair), [paredit](http://emacswiki.org/emacs/ParEdit) and others. With the basic features found in other packages it also brings many improvements as well as completely new features. [Here's][wiki-what] a highlight of some features, for a complete list and detailed documentation look in the [manual][wiki-new].

[Rommel Martinez](https://github.com/ebzzry) wrote a [shortish introduction](https://ebzzry.github.io/emacs-pairs.html) with worked examples, for the complete documentation visit the [documentation wiki][wiki].

[wiki]: https://github.com/Fuco1/smartparens/wiki
[wiki-what]: https://github.com/Fuco1/smartparens/wiki#wiki-what-is-this-package-about?
[wiki-new]: https://github.com/Fuco1/smartparens/wiki#wiki-information-for-new-users

# Default configuration

Smartparens provides many options to customize most aspects of its working.  After loading `smartparens.el`, you can customize many of these options using the customization interface: `M-x customize-group RET smartparens RET`.  Smartparens also ships with additional recommended (default) configuration, which is separated in file `smartparens-config.el` to make the maintenance easier.  If you wish to load the default configuration, add:

```scheme
(require 'smartparens-config)
```

in your configuration files (e.g. init.el) to load it.  There are also files with additional configuration for specific modes, such as `smartparens-latex.el` or `smartparens-ruby.el`.  You can load them the same way as the default config file.  Note however that the `smartparens-config.el` file will auto-load all the mode-specific customizations.  It is a good idea to require this file if you are a new user, and later add or remove the options you don't like.

*Note: `smartparens-config` automatically loads the core smartparens files, so you don't have to require those separately.*

# Testing

Smarparens uses [ert-runner](https://github.com/rejeep/ert-runner.el)
for testing. To run all the tests, run:

```
$ make test
```

Alternatively, you can open the individual files in Emacs, then
`M-x eval-buffer` `M-x ert`.

There are also some ecukes tests, but these are deprecated.

# Support the project

If you want to support this project, you can do it in the following ways:

* Contribute code. If you have an idea that is not yet implemented and will benefit this project, feel free to implement it and submit a pull request. If you have any concerns whether your contribution will be accepted, ask beforehand. You can email the author or [start an issue](https://github.com/Fuco1/smartparens/issues/new) on the tracker.
* Contribute ideas. Even if you can't code Emacs Lisp, you can still contribute valuable ideas for other programmers to implement. Simply [start new issue](https://github.com/Fuco1/smartparens/issues/new) on the tracker and submit your suggestion.
* You can make a [financial donation](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CEYP5YVHDRX8C) through PayPal.  If you like smartparens and can spare a modest amount on a donation, feel free to do so.  These donations are expressions of your gratitude and are used for my personal "rewards" (books, games, music etc.).  You can also gift me a game on [Steam](http://steamcommunity.com/profiles/76561198265034071/wishlist) or buy something on [Amazon](http://www.amazon.com/gp/registry/wishlist/2I8DOQH8OZEUR).  Regardless of the donations, smartparens will always be free both as in beer and as in speech.
