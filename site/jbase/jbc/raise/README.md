# RAISE

<PageHeader />

## Description

The **RAISE** function raises system delimiters in a string to the next highest delimiter. It takes the general form:

```
RAISE(expression)
```

Where:

**expression** is a string containing one or more delimiters, which are raised as follows:

| ASCII Character | Raised To |
| --- | --- |
| 248 | 249 |
| 249 | 250 |
| 250 | 251 |
| 251 | 252 |
| 252 | 253 |
| 253 | 254 |
| 254 | 255 |

An example of use is as:

```
ValuemarkDelimitedVariable = "A"+@VM+B+@SM+C+@SM+D+@VM+E
AttributeDelimitedVariable = RAISE(ValuemarkDelimitedVariable)
CRT AttributeDelimitedVariable
```
RESULT
```
"A"+@AM+B+@VM+C+@VM+D+@AM+E
```
Go back to [jBASE BASIC](./../README.md)

Go back to [Programmers' Reference Guide](./../../reference-guides/jbc/README.md)

<PageFooter />
