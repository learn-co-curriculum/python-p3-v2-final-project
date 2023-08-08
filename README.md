# Phase 3 Project: CLI and ORM

## Learning Goals

- Implement a Python application that includes a **Command Line Interface**.
- Implement a set of **Object-Relational Mapping** functions for two or more
  model classes.
- Define a Python object model that includes a one-to-many relationship between
  two classes.
- Exercise best practices in CLI design.
- Exercise best practices in OOP.

---

## Key Vocab

- **Command Line**: a text-based interface that is built into your computer's
  operating system. It allows you to access the files and applications on your
  computer manually or through scripts.
- **Terminal**: the application in Mac OS that allows you to access the command
  line.
- **Command Shell/Powershell/Windows Terminal**: the applications in Windows that allow you to
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

## Introduction

Welcome to the end of Phase 3! You've learned about a lot in this unit:

- Python fundamentals.
- Data structures (and more recently, algorithms).
- Object-oriented programming.
- Object inheritance.
- Instance and class attributes and methods.
- Configuring applications.
- SQL fundamentals.
- Table relations in SQL.
- Object-relational mapping with Python.
- Building CLIs.

You're going to use these skills to create a CLI and ORM application. The Phase
3 project is open-ended when it comes to the actual content. You are free to
create whatever you'd like, as long as it incorporates the requirements listed
below.

## Requirements

You need to implement a Python CLI Application that meets the following
requirements:

- The application must include a database created and modified with Python ORM
  methods provided by SQLAlchemy.
- The data model must include **at least 2** model classes.
- The data model must include **at least 1** one-to-many relationships.
- Property methods should be defined to add appropriate constraints to each model class.
- Each model class should include ORM methods (read, create, and delete at a minimum) using SQLAlchemy.
- Database migrations should be managed using Alembic.
- The CLI must display menus with which a user may interact.
- The CLI should use loops as needed to keep the user in the application until
  they choose to exit.
- For **EACH** class in the data model, the CLI must include options: to create an object,
  delete an object, display all objects, view related objects, 
  and find an object by attribute.
- The CLI should validate user input and object creations/updates, providing 
  informative errors to the user. 
- The project code should follow OOP best practices.
- The project should use a well-maintained virtual environment using Pipenv.
- Project folders, files, and modules should be organized and follow appropriate
  naming conventions.
- The project should include a `README.md` file that describes the application. If you are unsure what to include in a `README.md` file, please refer to [readme-requirements.md](./readme-requirements.md) in this repository. **Submitting your project with an empty or default `README.md` file will hurt your grade on this project.** 

You do **not** need to implement tests for `pytest`, although you should test
your code thoroughly using your CLI. Try entering bad data when prompted for
input, and confirm your application prints a useful error message.

## Before you write any code...
* You will be using SQLAlchemy for your ORM to construct your database, and you will be using Alembic for your migrations.  
* Clarify your models and associations **before** you start to code; migrations are a pain to deal with.
* Ideally, you will begin with an Entity Reference Diagram (ERD) you are happy with to guide you as you construct your database.
  * [DB Diagram](dbdiagram) is a great way to design a database schema starting from pseudo-code and diagrams. 
  * [Lucidchart](lucid) is an excellent resource to design a database schema graphically first. 
  * [This snapshot of a hypothetical user model](https://lucid.app/lucidchart/b2dcee4b-1f7d-474a-96a3-9cf07f9e45f5/edit?invitationId=inv_a3d2a25d-4e54-4a90-b4e8-531162cdd866) shows what a section of one of your ERDs might look like. 
* Making a good ERD is not trivial, and it is not easy. Do not skip this part. If you begin coding with a proper ERD, it will radically reduce the time it will take you to finish your project and help you avoid time-consuming errors and complicated migrations. 
* Keep your Python objects, SQLAlchemy objects, and CLI script in separate modules.

## How to begin?

- Start with the project template (provided in the following lesson). You are
  free to adapt the template structure, as long as you adhere to the project
  requirements.
- Think about the user interaction. How will you prompt the user? What
  information will the user enter? How will you provide feedback to the user?
- Think about your data model. How will you organize, store, and retrieve the information
  received from the user?
- If you get stuck trying to accomplish a specific task, check online to see if
  there's a Python library that will make it easier.
- Consider using [Click][click] or [Fire][fire] to take care of basic CLI tasks
  for you.



---

## Resources

- [README requirements](./readme-requirements.md)
- [SQLAlchemy documentation](https://docs.sqlalchemy.org/)
  - **NOTE** - Your curriculum focuses on SQLAlchemy 1.4! If you refer to SQLAlchemy documentation, make sure the version in your `Pipfile` matches the documentation you're referring to! 
- [Alembic documentation](https://alembic.sqlalchemy.org/)
- [Click documentation][click]
- [The Python Fire Guide][fire]
- [DB Diagram](dbdiagram)
- [Lucidchart](lucid)

[click]: https://click.palletsprojects.com/en/8.1.x/
[fire]: https://google.github.io/python-fire/guide/
[lucid]: https://lucidchart.com/pages/
[dbdiagram]: https://dbdiagram.io/
