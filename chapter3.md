# chapter3

# Multi-user DBMS Architectures
## Teleprocessing
* Traditional architecture for multi-user systems
* One computer with a single central processing unit (CPU) and a number of terminals
* Put a huge burden (包袱) on the central computer
## Downsizing
* Replacing expensive mainframe computers with more cost-effective networks of personal computers
## File-server architecture
* Processing is distributed about the network
* Multiple DBMSs can access the same files
### Three main disadvantages
* Large amount of network traffic
* Full copy of DBMS required on each workstation
* Concurrency, recovery, and integrity control are complex
## Traditional two-tier client–server architecture
* Client process requires some resource
* Server provides the resource
* Basic separation of four main components of business application
* Typical interaction between client and server
### Summary of client–server functions

![](https://github.com/yucing/database/blob/main/picture/s.png)