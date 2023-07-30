## Comments
- A note programmers make about the intention behind their code.
- Syntax:
    ```python
    # this is single line comment
    ```
    
    ```python
    """
    this is 
    multi-line comment.
    """
    ```
---
## Conditional Statements:
- Syntax:
  ```python
  if condition :
    statements
  else
    statements
  ```
  >Note: "else" is optional, and for multiple conditions we can simplify it to "elif"
---
## For Loop:
- Syntax:
  ```python
  for LoopVariable in Sequence:
    statements
  ```
  >Note: "Sequence" can be generated using range() function.
---
## While Loop:
- Syntax:
  ```python
  while condition:
    statements
  ```
---
## Creating a function:
- Syntax:
  ```python
  def funName ():
    body statements
    return returnValue
  ```
  >- Parameters can be as many as you want, separated by commas (example: funName(x, y, z))
  >- Return value is optional, you can create a function that returns nothing (void).
---
## Importing a Module:
- Syntax:
  ```python
  # Entire module:
  import moduleName

  # Specific parts from the module:
  from moduleName import fun1, fun2
  ```
  >**Some great modules for cybbersecurity**:
  >- The re module, which provides functions used for searching for patterns in log files
  >- The csv module, which provides functions used when working with .csv files
  >- The glob and os modules, which provide functions used when interacting with the command line
  >- The time and datetime modules, which provide functions used when working with timestamps
## Built-in Functions
</br>

### print()
- Outputs a specified object to the screen.

</br>

### type()
- Shows the type of an object.

</br>

### range()
- Generates a sequence of numbers.

</br>

### max()
- Returns the largest numeric input passed into it.

</br>

### min()
- Returns the smallest numeric input passed into it.

</br>

### sorted()
- Sorts the components of a list.