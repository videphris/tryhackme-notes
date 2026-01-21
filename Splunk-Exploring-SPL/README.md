**Date:** 2021/1/21
**Room URL / ID:** https://tryhackme.com/room/splunkexploringspl
**Goal / Objective:**  
Learn how to utilize search processing language (SPL) for Splunk log queries.

### Quick TL;DR
One sentence summary of what I did or found.
Used various techniques, operators and filters to narrow down the data to what we are looking for to be more effective.

### Key commands
index must always be pronounced in the beginning.
index=windowslogs | chart count by User
index=windowslogs | highlight User, host, EventID, Image
index=windowslogs EventID="1" AND User="Cybertees\\James"

### What confused me / slowed me down
Learning the syntax, NEED to make sure capitals are in place as the values are case sensitive

### Key takeaway
One thing to remember next time.
Keep going strong, try to think through the issue before looking at external documents.
