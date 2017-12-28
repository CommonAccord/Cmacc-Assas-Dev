
/* Expand the embedded variables in a string, by replacing each variable with
the value of a corresponding key in a hash.

	While any variable in String:

Break the String into an array at the variables.  Could be that the
array is of each string up through the end of the variable. In which
case, each item in the array is a string (the leading part) and an
array that starts off as one item.  :

	Call the dictionary, by passing it a keyName and an array of (0-n)
    prefixes, and the number of answers desired (1-n).

	optionally wrap the returned value in meta data (keyName, mapName)

	replace the variable (and its escape characters) with the wrapped value.

	break
*/

const readString = (stringToRead, dictionaryName) =>{




const readDictionary = (keyName, prefixArray dictionaryName) => {

//return the value of the first matching key.  First matching means the one that is nearest to the top of the stack of references, and highest in the stack of the keyNameArray.  The first match is returned.  (In a further iteration, the second best match, etc. could also be returned.

//

}




To {R.Name}, {Author} is ready to {Activity}.

R.=Alice.md

Alice:

Name={R-FN} {R-LN}



To {Reader}
, {Author}
is ready to {Activity}
.


To
	{R.Name} ; Root ; Null

,
	{Author} ; Root ; Null

"is ready to"
	{Activity} ; Root ; Null

.


"To"
	{R-FN} {R-LN} ; Alice.md ; [R]

","
	{Author}  ; Root ; Null

"is ready to"
	{Activity} ; Root ; Null

.


"To"
	""
		{R-FN}; Alice.md ; [R]
		" "
	    {R-LN} ; Alice.md ; [R]

","
	{Author}  ; Root ; Null

"is ready to"
	{Activity} ; Root ; Null

.


"To"
	""
		"Alice"; Alice.md ; [R]
		" "
	   "Apple" ; Alice.md ; [R]

","
	{Author}  ; Root ; Null

"is ready to"
	{Activity} ; Root ; Null

.

