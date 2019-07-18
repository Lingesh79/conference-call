# conference-call
Three people conference call implementation in java using networking concept.

INTRODUCTION

A conference call is a telephonic call in which someone talks to several people at the same time. The conference calls may be designed to allow the called party to participate during the call, or the call may be set up so that the called party merely listens into the call and cannot speak. It is sometimes called ATC (audio tele-conference).

OBJECTIVE

Conference call are an excellent working tool. It not only brings together people from different parts of the world, but can also save a ton of phone calls and long emails, in which everyone can understand what they want.

When handled efficiently, conference calls provide a great opportunity for raising ideas and reaching clear-cut decisions. The problem is that conference calls are seldom handled efficiently. Most times, they don’t start on schedule, they’re managed poorly, there are too many technical problems, and every participant talks about whatever he or she wants, for as long as they want.

IMPLEMENTATION

We have considered three systems one acts as Server while other two acts as Clients. Each system uses 2 ports for effective communication.

Server starts and waits for other 2 clients to get connected.

Each client sends connect packet to server and waits for reply.

Server after receiving connect packets from both the client,sends the IP address of clients as reply.

Example: Consider A and B are two clients. Both clients sends packet to server S. once Server S receives connect packets it will send IP address of A to B and IP address of B to A as a reply.

Once clients receives reply packet all systems starts audio channel to receive and send audio data.

We have used three threads in each system,
o First thread to receive audio packets from system 1.
o Second thread to receive audio packets from system 2.
o Third thread to send audio packets to both system 1 and system 2.

We have used UDP packets for communication between the systems.

Once the call is disconnected all three systems will have the audio record saved in .wav format.

User has an option to play the audio once the call is disconnected.

CONCLUSION

This Conference call system allows users to communicate in a LAN without internet. Reduces Data charges. Helps a project committee or
other department in a company to communicate with their colleagues.

Helps in organizing meetings in a company. Hence it will be useful in many of the company.Since every company has WIFI / ETHERNET facilities all the systems will be connected in a LAN. Hence it is easy to organize conference meeting within minimum time.
