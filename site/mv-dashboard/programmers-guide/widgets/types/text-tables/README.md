# Text Tables

<PageHeader />

Widgets can create HTML tables by setting the W$TYPE to “TABLE” and the following variables:


| <!----> | <!----> |
| --- | --- |
| W$TABLE.COL.LABELS<br> | VM-Array of column heading labels.<br> |
| W$TABLE.COL.JUST<br> | VM-Array of text-justification settings (“left”, “right”, “center”).<br> |
| W$TABLE.DATA<br> | AM/VM-Array. Each AM is a table ROW, each VM is a column within the row.<br> |
| W$TABLE.TOTALS<br> | VM-Array of total values (optional) at the bottom of each column. <br><br> |


This type of widget allows for easy creation of HTML-based tables. However, if you need more control over the way that these tables are presented, use the HTML type widget to create more complex tables.
<PageFooter />
