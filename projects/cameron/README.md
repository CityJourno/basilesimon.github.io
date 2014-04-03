The David Cameron paradox
========================

Both of these charts are based on API queries to BBC services for "David Cameron".
Two JSON files were returned, parsed and visualised with d3.js.

Despite coming from two almost identical queries, they present enormous differences. 
The version coming from the Linked Data Core shows a dominance of mentions by Birmingham and Football, while
the version coming from the Juicer presents what seems to be a more accurate portrait of PM's mentions by the BBC.

I reached our data architect for more explanations. 


Linked Data Core:
==================
![LDP](https://raw.github.com/basilesimon/d3experiments/master/Cameron%20queries/LDP.png)

The LDP is a journalist-tagging tool. For that reason, it has a high confidence. The problem is that its coverage and usage 
are limited at the moment to Birmingham local news, Business news and World news mostly. 


Juicer:
================
![Juicer](https://raw.github.com/basilesimon/d3experiments/master/Cameron%20queries/juicer.png)

The Juicer is a machine-tagging tool. We have a low confidence in its tag accuracy, but it has a high coverage of BBC News,
as it scrapes almost anything linked from our index.
