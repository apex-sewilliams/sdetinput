## Overview
Please create a program that will read input (either locally or from github), parse it, and generate the appropriate output.

Use any development environment you prefer, as well as whatever language you want.  This is an “open book” exercise and you are encouraged to use the Internet to look things up, though we ask that you not use any LLMs (  ChatGPT, Copilot, Gemini, etc).  Please share your desktop, so we can see both the code you are writing and anything you are researching online.

You should think of the interviewer as a partner in a pair programming situation or as a senior engineer/PM who knows the customer requirements. Definitely ask any clarifying questions, bounce ideas off, and share what you’re doing.

The purpose of this problem is so we can get some insights into your thought process, how you work, and other such traits, and is not strictly focused on a working solution.


## Details 
The input is formatted as shown below, with 4 properties per row (id, name, city, and state):

```
id=123,name=Sean Williams,city=Portland,state=Oregon
id=354,name=Beatrix Strong,city=Eugene,state=Oregon
id=189,name=Sachin Dixit,city=Atlanta,state=Georgia
id=123,name=Sean Williams,city=Portland,state=Oregon
id=10267,name=Richard Albe,city=Miami,state=Florida
id=46235,name=Dorothy Cline,city=Portland,state=Oregon
```
The output file should be grouped and sorted using this hierarchy:

By state

Then by city

Finally, by name (with id).

For example, for the above input, the output would be:


```
===Florida===
-Miami-
Richard Albe[10267]
===Georgia===
-Atlanta-
Sachin Dixit[189]
===Oregon===
-Eugene-
Beatrix Strong[354]
-Portland-
Dorothy Cline[46235]
Sean Williams[123]
```
Note that Florida is the first state alphabetically (coming from line 5), and is thus the first line of output

For the Oregon records, not that the cities are printed in alphabetical order, and then the names + ids are output.

