# openclinica_scripts
A place to put scripts relating to [OpenClinica](https://github.com/OpenClinica/OpenClinica). Some of these are listed on the [OpenClinica Extensions page](https://community.openclinica.com/extensions), or are mentioned in the [Wikibook](http://en.wikibooks.org/wiki/OpenClinica_User_Manual).

## [OC_XML_to_SAS_R_CSV](OC_XML_to_SAS_R_CSV)
XSL transformations for converting data from an ODM 1.3 XML into CSV, R, SAS and Access.

## [accessdatamart](accessdatamart)
Access database and accompanying scripts for building an SQL data mart - superseded by sqldatamart

## [codebook](codebook)
Python script for generating csv listing of all value-label pairs for coded items in a study, from an ODM 1.3 XML or study metadata XML file.

## [collate_rules](collate_rules)
XSL transformations for collating rule XML files into one file for editing / upload, and another for grouping (and ungrouping) rules by the target item.

## [compare_clinicaldata](compare_clinicaldata)
XSL transformation for combining multiple versions of an ODM 1.3 XML file for comparison, to show the changes in bulk

## [crf_manager](crf_manager)
Access database to read CRF .xls files in for review or editing, and write them out again.

## [dnotes](dnotes)
XSL transformations for preparing a pdf report of discrepancy notes from an ODM 1.3 XML file.

## [repeated_rules](repeated_rules)
Example of a CRF with many repeated items (16x50), a VBScript to generate rule xml for them based on a template (33 ruledefs, 35 rule actions) and selenium test suite to test the rules. 

## [scrape](scrape)
Python script for logging in to OpenClinica, scraping enrolment information and emailing a summary.

## [selenium_tasks](selenium_tasks)
Selenium scripts for automating user tasks - bulk CRF version migration, deleting rules.

## [sqldatamart](sqldatamart)
SQL scripts for building and maintaining a report database connected to OpenClinica's database via a foreign data wrapper. Also includes SQL scripts to facilitate export to xlsx (via R), and subsequent conversion to .dta (via stata) and .sas7bdat (via sas).

## [webservices](webservices)
Clients for interacting with OpenClinica webservices.

* Python 3 client, with tests! Returns Lists of OrderedDicts instead of XML.
* PHP client, now at: https://github.com/lindsay-stevens-kirby/openclinica_webservices_php

See also:

* [Java implementation by CTMM TraIT](https://github.com/jacobrousseau/traitocws/blob/master/TraITOCWS/src/nl/vumc/trait/oc/connect/OCWebServices.java)
* [Python implementation by Dimagi](https://github.com/dimagi/openclinica-xforms/blob/master/webservices.py)

## [xforms](xforms)
XSL transformation for converting an xform xml form into a flat structure for review.

## [xlsform_images](xlsform_images)
Python script that reads an ODK xlsform and generates images for each question, in order to provide a layout style that is a bit nicer than the default. Supports multiple languages. Included example xlsform and generated files with image settings ideal for a Galaxy Tab 4.