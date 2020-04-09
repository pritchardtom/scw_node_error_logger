# Simple Node Error Logger for SCW

A really basic Python CLI to store node errors in a sqlite3 database, and allow users to query this database.

## How to add a Node Error

Each node error consists of the following attributes:

- A node name;
- Date the error occurred;
- The error message; and
- The date the error was cleared.

This information can be logged in two ways:

1. Interactive Mode; and
2. Command Line Mode.


### 1. Interactive Mode

- Simply enter following command: `scw_node_logger -i`
- Enter the information as prompted.
- Done.


### 2. Command Line Mode

- Involves passing arguments.
- What should these be?
- And isn't this really clunky?
  - `-i` --> interactive mode
  - `-b` --> batch file mode
  - `-n` --> node name

- Something like:

```
 scw_node_logger -n scs0074 -d 01/01/2020 -m this is an error message -c 04/01/2020
```
