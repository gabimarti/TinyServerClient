# TinyServerClient
Small (tiny) tcp server and client for testing.

This repository contains only two files:

    * tinyserver.py - Small multi-threaded server, with configurable port, number of clients, 
                      buffer size, and message to receive that kills the process.
                      
    * tinyclient.py - Client to use with tinyserver.py and to be able to do communication tests. 
                      It also allows you to configure the host, port and message to send.
      

These modules have been used for the execution of tests of another project that is currently underway (August / 2019), and is not finished.

Please feel free to contact me if you wish to make any suggestions or send me any comments.

If you use this code or part of it for any project of yours, I would like to hear from it.

I will be glad to know that it has been useful to you.


# Usage
There is no gui, all by command line. Different parameters can be passed, but without parameters it also works because it has set default values.

    usage: tinyserver.py [-h] [-i INTERFACEBIND] [-c MAXCLIENTS] [-p SERVERPORT]
                         [-b BUFFERSIZE] [-k KILLMESSAGE] [-v {0,1,2}]
       
    optional arguments:
      -h, --help            show this help message and exit
      -i INTERFACEBIND, --interfacebind INTERFACEBIND
                            What interface is it linked to? Default (empty) to any
                            of this host.
      -c MAXCLIENTS, --maxclients MAXCLIENTS
                            Indicates the maximum number of clients/threads.
                            Default value: 10
      -p SERVERPORT, --serverport SERVERPORT
                            Port to listen. Default value: 6666
      -b BUFFERSIZE, --buffersize BUFFERSIZE
                            Buffer size. Default value: 4096
      -k KILLMESSAGE, --killmessage KILLMESSAGE
                            Message to kill server. Default value: 'kill'
      -v {0,1,2}, --verbose {0,1,2}
                            Increase output verbosity. Default value: 1
    
    
    usage: tinyclient.py [-h] [-s HOSTSERVER] [-p PORT] [-b BUFFERSIZE]
                         [-m MESSAGE] [-v {0,1,2}]
       
    optional arguments:
      -h, --help            show this help message and exit
      -s HOSTSERVER, --hostserver HOSTSERVER
                            Host to connect. Default 127.0.0.1
      -p PORT, --port PORT  Port to connect. Default value: 6666
      -b BUFFERSIZE, --buffersize BUFFERSIZE
                            Buffer size. Default value: 4096
      -m MESSAGE, --message MESSAGE
                            Message to send to the server. Default value: 'kill'
      -v {0,1,2}, --verbose {0,1,2}
                            Increase output verbosity. Default value: 1



# References
Part of the creation of this code has been inspired by the publication of the following blog by Daniel Hnyk (@hnykda).

http://danielhnyk.cz/simple-server-client-aplication-python-3/


# Contact
email: gabimarti (at) gmail (dot) com

twitter: @gmarti
                