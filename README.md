# bracketeer
Formats a formula string with brackets over multiple lines to help understand the components of a formula.

There is only one file with html, css and javascript to make it easy to use.

To use this little app, open the file in any web browser and paste or type in the formula into the top text box. The lower text area will show the formula split into separate lines to assist in understanding the formula elements.

The text boxes will resize to suit the input and output.

For example, the Excel formula

```
=IF(WEEKDAY(DATE($A$1,(ROW()+1)/3,1))=COLUMN()-1,1,IF(AND(ISNUMBER(B2),B2>0),B2+1,0))
```

Will be shown as 

```
=IF(                                                                                )
    WEEKDAY(                        )=COLUMN()-1,1,IF(                             )
            DATE(                  )                  AND(                 ),B2+1,0
                 $A$1,(       )/3,1                       ISNUMBER(  ),B2>0
                       ROW()+1                                     B2
```                        
This makes it easier to see if there are mismatched brackets or if the brackets are not correctly positioned.
