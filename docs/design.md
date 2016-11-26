# Abstract Factory

Creates families of related objects without depending on their specific classes.

:Implementaion example:
 App which lets the user decide weather connect to a website over http,
 https or ftp to list the directories of the corresponding web server (Zlobin
 2013, chapter "The Factory Method Implementation").

:Implementaion example:
 Creation of a game dependent on the user age for childs ("frog world")
 or adults ("wizard world"). (Kasampalis 2015, chapter "1. The Factory Pattern",
 subchapter "Abstract Method", subsubchapter "Implementation").

# Adapter

Makes two incompatible interfaces compatible.

:Implementation example:
 Abstract but running example of the Adapter Pattern implemented with
 the internal dictionary of a class instead of the traditional implementation
 based on inheritance (Kasampalis 2015, chapter "4. The Adapter pattern",
 subchapter "Implementation").

:Implementation example:
 Existing class does calculate a persons age dependent on the birthday
 date as string input. Adapter class uses the existing class but provides an
 interface which expects the birthday date in the datetime format (Phillips 2010,
 section "Adapter pattern" / p. 257).

# Builder

Composition of a complex object consisting of different parts step by step.

:Implementation example:
 The configuration of imaginary computers with different configurations
 points out the differences between the Builder Pattern and the Factory Pattern
 (Kasampalis 2015, chapter "2. The Builder Pattern", subchapter "Uses cases").

:Implementaion example:
 Preparing imaginary pizzas with different ingredients but whose
 preparation follow a common procedure (Kasampalis 2015, chapter "2. The Build
 Pattern", subchapter "Implementation").

# Container

Abstracts away data structuring from application domain classes.

:Implementation example:
 The standard library of Python 3 provides many built-in containers
 (dict, list, set, tuple) and specialized container datatypes (namedtuple, deque,
 ChainMap, Counter, OrderedDict, defaultDict, UserDict, UserList, UserString)
 in the module *collections*.

# Facade

:Implementaion example:
 Access layer to a SQLite database for blog and related post objects
 (Lott 2014, chapter "Designing an access layer for SQLite").

# Factory Method

Defines an interface for creating an instance of an object but lets the class
which implements the interface decide which class to instantiate.

:Implementaion example:
 App which lets the user decide weather connect to a website over http
 or ftp to list the directories of the corresponding web server (Zlobin 2013,
 chapter "The Factory Method Implementation").

:Implementaion example:
 Creation of objects for handling the input data in XML format or in
 JSON format and parsing it correspondingly. (Kasampalis 2015, chapter "1. The
 Factory Pattern", subchapter "Factory Method", subsubchapter "Implementation").

# Model View Controller

Separates the application (or part of it) into the parts model (data and logic),
view (HMI) and controller (links the model and the view).

:Implementation example:
 Web interface URL-shortening service implemented with the framework
 flask which does not support the MVC pattern out-of-the-box (Zlobin 2013, 
 section "1. Model-View-Controller", subchapter "Implementation in Python").

:Implemetation example:
 The chess game objects chessboard and pieces (model) are linked to the
 graphical representation (view) over mouse events (controller) (Chaudhary 2013,
 section "Project 4: Game of Chess"). (The separation into model, view and
 controller is not that obvious because the view and the model are placed into a
 single python file "gui.py".)

# Observer

Notification of clients about the status of a data server.

:Implementation example:
 The system time (subject) notifies its observers (12 hour formatter,
 24 hour formatter) about a change which convert and print the time accordingly
 (Zlobin 2013, chapter "Observer design pattern", subsection "Implementation in
 Python" / Kindle pos. 924).

:Implementation example:
 The value (subject) notifies its observers (hex formatter, binary
 formatter) about a change which convert an print the value accoringly
 (Kasampalis 2015, section "Chapter 13. The Observer Pattern", subsection
 "Implementation" / Kindle pos. 2416).

# Prototype

Creation of an exact copy of an object.

:Implementation example:
 Creation of information about the second version of a book based on
 the first version information by using pythons deepcopy functionality
 copy.deepcopy() (Kasampalis 2015, chapter "3. The Prototype Pattern").

# Singleton

Ensures that only one instance of a class may be created.

:Implementation example:
 __new__ class method ensures that only one instance of the class is
 created (using call "super") and returns the same single instance if "one is
 created" afterwards (Philipps 2010, section "Singleton implementation").

:Implementation example:
 A state based parser instantiates a class and assigns it immediatelly
 afterwards to a module variable (Phillips 2010, section "Module variables can
 mimic singletons").

:Implementation example:
 Basic "class" singleton (Zlobin 2013, section "A classic singleton").

:Implementation example:
 Webcrawler which scans for website-local hyperlinks, follows the links
 and downloads the pictures on it (Zlobin 2013, section "Chapter 2. Creating
 Only One Object with teh Singleton Pattern", subsection "Implementation in
 Python" / Kindle pos. 417)

## Implicitly Instantiated Module Singleton

Pythonic variant/implementation of the singleton where an object is instantiated
immediately (after module import).

:Implementation example:
 A state based parser instantiates a class and
 assigns it immediatelly afterwards to a module variable (Phillips 2010, section
 "Module variables can mimic singletons").

:Implementation example:
 Pythonic "modul instead of class" singleton
 (Zlobin 2013, section "A module-level singleton").

:Implementation example:
 Database object is instantiated as module local object (Phillips, p. 47).

## Explicitly Instantiated Module Singleton

Pythonic variant/implementation of the singleton where the object is instantiated
explicitly.

:Problem:
 - in Python objects are created immediatelly after modules are imported
 - if performance is critical or the object data not available yet a delayed
   instantiation may be required

:Implementation example:
 Database object may be instantiated as module local object per
 function call (Phillips, p. 47). (Phillips, p. 48).

## Borg singleton

Uses a shared state to ensure that successors of a singleton class are also
singletons.

:Implementation example:
 Borg singleton implements a shared resource (to store images) and a
 set of URLs  which are accessed by 2 threads which fetch images of the URLs and
 stores them (Zlobin 2013, chapter "2. Creating Only One Object with the
 Singleton Pattern", subchapter "Implementation in Python").

# State

:Implementation example:
 Emulation of basic operation system process states and transitions
 using the module "state_machine" (Kasampalis 2015, chapter "Chapter 14. The
 State Pattern", subchapter "Implementation").
