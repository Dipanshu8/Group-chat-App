# Group-chat-App Usingh Socket Programming
A group chat application using MulticastSocket (Java Platform SE 7) class is discussed. 
A MulticastSocket is a (UDP) DatagramSocket, with additional capabilities for joining “groups” of other multicast hosts on the internet.

## Procedure
1) Save the file code.java and compile it using javac
2) Run the program using two command line arguments (multicast host and port number)
3) A multicast host is specified by a class D IP address and by a standard UDP port number. Class D IP addresses are in the range 224.0.0.0 to 239.255.255.255, inclusive. The address 224.0.0.0 is reserved and should not be used.

## Further Instructions
I have used the multicast host IP address as 239.0.0.0 and the port number as 1234 (since the port numbers 0 through 1023 are reserved).
If ther are 3 members in the group, start all three terminals first before sending the message, otherwise messages which are sent before starting the terminal are lost (since there is no facility of buffer incorporated to store the messages.)
We need two threads in this application. One for accepting the user input (using the java.util.Scanner class) and the other for reading the messages sent from other clients. Hence I have separated the thread which does the reading work into ReadThreadclass. For leaving the group, any of the user can type in Exit to terminate the session.
The above program is executed on a single machine. Socket programming is meant for distributed programming. The same piece of code snippet when present on different machines which have Java installed can satisfy that requirement. This is just the bare bones service logic

**Thankyou**
