# Reverse Shell

## Intro
A shell which can access information from any remote server, using shell commands. The interface looks like a bash terminal virtually running on your PC, although everything that is displayed is the content of the server.

## Usage
### Server Side
Run `server.py` in the background. It will create a socket server and will be listening to the port 9999 by default. It stores all output from client into a file and also echo it onto the terminal on the go.

### Client Side
Now you need to run the file `client.py` in the device you want to control. On running it for the first time, a request will be sent to the server running on your machine. The server will acknowledge that request and will respond with bash commands you enter in the shell. The client will respond back with the STDOUT or the STDERR.
