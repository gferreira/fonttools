Other Tools
===========

Commands for inspecting, merging and subsetting fonts are also available:

.. code:: sh

    pyftinspect
    pyftmerge
    pyftsubset

fontTools Python Module
~~~~~~~~~~~~~~~~~~~~~~~

The fontTools python module provides a convenient way to programmatically edit font files.

.. code:: py

    >>> from fontTools.ttLib import TTFont
    >>> font = TTFont('/path/to/font.ttf')
    >>> font
    <fontTools.ttLib.TTFont object at 0x10c34ed50>
    >>>

A selection of sample python programs is in the `Snippets <https://github.com/fonttools/fonttools/blob/master/Snippets/>`__ directory.
