```coldfusion
humanize(text [, except ])
```
```coldfusion
// Humanize a string, will result in "Wheels Is A Framework" 
#humanize("wheelsIsAFramework")#

// Humanize a string, force wheels to replace "Cfml" with "CFML" 
#humanize("wheelsIsACFMLFramework", "CFML")#
```