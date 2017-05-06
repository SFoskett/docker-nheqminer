# docker-nheqminer 0.4b  
This is a docker for nheqminer version 0.4b prior to the switch to AVX instructions (<https://github.com/nicehash/nheqminer>). It works well with nicehash and many other mining pools.

### Usage:  
    docker run -d sfoskett/nheqminer-0.4b /nheqminer -l <server:port> -u <user_address.worker>  

### Full example:  
    docker run -d sfoskett/nheqminer-0.4b /nheqminer -l zec.slushpool.com:4444 -u sfoskett.demo  

### More usage:  
Run `docker run sfoskett/nheqminer-0.4b /nheqminer -h` to to see options.  
After that, you can run `docker run sfoskett/nheqminer-0.4b /nheqminer [OPT...]` as you like.

### Docker Hub:

This docker is available at https://hub.docker.com/r/sfoskett/nheqminer-0.4b

