AirBnB Clone Project
The Project Description

In the AirBnB clone project, we began by developing the backend and integrating it with a console application using the cmd module in Python. The data, represented as Python objects, is saved in a JSON file and can be retrieved using the json module in Python.

The Descripton of the command interpreter

The AirBnB website's command line interface resembles the Bash shell, but it has a limited set of commands that are specifically designed for the AirBnB website's usage. This command line interpreter functions as the front-end of the web application, allowing users to interact with the back-end that was developed with Python OOP programming.

Some of the available commands include: 
show
create
update
destroy
count

The implementation of the command line interpreter, coupled with the back-end and file storage system, allows for the following actions to be permformed:
Creating new objects (ex: a new User or a new Place)
Retrieving an object from a file, a database etc…
Updating attributes of an object
Doing operations on objects (count, compute stats, etc…)
Destroying an object

How to start it:

The following steps will enable you to obtain a copy of the project and deploy it on your local machine (Linux distribution) for the purposes of development and testing.

Installation

To acquire the simple shell program and all of its dependencies, it will be necessary to clone the project's repository from Github.

git clone https://github.com/BibiObiora/AirBnB_clone.git

Once the repository has been cloned, a folder named "AirBnB_clone" will be created. Inside this folder, there are several files that are necessary for the program to function.

console.py: This is the main executable for the project and it serves as the command interpreter.
models/engine/file_storage.py: This class is responsible for serializing instances to a JSON file and deserializing JSON files to instances.
models/init.py: This contains a distinctive instance of FileStorage for the application.
models/base_model.py: This class defines all of the common attributes and methods that are shared by other classes.
models/user.py: This class, User, is derived from the BaseModel class.
models/state.py: This class, State, is derived from the BaseModel class.
models/city.py: This class, City, is derived from the BaseModel class.
models/amenity.py: This class, Amenity, is derived from the BaseModel class.
models/place.py: This class, Place, is derived from the BaseModel class.
models/review.py: This class, Review, is derived from the BaseModel class.

How to use it:

There are two different modes in which it can operate:

Interactive and Non-interactive.

During Interactive mode, a prompt (hbnb) will be displayed on the console, indicating that the user can input and execute commands. Once the command is executed, the prompt will reappear, waiting for a new command. This cycle will continue indefinitely, unless the user exits the program.


$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb) 
(hbnb) 
(hbnb) quit
$


Non-interactive mode requires the shell to be launched with a command input piped into its execution, so that the command can be executed immediately upon the Shell's initiation. In this mode, no prompt will be displayed and no additional input will be anticipated from the user.


$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$


Authors :
 Edidiong Obiora & Joshua Ryan Akakpo
