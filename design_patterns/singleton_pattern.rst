.. _singleton_pattern:

*****************
Singleton Pattern
*****************

Ensures that only one instance of a class may be created.

:Implementation example:
 Python - __new__ class method ensures that only one instance of the class is
 created (using call "super") and returns the same single instance if "one is
 created" afterwards (Philipps 2010, section "Singleton implementation").

:Implementation example:
 Python - A state based parser instantiates a class and assigns it immediatelly
 afterwards to a module variable (Phillips 2010, section "Module variables can
 mimic singletons").

:Implementation example:
 Python - Basic "class" singleton (Zlobin 2013, section "A classic singleton").

:Implementation example:
 Python - Webcrawler which scans for website-local hyperlinks, follows the links
 and downloads the pictures on it (Zlobin 2013, section "Chapter 2. Creating
 Only One Object with teh Singleton Pattern", subsection "Implementation in
 Python" / Kindle pos. 417)

Python Implicitly Instantiated Module Singleton
-----------------------------------------------

Pythonic variant/implementation of the singleton where an object is instantiated
immediately (after module import).

:Implementation example:
 Python - A state based parser instantiates a class and
 assigns it immediatelly afterwards to a module variable (Phillips 2010, section
 "Module variables can mimic singletons").

:Implementation example:
 Python - Pythonic "modul instead of class" singleton
 (Zlobin 2013, section "A module-level singleton").

:Implementation example:
 Python - Database object is instantiated as module local object (Phillips, p. 47).

Python Explicitly Instantiated Module Singleton
-----------------------------------------------

Pythonic variant/implementation of the singleton where the object is instantiated
explicitly.

:Problem:
 - in Python objects are created immediatelly after modules are imported
 - if performance is critical or the object data not available yet a delayed
   instantiation may be required

:Implementation example:
 Python - Database object may be instantiated as module local object per
 function call (Phillips, p. 47). (Phillips, p. 48).

Borg singleton
--------------

Uses a shared state to ensure that successors of a singleton class are also
singletons.

:Implementation example:
 Python - Borg singleton implements a shared resource (to store images) and a
 set of URLs  which are accessed by 2 threads which fetch images of the URLs and
 stores them (Zlobin 2013, chapter "2. Creating Only One Object with the
 Singleton Pattern", subchapter "Implementation in Python")
