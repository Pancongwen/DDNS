# DDNS

This is a project show you how to install no-ip ddns client on ubuntu server

## Preparation
### Topology
  ```
   ___________________________        ______________
  |                           |      |              |  
  |     ubutnu server    ppp1 +------+ LAN          |
  |                           |      |     ISP 1    |
  |                           |      |______________|
  |                           |       ______________
  |                           |      |              |  
  |                      ppp2 +------+ LAN          |
  |___________________________|      |     ISP 2    |
                                     |______________|
                                   
  ```

* ppp1 - PPPoE connection interface 
* ppp2 - PPPoE connection interface
* Load balance 

### Sign in NO-IP
Sign in [NO-IP](https://www.noip.com/) and get a free domain

## Install client on ubuntu server

### download packages
./download


### install no-ip client
./install

### start no-ip process
./start

### check whether active 
./status


### reconfig no-ip client
./reconfig


### uninstall no-ip client 
./uninstall
