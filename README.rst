*******************************
Sublime Text Sphinx Completions
*******************************

This is a collection of Sublime Text completions for reStructuredText_ interpreted text roles defined by the Sphinx_ documentation tool for `inline semantic markup`_.
These completions are active in the ``text.restructuredtext`` scope.

.. _reStructuredText: http://docutils.sf.net/rst.html
.. _Sphinx: http://sphinx-doc.org/
.. _inline semantic markup: http://sphinx-doc.org/markup/inline.html

Not all Sphinx_ roles are included yet;
I'm just adding them as I have need for them.
Pull requests that add your favourites are more than welcome!


Installation
============

Clone the repository into your `packages folder`_::

  git clone git@github.com:douglatornell/sublime-sphinx-completion


.. _packages folder: http://sublimetext.info/docs/en/basic_concepts.html#the-packages-directory


Use
===

Type the name of the role and hit ``tab``.
The role name will be replaced by ``:role_name:```` and the insertion point will be left between the backticks for you to type the text that you want the role to apply to.
Example:

  ``file<tab>`` completes to ``:file:````

Hit tab again to jump past the closing backtip.

You can just use the frist few letters of a role name;
e.g. ``program`` and ``prog`` both complete to ``:program:````.

**Note:** For obvious (I think) reasons, ``tab`` inside a completion inserts a literal ``tab`` rather than activating another level of completion.
If you want to do a completion within a completion use ``Edit > Show Completions`` from the menu
(or the appropriate keyboard shortcut;
e.g. ``^Space`` on OS/X).


Customization
=============

You can put completions for your own custom roles in ``Packages/User/Sphinx.sublime-completions`` and they will be merged with the completions supplied by this package.


TODO
====

* Add a way of using Sphinx_ roles in Python docs strings


Author
======

Doug Latornell (douglatornell_)

.. _douglatornell: https://github.com/douglatornell


License
=======

This is just a few lines of editor configuration!
It's in the public domain.
If you insist on getting all legal about things,
go look at the ``UNLICENSE`` file.
