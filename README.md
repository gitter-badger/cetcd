# cetcd is a C client for etcd

## Status
 cetcd is on active development. It aims to be used in production environment and supply full features of etcd.
 *Any issues or pull requests are welcome!*

## Deps 
 cetcd use [sds](https://github.com/antirez/sds) as a dynamic string utility.  It is licensed in sds/LICENSE.
 sds is interaged in cetcd's source code, so you don't have to install it before.

 [yajl](https://github.com/lloyd/yajl) is a powerfull json stream parsing libaray. We use the stream apis to 
 parse response from cetcd

## Install
 cetcd parses json stream base on [yajl](https://github.com/lloyd/yajl), so you should install yajl first.

 then 
 ```
 make 
 make install
 ```
 It default installs to /usr/local.

 Use 
 ```
 make intall prefix=/path
 ```
 to specify your custom path.

## Link
 Use `-lcetcd` to link the library
