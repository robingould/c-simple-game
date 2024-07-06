lean client server guess my number game in c, part of Systems Programming course at UConn

important files: 
1. `server.c`: serverside impl
2. `client.c`: clientside impl
3. `socketio.c`: socket I/O helper functions.

to compile just run 
```
make 
```

to run the server
```
./server
```

then, in a seperate terminal run the client
```
./client [hostname]
```
where `[hostname]` is the IP address of the server

how the game works:
- server generates a random number between 1 and 1000.
- client tries to guess.
- on each guess the server either responds with 1 if too low, or -1 if too high (to indicate go up or go down)
- if the guess is correct, 0 is returned by the server
- the game continues until the correect number is guessed, and the amount of guesses made are sent to the client

