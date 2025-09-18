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

