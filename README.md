toolbox
=======

## What is the toolbox?

The toolbox is a collection of small work-in-progress scripts and code snippets for text processing produced by CLiGS.

Note that all functions are designed for Python 3 and are experimental in nature and quality. Each folder contains one or several Python scripts and some sample texts for testing. Currently, we are transitioning towards the toolbox as a module (see below). 

## Experimental feature: toolbox as module

This allows using the scripts as a repo-based module. The basic idea is that you clone the toolbox repository from GitHub and add the path to the folder containing the toolbox to your Python sys.path (using the script "activate_toolbox.py" which is included here). Then, you can import modules and submodules from the toolbox in your custom text processing scripts anywhere on your computer and use the functions provided in the toolbox. You may want to create your own branch of the toolbox to customize the functions as necessary. 

## Module structure

In order to use the module efficiently, you need to know which submodules are included, which functions are included in each submodule, and which arguments each function takes. The following is intended as a quick overview, please see the submodules themselves for details. 

* extract.py
    * read_tei5(teiFolder, txtFolder, xpath)
    * read_tei4(teiFolder, txtFolder)
    * get_metadata(teiFolder, metadataFile, mode)


## Example

If you want to read text from a TEI P5 file, you could use the following import statement and function call in your script: 

```
from toolbox import extract

extract.read_tei5([add arguments here])            
```
