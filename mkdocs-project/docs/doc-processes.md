# Learn Documenting / Documenting Processes #

This section focuses on how to document processes.

* [What is a Process?](#what-is-a-process)
* [Process Documentation Fundamentals](#process-documentation-fundamentals)
* [Process Documentation Options](#process-documentation-options)
* [Documentation Approach Decision](#documentation-approach-decision)

----

## What is a Process? ##

A process is a sequence of steps performed to complete a task:

* A process typically requires input and produces output.
* A process can be simple or complex.
* A process can be linear or branching with decision points.
* A process is typically repeated, but may change over time.
* A process can be manual or automated, or both.
* A process may involve roles and validation.

It may also be appropriate to document a group of processes, such as an "Operations Manual" or a "Modeling Manual".  In
this case, use a suitable documentation approach for a larger effort such as a [Project](doc-projects)
and incorporate documentation concepts from this section.

## Process Documentation Fundamentals ##

To allow effective use of a process, the input, workflow, and output of the process must be understood.
Consequently, definitions must be articulated to describe process components.

### Process Input ###

**Need to complete**

### Process Workflow ###

**Need to complete**

### Process Output ###

**Need to complete**

## Process Documentation Options ##

Options for documenting datasets depend on the approach for maintaining and distributing the dataset.

### Text Command Files ###

Command files are "macro language" files such as those used by TSTool, StateDMI, and GeoProcessor.

* Use in-lined comments in the command files.
	+ See example
	[TSTool command files to process Colorado Municipalities](https://github.com/OpenWaterFoundation/owf-data-co-municipalities/tree/master/analysis)
* Use [Markdown](ref-markdown) files in same folder as the file(s),
especially if tracked in a version control system like GitHub.
	+ **Need a README.md file in the above**

### Scripts ###

Scripts can be directly run, such as batch files, shell script, and Python scripts.

* Use in-lined comments to the scripts.
	+ **Need an example**
* Use [Markdown](ref-markdown) files in same folder as the file(s),
especially if tracked in a version control system like GitHub.
	+ **Need an example**

## Documentation Approach Decision ##

Consider the following questions when deciding which documentation approach to use:

1. If the process workflow is maintained as a text file in a version control system such as Git,
[Markdown](ref-markdown) files are an option.
2. If the process is complex and deserves a longer manual, [Markdown](ref-markdown) files as a static website is an option - use MkDocs.
3. Processes that need to be described as part of a policy and are less hands-on with data and software
may need to use traditional Word/PDF documentation approach.

**Need to add more content**
