# dateutil-parser-timezones
Timezone data for use with the Python dateutil module

If you are anything like me you got very excited when you saw that the Python [dateutil](https://github.com/dateutil/dateutil/) module can parse date and time strings.  So cool - it even does timezones!  Well, yes and no.  It can recognize timezones, but you have to supply the timezone identifiers with their associated timezone information.  

Well, that has to be easy, right?  I mean, there is a ton of timezone information out there!  That is true, but I found it very difficult to find a straightforward mapping between timezone abbreviations and IANA time zone identifiers.  The files in this repository address that.

This repository contains an Excel spreadsheet containing a list of short timezone identifiers taken from [Wikipedia](https://en.wikipedia.org/wiki/List_of_time_zone_abbreviations), the IANA time zone identifier, the common name for the time zone, and the UTC offset.  It also contains a Python function that can output a dictionary that is ready for the dateutil parser.

Date and time decisions are never easy, and there are several collisions in the timezone abbreviations.  Ones that didn't make the cut are highlighted in red on the spreadsheet.  Tweak as you see fit.  

Every effort has been made to assure the accuracy of the list, but errors may be present.  The accuracy of the list may drift over time as well since I will not be actively maintaining it.  Let me know about any issues and I will get them corrected.  Alternatively, submit a pull requiest and I will get it merged
