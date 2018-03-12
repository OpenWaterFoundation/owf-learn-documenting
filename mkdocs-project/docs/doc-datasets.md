# Learn Documenting / Documenting Datasets #

This section focuses on how to document datasets.

* [What is a Dataset?](#what-is-a-dataset)
* [Dataset Documentation Fundamentals](#dataset-documentation-fundamentals)
	+ [Data Properties](#data-properties)
	+ [Dataset Properties](#dataset-properties)
* [Dataset Documentation Options](#dataset-documentation-options)
* [Documentation Approach Decision](#documentation-approach-decision)

----

## What is a Dataset? ##

A "dataset" is a self-contained collection of data that with appropriate
definitions and context can be interpreted to gain understanding.
Typically a dataset represents observations of some phenomena (air temperature, population, etc.)
One way to think of a dataset is that it represents a fundamental collection of data
that can stand on its own.

Datasets also are often hierarchical, with relationships to sub-datasets and related datasets.
Datasets also are often aggregated using simple (total, mean, etc.) or
complex (distributions, correlations, etc.) statistical methods.

Examples of simple datasets include:

* A table of data samples, for example animal and its weight (a sample).
* A table of data samples, for example time and air temperature (a time series).
* A table with latitude and longitude and land use (a spatial data layer).

Examples of more complex datasets include:

* A collection of samples for different animal species at different locations and times (a database). 
* A collection of time series used to simulate a phenomena (a model).
* A collection of spatial data layers that can be viewed together (a geodatabase).

The spectrum of simple to complex datasets is governed by the domain in which the data are used.
Simple datasets can be used in multiple ways and complex datasets tend to focus on a specific goal.

## Dataset Documentation Fundamentals ##

To allow effective use of a dataset, the contents of a dataset must be understood.
Consequently, definitions must be articulated to describe dataset components.

### Data Properties ###

Ignoring the representation of a dataset (table, map layer, etc.),
elemental data within are typically described as a "property" or "attribute",
which has:

* definition (e.g., "air temperature", "animal weight", "water depth")
* data type (e.g., integer, decimal number, text, boolean, date, date/time, time)
* units (e.g., "degrees Celsius", "feet")
* measurement precision (e.g., date to month, .1-foot)
* value constraints (e.g., not null, one of "a, b, c", < 100)

Such information is typically called "metadata" (data about data) and software technologies
such as databases typically provide ways to record such information.
However, simple data formats such as comma-separated-value (CSV) files,
may be limited in representing metadata.

The individual metadata may also need further definition, for example:

* data units must use specific spellings (e.g, "in" rather than "inch") and only some units may be accepted
(e.g., "in" and "ft" but not "mile" or "km")
* date and time must adhere to a format (e.g., "YYYY-MM-DD" and not "mm/dd/YYYY")
and may need to account for time zone and daylight savings time
(see the [ISO 8601 specification](https://en.wikipedia.org/wiki/ISO_8601))
* spatial data must adhere to coordinate reference system standards (e.g., latitude and longitude or Web Mercator projection,
but no others allowed)
* international standards and locale-specific representations may impact data definition 
(e.g., text that uses a foreign language and special characters)

### Dataset Properties ###

The dataset may also be described with properties such as:

* author
* effective date (what date/time or period does the data apply?)
* publishing date
* limits on use
* attribution requirements
* schema

The above properties are less technical in some ways, although each dataset property must
be defined in a way that can be understood and used.
For example, is the author a name, or a full contact with address, and how is that data described?

The use of a "schema", which is a map of the dataset, can be quite technical and may refer to a published standard.

For example, the [Open Geospatial Consortium](http://www.opengeospatial.org/) publishes many standards.

## Dataset Documentation Options ##

Options for documenting datasets depend on the approach for maintaining and distributing the dataset.

### Text Files including CSV ###

* Use [Markdown](ref-markdown) files in same folder as the file(s),
especially if tracked in a version control system like GitHub.
	+ See example
	[README.md for Colorado Municipalities](https://github.com/OpenWaterFoundation/owf-data-co-municipalities/blob/master/README.md)
* Use [Google Docs](ref-google-docs) file parallel to the workbook, if files are stored as a Google sheet
* **Need to evaluate more options, such as comments within file**

### Microsoft Excel ###

* Use [Markdown](ref-markdown) files, especially if tracked in a version control system like GitHub.
	+ See example
	[README.md for Colorado Municipalities](https://github.com/OpenWaterFoundation/owf-data-co-municipalities/blob/master/README.md)
* Use [Google Docs](ref-google-docs) file parallel to the workbook, if files are stored as a Google sheet
* Add one or more worksheets to the workbook, with definitions and other information.

### Relational Database ###

* Define table metadata within the database and then automate creating a data dictionary
	+ One way to do this is with the TSTool software and CreateDataStoreDataDictionary command.	

### Model Dataset ###

* Use [Markdown](ref-markdown) files, especially if tracked in a version control system like GitHub.
	+ See example
	[Model dataset with README.md files](https://github.com/OpenWaterFoundation/cdss-model-cu-sw-yampa)

### Spatial Dataset (Spatial Data Layer) ###

* Use standard metadata files for spatial data layer
* Use [Markdown](ref-markdown) files, especially if tracked in a version control system like GitHub.
	+ See example 
	[README.md for Colorado Municipalities](https://github.com/OpenWaterFoundation/owf-data-co-municipalities/blob/master/README.md)
	for GeoJSON file

### Geodatabase ###

* Define table metadata within the database and then automate creating a data dictionary
	+ One way to do this is with the TSTool software and CreateDataStoreDataDictionary command.	

## Documentation Approach Decision ##

Consider the following questions when deciding which documentation approach to use:

1. If the dataset is maintained in a version control system such as Git, [Markdown](ref-markdown) files are an option.
2. If the dataset is maintained as a database, use the built-in database metadata features and software tools
to create a data dictionary.  Other documentation may still need to be created to track schema version release notes, etc.
3. If the dataset is maintained as a spatial data layer, use industry-accepted metadata standards.
If that approach does not apply, consider using simple formats such as [Markdown](ref-markdown).
5. If the dataset is maintained as a model dataset in a version control system such as Git,
consider using [Markdown](ref-markdown) files within the dataset files.
Markdown may also be appropriate for a longer integrated document, perhaps by using [Mkdocs](ref-markdown#mkdocs).
Traditional [Word/PDF](ref-word-pdf) is also an option.
