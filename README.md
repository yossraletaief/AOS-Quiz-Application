# AOS-Quiz
Quiz Application built using RPC supporting multiple clients and failure recovery.

The server has a list of 50 random questions. A client probes the server and server replies with a random question. On correct answer, the client is awarded one point and zero on wrong reply. A client can ask for server as many times as he wants and server replies with one question each time. There are other clients also requesting the server and are handled in same manner. A client can ask its score and its relative position amongst other clients. A client can go down and can recover. After recovery, it starts with the score it has gained before fault. Once the client wants to finish, it is allowed to exit at any stage. 
