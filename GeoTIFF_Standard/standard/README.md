# The GeoTIFF Standard

## Content

This folder contains the text for the GeoTIFF standard

* GeoTiff.adoc - the main standard document with references to all sections
* remaining adocs - each section of the standard document is in a separate document: follow directions in each document to populate
* images - directory for image files used as figures
* requirements - directory for requirements and requirement classes to be referenced from clause_7_requirements.adoc
* code - sample code to accompany the standard, if desired
* abstract_tests - the Abstract Test Suite comprising one test for every requirement, optional
* UML - UML diagrams, if applicable

## Building

To produce the HTML of the standard run `asciidoctor --safe -a data-uri -o GeoTiff.html GeoTiff.adoc`.

To produce the PDF of the standard run `asciidoctor-pdf --safe -o GeoTiff.pdf GeoTiff.adoc`
