## tech.cohorte.pinea.cipclientcore.tools.CIPConnectionPathValidator

### Fields Summary

| Modifier and Type                    |  Field and Description                                                                                                                                                                                |
|--------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Private Pattern                       | `pattern` <br> Java pattern to compile regex                                                                                                                                                                         |
| Private Matcher                      | `matcher` Java matcher , it takes path as argument and match it to a pattern                                                                                                                                    |
| static final String CIPPATH\_PATTERN | A Regex pattern to allow strictly of 8 HEX Values,  which means both maximum and minimum hex values of a path is  8 values all separated by spaces \. Path should be like Ex: 20 04 24 64 2C 66 2C 65 |

### Constructor Summary

| Modifier                    |   Description                                                                                    |
|-----------------------------|--------------------------------------------------------------------------------------------------|
| Public                      | `CIPConnectionPathValidator()` <br> Constructs a CIPConnectionPathValidator object and compile the java pattern with regex provided  |                                                                                                     
### Methods Summary

| Modifier and Type          | Method and Description                    |
|-------------------|--------------------------------|
| boolean           | `validate(final String path)` <br>  return true if a valid cip path, false when an invalid cip path |
| List<Integer>     | `connectionPathToHexValues(final String path)`  <br>   Transform a String Array path of Hex numbers to array of numbers after validating the path.                    |
