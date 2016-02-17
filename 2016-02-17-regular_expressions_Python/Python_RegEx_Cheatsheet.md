#Python RegEx Cheatsheet

##Functions:

Function to find a regular expression in a string (returns a match object or none):
`re.search(pattern_to_search, string_to_search_in)`

How to extract the k'th regular expression from a string:
`match.group(k)` 

Function to find more than one occurence of a regular expression in a string (returns a matches or none):
`re.findall(pattern_to_search, string_to_search_in)`

Function to find more than one occurence of a regular expression in a string (returns a match object or none)
`re.finditer(pattern_to_search, string_to_search_in)`
 
Function to compile a pattern:
`re.compile(pattern_to_search)` 

##Symbols:

~~~
|		## "OR"
.		## any single character
*		## 0 or more 
+		## 1 or more
? 		## 0 or 1
{N} 	## match N times
{M,N} 	## matches from M to N times

[...]	## matches characters in a set defined by the user (see examples below)
[0-9]	## matches characters in the set from 0-9
[a-z]	## matches characters in the set from a-z
[A-Z]	## matches characters in the set from A-Z
[aeiou]	## matches characters in the set from aeiou

\d		## matches digits
\s		## matches whitespace characters ',' or  '\t' or  '\r' or '\n'
\w		## matches word characters [A-Za-z0-9]
\S 		## matches non-space characters
\W		## matches non-word characters
^		## matches the beginning of the input text
\b 		## matches the boundary between word and non-word characters
~~~