# AutoDocs

# ./ncu/auto_docs.py

### file_write
Writes to a file in `wb` mode
## AutoDocs
Gets all Docstrings contained in the `{current_folder}` & subdirectories and saves it to `{self.filepath}`.
### doc -> AutoDocs
Writes documentation into `self.DOCS`
Adds a new-line each time
### get_python_paths -> AutoDocs
Gets all the python files in the tree.
### __class_fetch -> AutoDocs
* Creates documentation for itself
* Iterates over all methods in a class
    * Creating Documentation for the method
    * Set the method / function as flagged so it does not show up more than once.
### __funcmeth_fetch -> AutoDocs
Creates the documentation for a function / method.
Only create the documentation in the case of:
```python
if obj.lineno not in aw
``` 
### generate -> AutoDocs
The Entry point for creating auto-docs.
Creates a file automatically.
# ./ncu/constants.py

## FG
Contains all 16 Foreground Colors + Reset
## BG
Contains all 16 Background Colors + Reset
# ./ncu/git_automation.py

### run_git_command
Runs a git command and returns the output.
# ./ncu/update_version.py

## UpdateVersion
Updates the current project-version.

Version-scheme:
```python
"{major}.{minor}.{patch}"
major : int
minor : int
patch : int
```

Parameters:
* **pathname**: default -> `./src/version.py`, this is the path of the file that contains the `varname` variable
* **inc**: default -> `0.0.1` will be added to the current version
* **varname**: default -> `__version__`, the variable name to overwrite

Attributes:
* **new_version**: (tuple[int, int, int] | None)
* **old_version**: (tuple[int, int, int] | None)
* **varname**: (str) -> look into parameters
* **pathname**: (str) -> look into parameters
* **inc**: (str) -> look into parameters
