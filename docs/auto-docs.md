# AutoDocstring by Justus Decker

### file_write
Writes to a file in `wb` mode
## AutoDocstring
Gets all Docstrings contained in the `{current_folder}` & subdirectories and saves it to `{self.filepath}`.
### doc -> AutoDocstring
Writes documentation into `self.DOCS`
Adds a new-line each time
### get_python_paths -> AutoDocstring
Gets all the python files in the tree.
### __class_fetch -> AutoDocstring
* Creates documentation for itself
* Iterates over all methods in a class
    * Creating Documentation for the method
    * Set the method / function as flagged so it does not show up more than once.
### __funcmeth_fetch -> AutoDocstring
Creates the documentation for a function / method.
Only create the documentation in the case of:
```python
if obj.lineno not in aw
``` 
### generate -> AutoDocstring
The Entry point for creating auto-docs.
Creates a file automatically.
## FG
Contains all 16 Foreground Colors + Reset
## BG
Contains all 16 Background Colors + Reset
