# JCL DEBUG

<PageHeader />

**Tags:**
<badge text='jcl' vertical='middle' />

## Description

The command turns debug function on or off. It takes the general form:

```
DEBUG [ON|OFF]
```

## Note

> When the DEBUG function is turned on, the jCL  program will be suspended before each command (line) is executed. Displayed will be the program name and the next command to be executed. A prompt will appear expecting one of the following commands:

| Command | Description  |
| --- | --- |
| &lt;Enter&gt; | execute current line |
| ? | display list of available commands |
| e | toggle last error display |
| f | toggle file buffer display |
| h | display list of available commands |
| i | toggle input buffer display |
| n | toggle next line display between one and two lines |
| o | toggle output buffer display |
| q | quit (terminate) program |
| x | exit DEBUG function |

After each input, the program name and the next line to be executed will be redisplayed, together with any additional information requested (for example, the content of the input buffers).

Back to [jCL.](./../README.md)
  
<PageFooter />