# Peer-to-Peer-Network-with-Centralized-Index
Server-Client Infrastructure with the server managing clients using a Centralized Index with basic functionality of Peer-to-Peer Distributed Index File Transfer Protocol(P2P-DI) using TCP/IP and Socket programming. A concurrent server to increase the scalability of the network.
How to Run
1. Start the Server: In the root directory, run the "server.py" file to start the server application. 
     	Command:    python server.py

2. Simulate Clients:"client.py" starts an application for one client. To run mulpiple clients, Create multiple client directories 
		     and copy "client.py" into the directory and run it to start client application. Each client will ahve its own storage space 
		     The Server Host to whcih the client connects by default will be localhost ie '127.0.0.1'
		 		
	Command:    python client.py [server host]
If the server is running on AWS, input it's public IP as server host. For example, if you have a Linux instance running on 13.25.100.100, run like this:
	python client.py 13.25.100.100		

3. RFC_LIST: Once you run "client.py" file it will generate and empty directory 'RFC_LIST' to store it's RFC files.
	     Place several RFC files under this directory for each client.
	     Note that this means that the client has only those RFCs in its local which are present in its corresponding "RFC_List" folder. 

4. Command Line Interface: At server's CLI, recieved requests and the server's status will be shown. No inputs are accepted.
			   At client's end, An operation menu for the client to interact with will be shown. Enter/Choose the service of your chioce

