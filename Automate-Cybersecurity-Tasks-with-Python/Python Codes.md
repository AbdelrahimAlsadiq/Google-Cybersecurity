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

### `print()`
- Outputs a specified object to the screen.

</br>

### `type()`
- Shows the type of an object.

</br>

### `range()`
- Generates a sequence of numbers.

</br>

### `max()`
- Returns the largest numeric input passed into it.

</br>

### `min()`
- Returns the smallest numeric input passed into it.

</br>

### `sorted()`
- Sorts the components of a list.

</br>

### `int()` - `str()` - `float()` - `list()` - `tuple()` - `set()`
- convert the input object into specified data type.

</br>

### `len()`
- Returns the number of elements in an object.

---
## String Methods

</br>

### `.upper()`
- Returns a copy of the string in all uppercase letters.

</br>

### `.lower()`
- Returns a copy of the string in all uppercase letters.

</br>

### `.split("pattern")`
- Converts a string into a list.
> Examples:
>- "Hello-World".split("-") will produce: ["Hello", "World"].
>- "Hello World".split() will produce: ["Hello", "World"] (default value of the pattern is a space).

</br>

### `"pattern".join(obj)`
- Concatenates the elements of an iterable object into a string.
> Examples:
>- "".split("-") will produce: ["Hello", "World"].
>- "Hello World".split() will produce: ["Hello", "World"] (default value of the pattern is a space).

</br>

### `.index()`
- Finds the first occurrence of the input in a string and returns its location.

---
## List Methods

</br>

### `.insert()`
- Adds an element in a specific position inside a list.

</br>

### `.toupper()`
- Returns a copy of the string in all uppercase letters.

</br>

### `.remove()`
- Removes the first occurence of a specific element in a list.

</br>

### `.append()`
- Adds input to the end of a list.

</br>

### `.index()`
- Finds the first occurrence of the input in the list and returns its location.

---
## Regular Expressions (Regex)

> Note: Regular expressions can be used when "re" module is imported.

</br>

### `re.findall(expression, obj)`
- Returns a list of matches to a regular expression.

</br>

### `+`
- Represents one or more occurrences of a specific character.

</br>

### `.`
- matches to all characters, including symbols
>Note: for period character, you can use "`\.`".

</br>

### `\w`
- Matches with any alphanumeric character but it doesn't match symbols.


</br>

### `\d`
- matches to all single digits [0-9].

</br>

### `\s`
- matches to all single spaces.

---
## Managing Files

</br>

### `with`
- Handles errors and manages external resources.

</br>

### `with open("filePath", "action") as file:`
- Opens a specified file and stores it in `file` object.
>"action" can be:
  >- "r" for read.
  >- "w" for write (removes existing text).
  >- "a" for append (write without removing existing text).

</br>

### `file.read()`
- Converts file contents into strings.

</br>

### `file.write()`
- Writes string data to a specific file.

</br>

### `Example:`
- ```python
  # Read data from a file:
  with open("F:\\Desktop\\file.txt", "r") as file:
    text = file.read()
  print(text)

  # Write data to a file:
  data = "Hello Python!"
  with open("F:\\Desktop\\file.txt", "w") as file:
    file.write(data)
  ```
  >Output1: File contents.



