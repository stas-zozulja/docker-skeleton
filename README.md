Basic configuration/setup for Dockerized Symfony development

### Setup

1. Add network interface alias for xDebug:

    In Mac:
    ```sudo ifconfig en0 alias 10.254.254.254 255.255.255.0```
    
    In Linux:
    ```sudo ip addr add 10.254.254.254/24 brd + dev eth0 label eth0:1```

    where `eth0` is local network interface

2. Build and run containers:

    ```bash
    docker-compose build
    ...
    docker-compose up -d
    ```
    