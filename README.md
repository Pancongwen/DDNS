# DDNS

This is a project show you how to install no-ip ddns client on ubuntu server

## Preparation
### Topology
    ```
    ___________________________        ______________
    |                           |      |              |  
    |                           |      |              | 
    |     ubutnu server    WAN  +------+ LAN  ISP 1   |
    |                           |      |              |
    |___________________________|      |______________|
                                    
    ```

### Sign in NO-IP
Sign in [NO-IP](https://www.noip.com/) and get a free domain


## Install client on ubuntu server

### clone the code 
    ```
    $ git clone https://github.com/LaoLuMian/DDNS.git
    ```


## conf: the name of you configure (without .conf)

### config 
    ```
    $ cd DDNS
    $ ./DDNS-control config [conf]
    ```

### clean 
    ```
    $ cd DDNS
    $ ./DDNS-control clean [conf]
    ```

### start ddns
    ```
    $ cd DDNS
    $ ./DDNS-control start [conf]
    ```
    
### stop ddns
    ```
    $ cd DDNS
    $ ./DDNS-control stop [conf]
    ```
    
### check the status
    ```
    $ cd DDNS
    $ ./DDNS-control status 
    ```
    