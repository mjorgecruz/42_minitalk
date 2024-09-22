# 42_minitalk

The purpose of this project is to code a small data exchange program using UNIX signals.</br></br>

A message is written on the client that must then send the string passed as a parameter to the server.</br>
Once the string has been received, the server must print it. </br>
</br>
The message is encoded in its binary code and then sent between two processes using the SIGUSR1 and SIGUSR2 signals.</br></br>
`signal.h` library is used to send and interpret signals on client and server side.

## How to run

1. Clone repository
    ```bash
    git clone git@github.com:mjorgecruz/42_minitalk.git
    ```

2. Go inside project directory and run `make`
    ```bash
    cd 42_minitalk
    make
    ```
3. Open one terminal and run `./server`. The pid of the process should appear on the terminal output.
     ```bash
    ./server 
    ```
4.  Open another terminal and run `./client {server_PID} {MESSAGE}`.
     ```bash
    ./server 10254 "This is my minitalk"
    ```
</br>
