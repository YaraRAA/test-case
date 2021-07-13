# [MC number] [Imperfect Example] Validation and Replication results

> INSTRUCTIONS: Once you've read these instructions, DELETE THESE AND SIMILAR LINES.
> In the above title, replace [Manuscript Title] with the actual title of the paper, and [MC number] with the Manuscript Central number (e.g., AEJPol-2017-0097)
> Go through the steps to download and attempt a replication. Document your steps here, the errors generated, and the steps you took to alleviate those errors.

> Some useful links:
> - [Official Data and Code Availability Policy](https://www.aeaweb.org/journals/policies/data-code)
> - [Step by step guidance](https://aeadataeditor.github.io/aea-de-guidance/) 
> - [Template README](https://social-science-data-editors.github.io/template_README/)

SUMMARY
-------

> INSTRUCTION: The Data Editor will fill this part out. It will be based on any [REQUIRED] and [SUGGESTED] action items that the report makes a note of. 

> INSTRUCTION: ALWAYS do "Data description", "Code description". If data is present, ALWAYS do "Data checks". If time is sufficient (initial assessment!), do "Replication steps", if not, explain why not.

> INSTRUCTION: leave this in.

> The openICPSR submission process has changed. If you have not already done so, please "Change Status -> Submit to AEA" from your deposit Workspace.

> [NOTE] Starting July 1, 2021, we will start to publish replication packages as soon as all requested changes to the deposit have been made. Please process any requested changes as soon as possible.

General
-------

> INSTRUCTIONS: Leave this in, when any of the sections is lacking. Remove the entire section only if the README has all the pieces necessary (up to minor imprecisions).

> [SUGGESTED] A recommended README template for replication packages in economics can be found on the [Social Science Data Editor Github site](https://social-science-data-editors.github.io/guidance/template-README.html).

Data description
----------------

### Data Sources

#### US Census of Population

- Dataset is not provided, but a link is provided in the README: 
    https://doi.org/10.3886/ICPSR13568.v1
- Access conditions are  described. The website requires registration.
- The data are not cited in the paper nor in the README.

Suggested citation:

>United States. Bureau of the Census. Census of Population and Housing, 2000 [United States]:  Public Use Microdata Sample:  5-Percent Sample    . [distributor], 2006-01-12. https://doi.org/10.3886/ICPSR13568.v1

### Analysis Data Files


- [x] No analysis data file mentioned
- [ ] Analysis data files mentioned, not provided (explain reasons below)
- [ ] Analysis data files mentioned, provided. File names listed below.

> INSTRUCTIONS: List all provided filenames here. For large deposits, this can be done using the "Git Bash" program:
> > find . -name \*.dta
> will list all Stata datasets. Replace `dta` with `.Rdata` or any other extension to find other datafiles.

Example:

```
./Output_Empirical/data/census_shp/counties_coord.dta
./Output_Empirical/data/census_shp/counties_db.dta
./Output_Empirical/data/census_shp/state_coord.dta
./Output_Empirical/data/census_shp/state_db.dta
```

Data deposit
------------

> INSTRUCTIONS: Most deposits will be at openICPSR, but all need to be checked for complete metadata. Detailed guidance is at [https://aeadataeditor.github.io/aea-de-guidance/](https://aeadataeditor.github.io/aea-de-guidance/). 

### Requirements 

> INSTRUCTIONS: Check that these requirements are met. 

- [ ] README is in TXT, MD, PDF format
- [ ] openICPSR deposit has no ZIP files
- [ ] Title conforms to guidance (starts with "Data and Code for:" or "Code for:", is properly capitalized)
- [ ] Authors (with affiliations) are listed in the same order as on the paper

> INSTRUCTIONS: If any of the above are NOT checked, leave the related [REQUIRED] element here. Otherwise, delete the line.

> [REQUIRED] Please ensure that a ASCII (txt), Markdown (md), or PDF version of the README are available in the data and code deposit.

> [REQUIRED] openICPSR should not have ZIP files visible. ZIP files should be uploaded to openICPSR via "Import from ZIP" instead of "Upload Files". Please delete the ZIP files, and re-upload using the "Import from ZIP" function.

> [REQUIRED] Please review the title of the openICPSR deposit as per our guidelines (below).

> [REQUIRED] Please review authors and affiliations on the openICPSR deposit. In general, they are the same, and in the same order, as for the manuscript; however, authors can deviate from that order.

> INSTRUCTIONS: Leave the following line in the report if any of the above are checked:

> Detailed guidance is at [https://aeadataeditor.github.io/aea-de-guidance/](https://aeadataeditor.github.io/aea-de-guidance/). 

### Deposit Metadata

> INSTRUCTIONS: Some of these are specific to openICPSR (JEL, Manuscript Number). Others may or may not be present at other trusted repositories (Dataverse, Zenodo, etc.). Verify all items for openICPSR, check with supervisor for other deposits.

- [ ] JEL Classification (required)
- [ ] Manuscript Number (required)
- [ ] Subject Terms (highly recommended)
- [ ] Geographic coverage (highly recommended)
- [ ] Time period(s) (highly recommended)
- [ ] Collection date(s) (suggested)
- [ ] Universe (suggested)
- [ ] Data Type(s) (suggested)
- [ ] Data Source (suggested)
- [ ] Units of Observation (suggested)

> INSTRUCTIONS: Go through the checklist above, and then choose ONE of the following results:

- [NOTE] openICPSR metadata is sufficient.

or

- [REQUIRED] Please update the openICPSR metadata fields marked as (required), in order to improve findability of your data and code supplement. 

and/or

- [SUGGESTED] We suggest you update the openICPSR metadata fields marked as (highly recommended), in order to improve findability of your data and code supplement. 
- [SUGGESTED] We suggest you update the openICPSR metadata fields marked as (suggested), in order to improve findability of your data and code supplement. 


For additional guidance, see [https://aeadataeditor.github.io/aea-de-guidance/data-deposit-aea-guidance.html](https://aeadataeditor.github.io/aea-de-guidance/data-deposit-aea-guidance.html).

Data checks
-----------

No data are present so we ran no checks.


Code description
----------------

there are five provided Stata do files, including a "master.do", and one DCT (dictionary) file. 
- Table 1 is generated by '02_table1.do'
> INSTRUCTIONS: Review the code (but do not run it yet). Identify programs that create "analysis files" ("data preparation code"). Identify programs that create tables and figures. Not every deposit will have separate programs for this.

> INSTRUCTIONS: Identify all **Figure, Table, and any in-text numbers**. Create a list, mapping each of them to a particular program and line number within the program (use [this template](code-check-TEMPLATE.xlsx)). Commit that list. You will come back to the list in your findings. IN THIS SECTION, point out only a summary description, including of shortcomings. E.g.

There are four provided Stata do files, three Matlab .m files, including a "master.do".

- Table 5: could not identify code that produces Table 5
- Neither the program codes, nor the README, identify which tables are produced by what program.

> NOTE: In-text numbers that reference numbers in tables do not need to be listed. Only in-text numbers that correspond to no table or figure need to be listed.

Stated Requirements
---------------------

> INSTRUCTIONS: The authors may have specified specific requirements in terms of software, computer hardware, etc. Please list them here. This is **different** from the Computing Environment of the Replicator. You have the option to amend these with unstated requirements later. If all requirements are listed, check the box "Requirements are complete".

- [ ] No requirements specified
- [x] Software Requirements specified as follows:
  - Stata (inferred)
- [ ] Computational Requirements specified as follows:
  - Cluster size, etc.
- [ ] Time Requirements specified as follows:
  - Length of necessary computation (hours, weeks, etc.)

- [] Requirements are complete.

> If easier, simply copy-and-paste the authors' stated requirements here:


Missing Requirements
--------------------

> INSTRUCTIONS: If it turns out that some requirements were not stated/ are incomplete (software, packages, operating system), please list the *missing* list of requirements here. Remove lines that are not necessary. If the stated requirements are complete, delete this entire section, including the [REQUIRED] tag at the end.

- [x] Software Requirements 
  - [x] Stata
    - [x] Version
    - [x] Packages: 'latab'

> [REQUIRED] Please amend README to contain complete requirements. 

You can copy the section above, amended if necessary.

Computing Environment of the Replicator
---------------------

- CodeOcean, Stata 'MP 16.0 on Ubuntu 18.04
  - Stata Updated as of: 11 Dec 2019
  - Processors: 4

Replication steps
-----------------

1. We obtained a zip file from the authors with code.
2. Downloaded data from DOI indicated in the README. A sign-up was required.
3. Upliaded the code part to CodeOcean.
4. We adjusted some paths.
5. Code failed because command 'latab' was not installed
    - Added code to the "config.do" to install 'latab'
6. We created a few subdirectories to house the downloaded data and added to code to create directories for cleaned data.
7. We uploaded data.
8. Code ran without error.

>[SUGGESTED] Add code to "config.do" that creates directories named "inputdata" and "outputdata".

Findings
--------

> INSTRUCTIONS: Describe your findings both positive and negative in some detail, for each **Data Preparation Code, Figure, Table, and any in-text numbers**. You can re-use the Excel file created under *Code Description*. When errors happen, be as precise as possible. For differences in figures, provide both a screenshot of what the manuscript contains, as well as the figure produced by the code you ran. For differences in numbers, provide both the number as reported in the manuscript, as well as the number replicated. If too many numbers, contact your supervisor.



### Tables

Examples:

- Table 1: Looks the same


### In-Text Numbers

[x] There are no in-text numbers, or all in-text numbers stem from tables and figures.
[ ] There are in-text numbers, but they are not identified in the code


Classification
--------------

- [x] full reproduction
- [ ] full reproduction with minor issues
- [ ] partial reproduction (see above)
- [ ] not able to reproduce most or all of the results (reasons see above)

### Reason for incomplete reproducibility

- [ ] `Discrepancy in output` (either figures or numbers in tables or text differ)
- [ ] `Bugs in code`  that  were fixable by the replicator (but should be fixed in the final deposit)
- [ ] `Code missing`, in particular if it  prevented the replicator from completing the reproducibility check
  - [ ] `Data preparation code missing` should be checked if the code missing seems to be data preparation code
- [ ] `Code not functional` is more severe than a simple bug: it  prevented the replicator from completing the reproducibility check
- [ ] `Software not available to replicator`  may happen for a variety of reasons, but in particular (a) when the software is commercial, and the replicator does not have access to a licensed copy, or (b) the software is open-source, but a specific version required to conduct the reproducibility check is not available.
- [ ] `Insufficient time available to replicator` is applicable when (a) running the code would take weeks or more (b) running the code might take less time if sufficient compute resources were to be brought to bear, but no such resources can be accessed in a timely fashion (c) the replication package is very complex, and following all (manual and scripted) steps would take too long.
- [ ] `Data missing` is marked when data *should* be available, but was erroneously not provided, or is not accessible via the procedures described in the replication package
- [ ] `Data not available` is marked when data requires additional access steps, for instance purchase or application procedure. 
