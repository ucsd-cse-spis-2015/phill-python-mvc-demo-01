# phill-python-mvc-demo-01
A demo of the basic ideas behind MVC separation 

We see a file myConversions.py that contains a simple ftoc function.   This is our "model", something that does some basic computation.

Then we have various ways of getting the input into that function, and getting the output out.

The computation is all in one place.    And the computation is SEPARATE from how we get the input, and how we provide the output.    This is the principle of "separation of concerns".

We see:

* a console app that prompts for input and prints output
* a script intended to be used at the command prompt that takes input as a command line parameter
* a GUI converter that runs in a frame on our desktop
* a webapp that takes input as part of the URL and prints the answer to the console
* a webapp that takes input in an HTML form and provides a response as an HTML form.

In an MVC application, you try to separate the:
* model: code that does pure computation (it may also read from a database, or writes to a database)
* view: code that prompts for input and formats output&mdash;the user's view of the application
* controller: some "glue" that helps the model and view communicate.

In large MVC applications, Model, View and Controller code may end up in different directories, or at the very least, in different files.  Here, we are typically seeing view and controller all mashed into one.

This is GPL because it uses some GPL software&mdash;namely, the file breezypythongui.py comes from the website: http://home.wlu.edu/~lambertk/breezypythongui

