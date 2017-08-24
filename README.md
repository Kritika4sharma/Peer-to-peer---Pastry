Skynet-P2P File Sharing

Packages(in Python) Required :
1. ipaddress
2. netifaces
3. recordtype 
4. pytftlib.handlers 
5. pysendfile 

For running the software :
1. Go to the folder "persistence".In file persist.py, set the free port where persistence will listen. 
2. Type "python persist.py". This will run the persistence.
3. Now open a new terminal and change the directory to the project directory where master.py file is present.
4. Type "python master.py master_port". Here master_port is argument for the port where client and server will listen.
5. To run server, type "python server.py server_port peer_forward_port peer_backward_port client_forward_port client_backward_port master_port".
6. Change the ports in file Client.py, setting self.MASTER_SERVER_PORT = master_port and self.TIER_TWO_SERVER_PORT = server_port as passed in arguments in previous two commands.
7. For uploading : Type "python new_client.py --upload file_name"
8. For downloading : Type "python new_client.py --download file_name"
