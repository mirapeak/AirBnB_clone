# 0x00. AirBnB clone - The Console
<a href="URL_REDIRECT" target="blank"><img align="center" src="https://camo.githubusercontent.com/d8a348e1fceb92d45fa8981ac42a6223e454acefe89750896e80fd1287cab92b/68747470733a2f2f7777772e706e676974656d2e636f6d2f70696d67732f6d2f3133322d313332323132355f7472616e73706172656e742d6261636b67726f756e642d616972626e622d6c6f676f2d68642d706e672d646f776e6c6f61642e706e67" height="100" /></a>
## Description of the Project
This is the first part of the AirBnB clone project where we worked on the backend of the project whiles interfacing it with a console application with the help of the cmd module in python.

Data (python objects) generated are stored in a json file and can be accessed with the help of the json module in python
## Description of the Command Interpreter
The interface of the application is just like the Bash shell except that this has a limited number of accepted commands that were solely defined for the purposes of the usage of the AirBnB website.

This command line interpreter serves as the frontend of the web app where users can interact with the backend which was developed with python OOP programming.

Some of the commands available are:
* show
* create
* update
* destroy
* count

And as part of the implementation of the command line interpreter coupled with the backend and file storage system, the folowing actions can be performed:
* Creating new objects (ex: a new User or a new Place)
* Retrieving an object from a file, a database etc…
* Doing operations on objects (count, compute stats, etc…)
* Updating attributes of an object
* Destroying an object

### How to start it
These instructions will get you a copy of the project up and running on your local machine (Linux distro) for development and testing purposes.

#### Installing
You will need to clone the repository of the project from Github. This will contain the simple shell program and all of its dependencies.

https://github.com/mirapeak/AirBnB_clone.git

After cloning the repository you will have a folder called AirBnB_clone. In here there will be several files that allow the program to work.

'''
> /console.py : The main executable of the project, the command interpreter.

> models/engine/file_storage.py: Class that serializes instances to a JSON file and deserializes JSON file to instances

> models/__ init __.py: A unique FileStorage instance for the application

> models/base_model.py: Class that defines all common attributes/methods for other classes.

> models/user.py: User class that inherits from BaseModel

> models/state.py: State class that inherits from BaseModel

> models/city.py: City class that inherits from BaseModel

> models/amenity.py: Amenity class that inherits from BaseModel

> models/place.py: Place class that inherits from BaseModel

> models/review.py: Review class that inherits from BaseModel 
'''

### How to use it
It can work in two different modes:

**Interactive** and **Non-interactive**.

In **Interactive mode**, the console will display a prompt (hbnb) indicating that the user can write and execute a command. After the command is run, the prompt will appear again a wait for a new command. This can go indefinitely as long as the user does not exit the program.

In **Non-interactive mode**, the shell will need to be run with a command input piped into its execution so that the command is run as soon as the Shell starts. In this mode no prompt will appear, and no further input will be expected from the user.

## Format of Command Input
In order to give commands to the console, these will need to be piped through an echo in case of **Non-interactive mode**.

In **Interactive Mode** the commands will need to be written with a keyboard when the prompt appears and will be recognized when an enter key is pressed (new line). As soon as this happens, the console will attempt to execute the command through several means or will show an error message if the command didn't run successfully. In this mode, the console can be exited using the **CTRL + D** combination, **CTRL + C**, or the command **quit** or **EOF**.

## Arguments
Most commands have several options or arguments that can be used when executing the program. In order for the Shell to recognize those parameters, the user must separate everything with spaces.

Example:

## Authors:
* **Miracle Livinus**
* **John Josephine**
