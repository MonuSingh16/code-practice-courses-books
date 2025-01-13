### L2. 13-Jan-2024

1. Model OSI - Open system internet. It has 7 layers. 
    a. Physical layer - on the 0 and 1
    b. data link layer - frames. (IP address, HTTP Headers, etc)
    c. Network layer - Routing, - IP Addressing
    d. Transport layer - TCP / UDP
    e. Session layer
    f. Presentation layer
    g. Application layer

2. TCP / UDP - When the data is transferred using some protocol. TCP - Transmission control protocol - it is *reliable, ordered, 3-way handshake*

        client <---> Server

TCP ensures all the packet are received, ordered. Client gives a sequence number, then we send a sync mesage to server. Like sync-1. Server will also send a sync-200 message, and also acknowledgement of ack-1.Client will also ack the server sync-200 message  ack-200

sycn , sync+ack, ack  ~ Handshake

What is overhead in TCP ? - 3 way handshake, then data sent, preprocess by arranging the packets. This leads to latency. Reliability is high, while Time is down. Ex - Video Call will have delay

UDP - delay will drop, while reliability will drop due to loss in packets until all packets arrive

Live cricket matches - TCP.
Live Video - UDP
Youtube Live - TCP
Chat - TCP

3. HTTP - HyperText Transfer Protocol - Works on application layer, while the data moves on transport layer. version 1 - whenever you want to transfer then you want 3 way handshake. 1.1 - Only 1 time sync requires, during the session.

4. IP Address - Browser request goes to DNS Server via DNS Resolutio, to fetch the IP address of the 'google.com'. The communication will be routed to the IP Address. One domain will point to one one address.

If you buy a domain from a website.

    Browser ---> DNS Server ---> Root Name Server 
    chaicode.com ----------          --------- (Top level server - returns the domain name of the TLD, .ai, .com, .uk, etc)
    a. First return th ip address of the .com server
    b. Now using the .com server try to fetch the using ANS - authorative name server, like the server where this url was bought from
    c. DNS works on the UDP Protocol Port Number:53,

dig <chaicode.com>

Also browser keeps some cache, so it does not have to do DNS resolution again and again.

5. What is pipelining 