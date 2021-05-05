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

Returns a new string extracted from a string without altering the original string using a starting index and optionally an ending index. Negative index values can be utilized to determine index positions from the end of the string

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

### >>match<<

Returns array of found strings that pass the regular expression argument within a string.

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


repeat
replace
search
split
substr
toLowerCase
toUpperCase
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
