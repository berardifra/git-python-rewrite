# About The Project

Just rewriting Git with Python. Why?

1. Is fun
2. To finally get it
<br><br>
# Classes

### GitRepository

1. **Description:** the repository object
2. **Attributes:**
    - *worktree*: the work tree is the path where the files that are meant to be in version control are
    - *gitdir*: the git directory is the path where git stores its own data. Usually is a child directory of the work tree, called .git
    - *conf*: is an instance of the class ConfigParser, from the external module configparser, used to read and write INI configuration files

### GitObject

1. **Description:** base class that abstracts the common  features of different object types (e.g., blob, commit, tag or tree)
2. **Attributes:**
    - *init*: will be used by the derived class to create a new empty object if needed (optional)
    - *eserialize*: will be used by the derived class to convert the data into an object (mandatory)
    - *serialize*: will be used by the derived class to convert the object into a meaningful representation (mandatory)
<br><br>
# Getting Started

### Pre-requisites
- *Python version 3.10* or higher along with your favorite text editor. We won’t need third party packages or virtualenvs, or anything besides a regular Python interpreter: everything we need is in **Python’s standard library.**