Optional Requirements
=====================

The ``fontTools`` package currently has no (required) external dependencies besides the modules included in the Python Standard Library.

However, a few extra dependencies are required by some of its modules, which are needed to unlock optional features.

``ttLib/woff2.py``
--------------------------------

Module to compress/decompress WOFF 2.0 web fonts; it requires:

-  `brotli <https://pypi.python.org/pypi/Brotli>`__: Python bindings of
   the Brotli compression library.

``ttLib/sfnt.py``
-------------------------------

To better compress WOFF 1.0 web fonts, the following module can be used instead of the built-in ``zlib`` library:

-  `zopfli <https://pypi.python.org/pypi/zopfli>`__: Python bindings of
   the Zopfli compression library.

``unicode.py``
----------------------------

To display the Unicode character names when dumping the ``cmap`` table with ``ttx`` we use the ``unicodedata`` module in the Standard Library. The version included in there varies between different Python versions. To use the latest available data, you can install:

-  `unicodedata2 <https://pypi.python.org/pypi/unicodedata2>`__: ``unicodedata`` backport for Python 2.7 and 3.5 updated to the latest Unicode version 9.0. Note this is not necessary if you use Python 3.6 as the latter already comes with an up-to-date ``unicodedata``.

``varLib/interpolatable.py``
------------------------------------------

Module for finding wrong contour/component order between different masters. It requires one of the following packages in order to solve the so-called "minimum weight perfect matching problem in bipartite graphs", or the Assignment problem:

*  `scipy <https://pypi.python.org/pypi/scipy>`__: the Scientific Library for Python, which internally uses `NumPy <https://pypi.python.org/pypi/numpy>`__ arrays and hence is very fast;
*  `munkres <https://pypi.python.org/pypi/munkres>`__: a pure-Python module that implements the Hungarian or Kuhn-Munkres algorithm.

``misc/symfont.py``
---------------------------------

Advanced module for symbolic font statistics analysis; it requires:

*  `sympy <https://pypi.python.org/pypi/sympy>`__: the Python library for symbolic mathematics.

``t1Lib.py``
--------------------------

To get the file creator and type of Macintosh PostScript Type 1 fonts on Python 3 you need to install the following module, as the old ``MacOS`` module is no longer included in Mac Python:

*  `xattr <https://pypi.python.org/pypi/xattr>`__: Python wrapper for extended filesystem attributes (macOS platform only).

``pens/cocoaPen.py``
----------------------------------

Pen for drawing glyphs with Cocoa ``NSBezierPath``, requires:

*  `PyObjC <https://pypi.python.org/pypi/pyobjc>`__: the bridge between Python and the Objective-C runtime (macOS platform only).

``pens/qtPen.py``
-------------------------------

Pen for drawing glyphs with Qt's ``QPainterPath``, requires:

*  `PyQt5 <https://pypi.python.org/pypi/PyQt5>`__: Python bindings for the Qt cross platform UI and application toolkit.

``pens/reportLabPen.py``
--------------------------------------

Pen to drawing glyphs as PNG images, requires:

*  `reportlab <https://pypi.python.org/pypi/reportlab>`__: Python toolkit for generating PDFs and graphics.

``inspect.py``
----------------------------

A GUI font inspector, requires one of the following packages:

*  `PyGTK <https://pypi.python.org/pypi/PyGTK>`__: Python bindings for GTK 2.x (only works with Python 2).
*  `PyGObject <https://wiki.gnome.org/action/show/Projects/PyGObject>`__ : Python bindings for GTK 3.x and gobject-introspection libraries (also compatible with Python 3).
