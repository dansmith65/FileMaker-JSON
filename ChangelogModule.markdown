### 1.0.6 ###

release date: 2017-DEC-01

When converting FM to JSON and a value is already a JSON object or array, don't convert it to a string.

- modify scripts:
	- ~JSON-FM String


### 1.0.5 ###

release date: 2016-MAY-05

- modify scripts:
	- FM-JSON ( letNotation )
	- ~JSON-FM Value
	- ~JSON-FM String
	- ~FM-JSON { value }


### 1.0.4 ###

release date: 2015-MAR-30

- modify scripts:
	- ~FM-JSON { value }
		- fix bug: time or timestamp with milliseconds would use the right two digits as the seconds and would not display milliseconds
		- fix bug: (GitHub Issue #6) return delimited list of field names from the current layout were detected as an array
		- now requires an array to end in a trailing return (which is the format produced by the #List function)
			- modified the "manually generated array" unit tests to reflect this change


### 1.0.3 ###

- modify scripts:
	- ~FM-JSON { string }
		- fix bug: encode unicode control characters


### 1.0.2 ###

- modify scripts:
	- ~FM-JSON { value }
		- update test that differentiates an array from a string
			- previously, a quoted number was interpreted as an array
	- ~JSON-FM Object
		- update # ( name ; value ) function used in encode object section to version date 2014-06-06
	- ~JSON-FM Array
		- update #List ( value ) function used in encode value section to version date 2014-06-06
	- JSON: READ ME
		- add "UPGRADE PROCESS" section


### 1.0.1 ###

- fix Issue #1 and #2 from GitHub
- modify scripts:
	- JSON: Changelog: Detailed
		- deleted, will store list of all changes in the version script instead
	- ~JSON-FM Object
		- update # ( name ; value ) function used in encode object section
	- ~JSON-FM Array
		- update #List ( value ) function used in encode value section
	- ~FM-JSON { value }
		- fix handling of LF and CRLF returns/line endings
		- accommodate numbers encoded with GetAsNumber
		- return an error if an unknown GetAs... function is detected
		- prepend decimals with a 0, as required by JSON standard
	- ~FM-JSON { object }
		- process object as ¶ delimited list instead of a return delimited list, which didn't work for Char(10)
		- this is now the same method of processing as #Get ( parameters ; name ) function uses
	- ~JSON-FM Next { character }
		- add space before "instead of"
	- JSON: READ ME
		- update documentation


# 1.0.0 #

- initial release