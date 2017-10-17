############################
### CMYK regex validator ###
############################

Regex to check for validity of CMYK values. 
The regex is javascript-compatible and does not use PCRE -style if-statements.
Currently only accepts percentage values with or without the alpha channel.

Do note that I am not very comfortable with regex and take no responsibility for anything that goes wrong with using this.

[DEMO](https://regex101.com/r/6vDDKY/1)

Regex:

(cmyk\()(((100\%\,\s?)|((\d{1,2})((?=(\%\,\s?))(\%\,\s?)|(?!=(\%\,\s?))(\.\d{1,4}\%\,\s?)))){3})((100\%)|((\d{1,2})((?=(\%))(\%)|(?!=(\%))(\.\d{1,4}\%))))(((?=(\,\s?))((\,\s?)((100\%)|((\d{1,2})((?=(\%))(\%)|(?!=(\%))(\.\d{1,4}\%))))))\)|((?!=(\,\s?))(\))))\;