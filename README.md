# DDNS

This is a project show you how to install no-ip ddns client on ubuntu server

# Topology
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
```
$ ip route

ip route default scope link

nexthop dev ppp1 weight 1
nexthop dev ppp2 weight 2 

```

# How to use

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
