TO RUN THE SERVER

Run the server from the command line and provide the port for the server, ex. 10007
//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////


TO RUN THE CLIENT

Run the server from the command line and provide:
-the IP address of the server
-the port in which the server is listening for connections.

ex. for a client running in the same machine as the server in port 10007 provide:
127.0.0.1 10007



//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

ABOUT MESSAGE CLASS:

Application protocols:



Broadcast 	>>>> this could be either a message for everyone or an update of user connected. We can check if it is either of the two by looking at the array in the message object if it is empty or not
PrivateChat	>>>> just private chat
Login		>>>> when a client wants to log in
Register	>>>> for registration
Confirmation    >>>> if registration or log in has been successfull, server responds this to the client



confirmation types

Success		//when user could make a registration or login
Fail		//when a user could not make a registration
Fail0		//when trying to login but user and passwortd NOT OK
Fail2		//when trying to login but user OK and password NOT OK
Fail3		//when a loged in user tries to log in again