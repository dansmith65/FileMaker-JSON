### 1.0.3 ###

- add unit tests for JSON-FM and FM-JSON:
	- GitHub Issue #7: Printer quotes ruin your day: in array
	- GitHub Issue #7: Printer quotes ruin your day: in object


### 1.0.2 ###

- add unit tests for FM-JSON:
	- unicode control characters w/ backslash escape
	- unicode 0
	- unicode control characters w/out backslash escape

- add Speed Test scripts:
	- Speed Test: Template
	- Speed Test: Substitute vs Filter
	- Speed Test: Text vs Char function


### 1.0.1 ###

- unit tests for FM-JSON:
	- "text miss-interpreted as a date" unit test now produces expected result
	- add unit tests for "quoted number treated as list" bug
	- add misc. unit tests
	- add unit tests with large chunks of data to better represent real-world data

- update custom functions to current #Parameters module version 1.1.3:
	- #
	- #List


# 1.0.0 #

- the first release of this file did not include a separate version script for the application. This version script was created with JSON: Version 1.0.1.
- updated custom functions:
	#
	#GetNameList
	#List
- add unit tests for JSON-FM:
	- Object with returns
	- Array with returns
- unit tests for FM-JSON:
	- modify: Escape characters pt 2: returns/line endings
	- add: Escape characters pt 4: returns/line endings in object
- scripts
	- added
		- JSON-FM: Go To
		- FM-JSON: Go To
	- deleted
		- Toggle section
	- modified
		- FM-JSON: Parse All Found
		- FM-JSON: Parse letNotation text { skipRefresh }
		- FM-JSON: Parse letNotation expression { skipRefresh }
- update navigation button in header