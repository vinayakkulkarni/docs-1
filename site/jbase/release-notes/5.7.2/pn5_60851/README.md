# PN5_60851

<PageHeader />

## Description

Compiler parsing issue when a function definition [DEFFUN] has the same name as a DIM() or COMMON array

### Previous Release Behavior

The following code should not be allowed to compile, but did:

```
COMMON xyz(100)
DEFFUN xyz()
x = xyz()       ;* intended function call
```

### Current Release Behavior

Compiling the above code will produce an error similar to:

```
jpp2: Error Variable xyz at line 1 in file test.b is both a function and a dimensioned array.

Error occurred connecting jbc Pre-Processor, jpp: No error
jbccom -f -d -a. BASIC_2.b failed , command returned a code of 2
jcompile: Returned an error code of 8
 ** Unable to compile source aaa.b **
Return code = BASIC_ERROR
```

Back to [5.7.2 Release Notes](./../jbase-5.7.2.1-release-notes/README.md)
  
<PageFooter />
