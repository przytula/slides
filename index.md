---
title       : DB2 interactive learning 
subtitle    : An interactive course to become a DB2 for LUW Database Administrator
author      : Guy Przytula
job         : Consultant 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [bootstrap, quiz]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
--- bg:ibm-db2.png

## Enable connectivity  for your instance

1. Update dbm cfg using svcename 50001   (or any port you want DB2 to listen on)
2. db2set comm=tcpip     (to enable the listener for tcpip)
3. db2stop - db2start to read these settings and create the listener

--- .class #id 

## Number of customers using DB2 in Belgium

<!-- html table generated in R 3.1.1 by xtable 1.7-3 package -->
<!-- Sat Aug 16 10:10:54 2014 -->
<TABLE class:mytable>
<TR> <TH>  </TH> <TH> year </TH> <TH> cust </TH>  </TR>
  <TR> <TD align="right"> 1 </TD> <TD> 2000 </TD> <TD> 100 </TD> </TR>
  <TR> <TD align="right"> 2 </TD> <TD> 2001 </TD> <TD> 200 </TD> </TR>
  <TR> <TD align="right"> 3 </TD> <TD> 2002 </TD> <TD> 300 </TD> </TR>
  <TR> <TD align="right"> 4 </TD> <TD> 2003 </TD> <TD> 400 </TD> </TR>
  <TR> <TD align="right"> 5 </TD> <TD> 2004 </TD> <TD> 500 </TD> </TR>
   </TABLE>

---

![plot of chunk unnamed-chunk-2](assets/fig/unnamed-chunk-2.png) 

--- &radio
## Question 1

What is SVCENAME ?

1. database configuration setting services
2. _database manager setting the port for this instance or symbolic name translated in etc/services_

*** .hint
There is only port used by the instance

*** .explanation
SVCENAME is a dbm config setting specifyng the port number the instance is listening on




