# frmttime
*frmttime* - is the fastest javascript 'strftime' implementation.

## Installation

### Browser:

**frmttime** can be [downloaded](https://raw.githubusercontent.com/sergey-shpak/frmttime/master/frmttime.js) and used as 
typical javascript library ( **frmttime** supports AMD, CommonJs and plain browser module exports).
 
[Script tag](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script)

    <script type="text/javascript" src="path_to_frmttime"></script>
    window.tools.frmttime
 
[AMD](https://addyosmani.com/writing-modular-js/):

    define('myModuleName', ['frmttime'], function( frmttime ){
    	// frmttime usage
    })

### NodeJS:

**frmttime** can be installed as [npm package](https://www.npmjs.com/):

    npm install frmtftime

And used as [CommonJS](https://addyosmani.com/writing-modular-js/):

    var frmttime = require('frmttime');
    // frmttime usage    

## Usage

## Supported Specifiers

### Seconds:
- L: the milliseconds, padded to 3 digits
- S: the second, padded to 2 digits (00-60)
- s: the number of seconds since the Epoch, UTC

### Minutes:
- M: the minute, padded to 2 digits (00-59)

### Hours:
- H: the hour (24-hour clock), padded to 2 digits (00-23)
- I: the hour (12-hour clock), padded to 2 digits (01-12)
- k: the hour (24-hour clock), padded with a leading space for single digit values (0-23)
- l: the hour (12-hour clock), padded with a leading space for single digit values (1-12)
- P: "am" or "pm" in lowercase
- p: "AM" or "PM"

### Days:

- A: full weekday name
- a: abbreviated weekday name
- d: day of the month, padded to 2 digits (01-31)
- e: day of the month, padded with a leading space for single digit values (1-31)
- j: day of the year, padded to 3 digits (001-366)
- o: day of the month as an ordinal (without padding), e.g. 1st, 2nd, 3rd, 4th, ...
- w: the weekday, Sunday as the first day of the week (0-6)
- u: the weekday, Monday as the first day of the week (1-7)

### Weeks:
- U: week number of the year, Sunday as the first day of the week, padded to 2 digits (00-53)
- W: week number of the year, Monday as the first day of the week, padded to 2 digits (00-53)

### Months:
- B: full month name
- b: abbreviated month name
- h: the same as %b (abbreviated month name)
- m: the month, padded to 2 digits (01-12)

### Years: 
- C: AD century (year / 100), padded to 2 digits
- Y: the year with the century
- y: the year without the century (00-99)

### Other equivalents, timezones, etc:
- D: equivalent to `%m/%d/%y`
- F: equivalent to `%Y-%m-%d`
- n: newline character
- R: equivalent to `%H:%M`
- r: equivalent to `%I:%M:%S %p`
- T: equivalent to `%H:%M:%S`
- t: tab character
- v: equivalent to `%e-%b-%Y`
- Z: the time zone name, replaced with an empty string if it is not found
- z: the time zone offset from UTC, with a leading plus sign for UTC and zones east
     of UTC and a minus sign for those west of UTC, hours and minutes follow each
     padded to 2 digits and with no delimiter between them
     
## License

Copyright © 2014 Sergey Shpak <sergey.shpak.web@gmail.com>

[MIT license](http://shps.mit-license.org)
