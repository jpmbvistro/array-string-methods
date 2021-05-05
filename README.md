# JS String and Array Methods for Interviewing

Each Method is structured to provide EUE
Explanation
Use
Example

## String Methods

### >>charAt<<

Returns the character at a specified zero-based index

#### Use:
```
<string>.charAt(<index>)
```


#### Example:
```
let stringy = 'Bubleh!'
console.log( stringy.charAt(2) )
//Expect to print 'b'

console.log( stringy.charAt(6) )
//Expect to print '!'
```


### >>charCodeAt<<

Returns the UTF-16 code of a character at a specified zero-based index

#### Use:
```
<string>.charCodeAt(<index>)
```

#### Example:
```
let stringy = 'Bubleh!'
console.log( stringy.charCodeAt(2) )
//Expect to print '98'

console.log( stringy.charCodeAt(6) )
//Expect to print '33'
```

### >>concat<<

Returns a new string, the second string added to the first

#### Use:
```
<string1>.concat(<string2>)
```

#### Example:
```
let string1 = 'Bubleh!'
let string2 = 'Oobleck?'
console.log( string1.concat(string2) )
//Expect to print 'Bubleh!Oobleck?'

console.log( string2.concat(string1) )
//Expect to print 'Bubleh!Oobleck?'
```

### >>includes<<

Returns a boolean value if argument string is in a string

#### Use:
```
<string1>.includes(<string2>)
```

#### Example:
```
let string1 = 'Bubleh!'
console.log( string1.includes('eh!') )
//Expect to print 'true'

console.log( string1.includes('Bub!') )
//Expect to print 'false'
```

### >>indexOf<<

Returns the zero-based index of the argument string. Returns -1 if string is not found

#### Use:
```
<string1>.indexOf(<string2>)
```

#### Example:
```
let string1 = 'Bubleh!'
console.log( string1.indexOf('h!') )
//Expect to print '5'

console.log( string1.indexOf('!h') )
//Expect to print '-1'
```

### >>slice<<

Returns a new string extracted from a string without altering the original string using a starting index and optionally an ending index. Negative index values can be utilized to determine index positions from the end of the string. If starting index is larger than ending index, then resulting string is empty

#### Use:
```
<string1>.slice(<starting index>)
<string1>.slice(<starting index>, <ending index>)
```

#### Example:
```
let string1 = 'Bubleh!'
console.log( string1.slice(-2) )
//Expect to print 'h!'

console.log( string1.slice(2,4) )
//Expect to print 'bl'
```

### >>substring<<

Returns a new string extracted from a string without altering the original string using a starting index and optionally an ending index. Negative index values can be utilized to determine index positions from the end of the string. If starting index is larger than ending index, then resulting string swaps the positions.

#### Use:
```
<string1>.substring(<starting index>)
<string1>.substring(<starting index>, <ending index>)
```

#### Example:
```
let string1 = 'Bubleh!'
console.log( string1.substring(-2) )
//Expect to print 'h!'

console.log( string1.substring(2,4) )
//Expect to print 'bl'
```

### >>substr<<

Returns a new string extracted from a string without altering the original string using a starting index and optionally a number of characters to extract. Negative length values are interpreted as 0.

#### Use:
```
<string1>.substring(<starting index>)
<string1>.substring(<starting index>, <ending index>)
```

#### Example:
```
let string1 = 'Bubleh!'
console.log( string1.substring(1) )
//Expect to print 'ubleh!'

console.log( string1.substring(1,2) )
//Expect to print 'ub'
```

### >>split<<

Returns an array of strings from a string, utilizing a passed argument string as a delimiter. If an empty string is passed, the resulting array will contain individual characters.

#### Use:
```
<string1>.split(<string2>)
```

#### Example:
```
let string1 = 'Bubuleh!'
console.log(string1.split('u'))
//Expect to print ['B','b','leh!']

console.log( string1.split('') )
//Expect to print ['B','u','b','u','l','e','h','!']
```

### >>match<<

Returns array of found strings that pass the regular expression argument within a string. Returns Null if nothing found

#### Use:
```
<string1>.match(<regex>)
```

#### Example:
```
let string1 = 'Bubleh! oh :('
console.log( string1.match('/([A-Z])\w+/g') )
//Expect to print ['Bubleh']

console.log( string1.match('/([a-z])\w+/g') )
//Expect to print ['ubleh','oh']
```

### >>toLowerCase<<

returns a new string with each letter character being lower case

#### Use:
```
<string1>.toLowerCase())
```

#### Example:
```
let string1 = 'Bubleh! oh :('
console.log( string1.toLowerCase() )
//Expect to print 'bubleh! oh :('
```

### >>toUpperCase<<

returns a new string with each letter character being upper case

#### Use:
```
<string1>.toUpperCase())
```

#### Example:
```
let string1 = 'Bubleh! oh :('
console.log( string1.toUpperCase() )
//Expect to print 'BUBLEH! OH :('
```

### >>trim<<

removes white space from end and start of string

#### Use:
```
<string1>.trim())
```

#### Example:
```
let string1 = 'Bubleh! oh :('
console.log( string1.toUpperCase() )
//Expect to print 'BUBLEH! OH :('
```


repeat
replace
search


trim





## Array Methods

map
reduce
filter
forEach
sort
slice
pop
shift
push
unshift
includes
indexOf
every
