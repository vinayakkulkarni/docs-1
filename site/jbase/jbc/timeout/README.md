# TIMEOUT

<PageHeader />

## Description

The statement is used to terminate a read statement when no data has been read in a specified time period. It takes the general from:

```
TIMEOUT file.variable,Time
```

Where:

**file.variable** specifies a file opened for sequential access.

**time** is an expression that evaluates to the number of seconds the program should wait before terminating the [READSEQ](./../readseq) statement.

**TIMEOUT** causes subsequent [READSEQ](./../readseq) and [READBLK](./../readblk) statements to terminate and execute ELSE statements if the number of seconds specified by time elapses while waiting for data.

If either **file.variable** or **time** evaluates to null, the **TIMEOUT** statement fails and the program enters the debugger.

An example of use is as:

```
OPENSEQ "SLIPPERS" TO FILE_VAR ELSE ABORT 201
TIMEOUT FILE_VAR, 10
READBLK VAR1 FROM SLIPPERS, 15 THEN CRT VAR1 ELSE
    CRT "TIMEOUT OCCURRED"
END
```

Go back  to [jBASE BASIC](./../jbase-basic-programmers-reference-guide).

Go back to [Programmers' Reference Guide](./../../reference-guides/jbc/README.md)

<PageFooter />
