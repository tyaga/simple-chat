# simple-chat
cool simple little chat server I made for telnet/nc, client included for op timestamps :)

**Running on aubble.com:444, connect with telnet/nc or the provided client**

## Install

The commands will install into $GOPATH/bin, just make sure you have it in your $PATH.

Otherwise navigate to $GOPATH/github.com/nhooyr/simple-chat and build from source.

### cserver

	go get github.com/nhooyr/simple-chat/cserver

Run, log to stderr with timestamps and listen on ip:port (can be shortened to just port)

	cserver -e -t -l ip:port

See all options with

	cserver -h

### cclient
First of all the client is unnecessary, you can use telnet/netcat. It's only advantage is that it comes with timestamps and its very straightforward.

	go get github.com/nhooyr/simple-chat/cclient

Run and connect to host:port (can be just port)

	cclient host:port

#### Help

Once connected via a client, type /help to see help on the different commands you can use on the server.
