.. _model_view_controller_pattern:

*****************************
Model-View-Controller Pattern
*****************************

Separates the application (or part of it) into the parts model (data and logic), view (HMI) and controller (links the model and the view).

:Implementation example:
 Python - Web interface URL-shortening service implemented with the framework
 flask which does not support the MVC pattern out-of-the-box (Zlobin 2013, 
 section "1. Model-View-Controller", subchapter "Implementation in Python").

:Implemetation example:
 Python - The chess game objects chessboard and pieces (model) are linked to the
 graphical representation (view) over mouse events (controller) (Chaudhary 2013,
 section "Project 4: Game of Chess"). (The separation into model, view and
 controller is not that obvious because the view and the model are placed into a
 single python file "gui.py".)
