# Phase 3 Project: CLI and ORM

## Learning Goals

- Configure environments with project-specific parameters using Pipenv.
- Import and use external libraries.
- Define a Python object model that includes a one-to-many relationship between
  classes.
- Implement a set of **Object-Relational Mapping** functions to persist
  instances of a Python class to a relational database.
- Implement a **Command Line Interface** application.
- Use `list`s, `dict`s, and `tuple`s in appropriate contexts.
- Exercise best practices in CLI design.

---

## Key Vocab

- **Command Line**: a text-based interface that is built into your computer's
  operating system. It allows you to access the files and applications on your
  computer manually or through scripts.
- **Terminal**: the application in Mac OS that allows you to access the command
  line.
- **Command Shell/Powershell**: the applications in Windows that allow you to
  access the command line.
- **Command-Line Interface (CLI)**: a text-based interface used to run programs,
  manage files and interact with objects in memory. As the name suggests, it is
  run from the command line.
- **Object-Relational Mapping (ORM)**: a programming technique that provides a
  mapping between an object-oriented data model and a relational database model.
- **Attribute**: variables that belong to an object.
- **Property**: attributes that are controlled by methods.
- **Decorator**: function that takes another function as an argument and returns
  a new function with added functionality.

---

## Instructions

Welcome to the end of Phase 3! You've learned about a lot in this unit:

- Python fundamentals.
- Data structures (and more recently, algorithms).
- Object-oriented programming.
- Object inheritance.
- Class attributes and methods.
- Configuring applications.
- SQL fundamentals.
- Table relations in SQL.
- Object-relational mapping with Python.
- Building CLIs.

In this project, we're going to use these skills to create a CLI and ORM
application. We want you to display knowledge of as much from Phase 3 as you
can- you won't be able to fit everything in, but we'll expect to see:

- A database created and modified with Python ORM methods that you will write.
  - The data model includes **at least 2** model classes.
  - The data model includes **at least 1** one-to-many relationships.
  - ORM methods are implemented for each class in the data model.
- A CLI application that solves a real-world problem and adheres to best
  practices.

  - Display menus with which a user may interact.
  - Create loops as needed to keep the user in the application until they choose
    to exit.
  - For each class in the data model, the CLI includes options to create,
    update, delete, get all, and find by id.
  - Validate user input.

- Proper separation of concerns - (ex: models do not contain print statements)
- A well-maintained virtual environment using Pipenv.
- Proper package structure in your application.
- Use Python data structures in appropriate context

You do **not** need to implement tests for `pytest`, although you should test
your code thoroughly using your CLI. Try entering bad data when prompted for
input, and confirm your application prints a useful error message.

## How to begin?

- Think about your data model.
- Think about the user interaction. How will you prompt the user? What
  information will the user enter? How will you provide feedback to the user?
- Use the project template (provided in a separate lesson) to organize your
  Python classes.
- If you get stuck trying to accomplish a specific task, check online to see if
  there's a Python library that will make it easier.
- Consider using [Click][click] or [Fire][fire] to take care of basic CLI tasks
  for you.

---

## Resources

- [Click documentation][click]
- [The Python Fire Guide][fire]

[click]: https://click.palletsprojects.com/en/8.1.x/
[fire]: https://google.github.io/python-fire/guide/
