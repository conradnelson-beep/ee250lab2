# ee250lab2

# Conrad Nelson - conradnelson-beep
# Aava Abedinpour - abedinpo-cmd

Question 1: How did the reliability of UDP change when you added 50% loss to your local
environment? Why did this occur?

Half of the inputs we sent would not be received. This is because the packets with that information were lost. 

Question 2: How did the reliability of TCP change? Why did this occur?

TCP's reliability did not change, because the packets are numbered and will be re-sent if they are not received. 

Question 3: How did the speed of the TCP response change? Why might this happen?

There was a small delay with the TCP response, because the packets that were lost had to be re-sent. 

Question 4: If you used LLMs for any part of this lab, explain how you used it. 

We used the included python sockets tutorial to write the tcp_client.py file, but when we tried compiling and running the file in terminal we received an error telling us that the port was already in use. ChatGPT said that the client was actually another server, and helped us debug our code to get the client to function properly.

1. What is argc and *argv[]?
   Argc is the integer counting the number of arguments inputted. *argv[] is the array holding each word used as argument. It can be dereferenced again to sift through individual characters inputted.

2. What is a UNIX file descriptor and file descriptor table?
The file descriptor is an indicator (small non-negative integer) used to access a file. The file descriptor table is a table that maps file descriptors to entries in the system-wide open file table.

3. What is a struct? What's the structure of sockaddr_in?
 A struct is an object that allows you to combine many different data types into one variable. sockaddr_in combines the server and client addresses as well as their respective data members.

4. What are the input parameters and return value of socket()
 The input parameters are AF_INET, SOCK_STREAM, and 0.
The return value of the socket() function can be a socket file descriptor (if successful), and -1 if unsuccessful (ie an error occurs).

5. What are the input parameters of bind() and listen()?
   The input parameters of bind() are sockfd, and a reference to serv_addr. The input parameters of listen() are sockfd and 5.

6.  Why use while(1)? Based on the code below, what problems might occur if there are multiple simultaneous connections to handle?
   while(1) lets the server handle clients repeatedly without quitting after only one. A problem that might occur would be if one client is very slow, all clients will suffer since only one client is handled at a time.

7. Research how the command fork() works. How can it be applied here to better handle multiple connections?
   Fork() creates another process that is done side-by-side with the original process. It could be used here to allow multiple clients' requests to be processed at once.

This program makes several system calls such as 'bind', and 'listen.' What exactly is a system call?
A system call is a call that requests a service from the OS kernel. 
