# AirBnB Project Overview

## Project Description

This project is the initial phase of building a comprehensive web application, specifically an AirBnB clone. It lays the foundation for future projects involving HTML/CSS templating, database storage, API integration, and front-end development. The goals of this project include:

- Implementing a parent class (`BaseModel`) to handle initialization, serialization, and deserialization of instances.
- Establishing a straightforward serialization/deserialization process: Instance <-> Dictionary <-> JSON string <-> File.
- Developing essential classes for AirBnB (e.g., `User`, `State`, `City`, `Place`) that inherit from `BaseModel`.
- Creating the first abstracted storage engine: File storage.
- Writing unittests to validate all classes and the storage engine.

## Command Interpreter Description

The command interpreter functions like a shell but is tailored for managing the objects of this project. It supports the following functionalities:

- Creating new objects (e.g., a new `User` or `Place`).
- Retrieving objects from a file or database.
- Performing operations on objects (e.g., count, compute stats).
- Updating object attributes.
- Deleting objects.

### Usage Instructions with Examples

**Interactive Mode:**
To start the shell in interactive mode:
```sh
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb)
(hbnb) quit
$
```

**Non-Interactive Mode:**
The shell can also operate in non-interactive mode:
```sh
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
```

**Running Tests:**
To ensure all tests pass in non-interactive mode:
```sh
$ echo "python3 -m unittest discover tests" | bash
```
