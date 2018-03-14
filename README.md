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
