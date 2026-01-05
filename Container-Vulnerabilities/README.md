**Date:** 1/5/26
**Room URL / ID:** https://tryhackme.com/room/containervulnerabilitiesDG

**Goal / Objective:**  
Learned how containers are vulnerable when they get kernal access of the host system using various techniques.

### Quick TL;DR
One sentence summary of what I did or found.
Sockets are how processes interact with each other on Linux and is how the docker engine talks to the host operating system and the containers.

### Key commands
Anything worth keeping.
nsenter - allows use to execute or start processes and place them as the same namespace as another.
Processes on linux have a parent child relationship and derive from the last. Process one is the first userspace process started by the Linux kernal. It's the parent of all other processses. It starts services, handles shutdown and signals, keeps the system alive and reaps orphaned processes. 
It should always be up unless the system dies. PID might be "init" or "upstart"

### What confused me / slowed me down
Overall knowledge of linux systems

### Key takeaway
One thing to remember next time.
Containerization can be vulnerable if misconfigured and not following the best security practices.
