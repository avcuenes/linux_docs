# xhost command

Controls who accesses Enhanced X-Windows on the current host machine.The xhost command adds or deletes host names on the list of machines from which the X Server accepts connections.

 xhost - server access control program for X .
The xhost program is used to add and delete host names or user names to the list allowed to make connections to the X server. In the case of hosts, this provides a rudimentary form of privacy control and security. It is only sufficient for a workstation (single user) environment, although it does limit the worst abuses. Environments which require more sophisticated measures should implement the user-based mechanism or use the hooks in the protocol for passing other authentication data to the server. 



## Options
Xhost accepts the following command line options described below. For security, the options that affect access control may only be run from the "controlling host". For workstations, this is the same machine as the server. For X terminals, it is the login host.

-help
    Prints a usage message. 
[+]name
    The given name (the plus sign is optional) is added to the list allowed to connect to the X server. The name can be a host name or a user name. 
-name
    The given name is removed from the list of allowed to connect to the server. The name can be a host name or a user name. Existing connections are not broken, but new connection attempts will be denied. Note that the current machine is allowed to be removed; however, further connections (including attempts to add it back) will not be permitted. Resetting the server (thereby breaking all connections) is the only way to allow local connections again. 
+
    Access is granted to everyone, even if they aren't on the list (i.e., access control is turned off). 
-
    Access is restricted to only those on the list (i.e., access control is turned on). 
nothing
    If no command line arguments are given, a message indicating whether or not access control is currently enabled is printed, followed by the list of those allowed to connect. This is the only option that may be used from machines other than the controlling host.

## References
1.<https://www.ibm.com/docs/ru/aix/7.2?topic=x-xhost-command>
2.<https://linux.die.net/man/1/xhost>



