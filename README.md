CRDS Submission tool for INS scientists
=======================================

This site uses Django, a Python package for web development.  Django has a
bit of a learning curve, and some of the tutorials just dive in without
giving you the Big Picture of what the package is doing for you.  One of
the best explanations I've seen is in the Mozilla Django tutorial, especially
this section:
[What does Django look like?](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Introduction#What_does_Django_code_look_like).
Otherwise, I used tutorials by Corey Schafer, of which
[this](https://www.youtube.com/watch?v=UmljXZIypDc)
is the first.

To use the code, clone this repository and then, from the top-level directory
of the project (in which there should be a file named manage.py), type

% python manage.py runserver

This will start a sinple server that is used to serve up the Django page.

In your browser, enter the URL [http://127.0.0.1:8000/submit_reference_file/](http://127.0.0.1:8000/submit_reference_file/)

This gets handled by the file ins_submit/urls.py in the first line of
urlpatterns:

    path('submit_reference_file/', include('submit_reference_file.urls')),
