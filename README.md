Cython Sandbox
==================================================================================

Study / solve the following issues:

  - make basic distutils-based build/install `setup.py` file for a Cython
    package. See <https://github.com/cython/cython/wiki/PackageHierarchy>

  - Package may be necessary even for "flat" modules to have the access
    to package data. And package data is interesting for example to
    distribute reliably `pxd` files. Have a look at how this stuff
    should be done.

  - package stuff: on Linux the behavior differs when there is a package
    with a `__init__.pyx` file with Python 2 and 3: I'd like say to a
    class in this package to appear as `PACKAGE.C`, 
    not `PACKAGE.__init__.C` but so far it doesn't work reliably.

  - issues with Windows and Python 3: `__init__` stuff (link issue)
    when packages are used. Difference of behavior with 32 and 64 build
    bugs

  - Use Travis and AppVeyor to make sure 
    that this stuff builds and works as expected.
    See <https://packaging.python.org/guides/supporting-windows-using-appveyor/>
