#Socket Project: Pink Floyd
<img src="https://i1.sndcdn.com/artworks-000374202633-pqm4gy-t500x500.jpg" alt="The Dark Side Of The Moon" width="200"/>

![](https://img.shields.io/github/stars/pandao/editor.md.svg) ![](https://img.shields.io/github/forks/pandao/editor.md.svg) ![](https://img.shields.io/github/tag/pandao/editor.md.svg) ![](https://img.shields.io/github/release/pandao/editor.md.svg) ![](https://img.shields.io/github/issues/pandao/editor.md.svg) ![](https://img.shields.io/bower/v/editor.md.svg)


**Table of Contents**

[TOCM]

[TOC]

####ASIB Protocol
ASIB Protocol aka; **A**venged **S**evenfold **I**s **B**etter, is the protocol used for the communication between our client and server.
#####Command List:
| ID 	|  Requests  	| Description 	|
|:----------:	|:----------	|:-----------	|
|     200    	| ABMLIST    	| User gets the list of albums.|
|     207    	| SNGINABM   	| User inputs an albums name and gets its listed songs.|
|     214    	| SNGDUR     	| User inputs a songs name and gets its duration.|
|     221    	| SNGLYR     	| User inputs a songs name and gets its lyrics.|
|     228    	| ABMFROMSNG 	| User inputs a songs name and gets its associated album.|
|     235    	| SNGBYNAME  	| User inputs a word and gets all songs that includes that keyword (Case Insensitive)|
|     242    	| SNGBYLYR   	| User inputs a word and gets all songs that include the word in its lyrics (Case Insensitive)|
|     249    	| EXIT       	| End the conversation with the server.|
#####Requests format&pattern:
>Format `<CODE>:<REQUEST>&<DATA>`
>Regex `r'(\d{3}):([A-Z]+)(?:&(\w+(?: \w+)*))?'`

#####Server Response format&pattern:
>Format `OK:<RESPONSE>&<DATA>`
>Regex `r'OK:([A-Z]+)(?:&(\w+(?:.\w+)*))?'`

#####Server Error format&pattern:
>Format `<CODE>:ERROR:<TYPE>:<DATA>`
>Regex `r'(\d{3}):ERROR:([A-Z]+):(\w+(?: \w+)*)'`

------------------
<h2>Expect to see more soon...</h2> 
