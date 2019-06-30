`bang.el`
=========

`bang` is a `shell-command` substitute that makes it easier to run
commands on regions or whole buffers. This is done by potentially
interpreting the first character differently, as the `bang` docstring
explains:

	When COMMAND starts with
	  <  the output of COMMAND replaces the current selection
	  >  COMMAND is run with the current selection as input
	  |  the current selection is filtered through COMMAND
	  !  executes the last command that started with COMMAND,
		 or if a number, re-execute nth last command

Bang has been based on a function of the same name by [Leah
Neukirchen][leah].

How to use
----------

Using [MELPA] and `use-package`, a minimal setup might look something like
this:

	(use-package bang
	  :bind ("M-!" . bang))

Copying
-------

`bang.el` is distributed under the [CC0 1.0 Universal (CC0 1.0) Public
Domain Dedication][cc0] license.

[leah]: http://leahneukirchen.org/dotfiles/.emacs
[MELPA]: https://melpa.org/#/bang
[cc0]: https://creativecommons.org/publicdomain/zero/1.0/deed
