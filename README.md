This repository contains variouse of Docker images with network tools for Docekr and Kubernetes network trobleshooting. it was inpired by:
* https://github.com/Praqma/Network-MultiTool
* https://github.com/raesene/alpine-nettools

**Table of Content**
- [Minimal Alpine Image](#Minimal-Alpine-Image)
- [Network-Multitool](#Network-Multitool)
- [netshoot: a Docker + Kubernetes network trouble-shooting swiss-army container](#netshoot-a-Docker--Kubernetes-network-trouble-shooting-swiss-army-container)

# Minimal Alpine Image
Build on with latest alpine image.
Includes: `ind-tools, net-tools, curl`

**build**
```bash
docker build  -t  net-tool-mini:1.0.0-alpine alpine_small_image
```
**use** 
```bash
docker run -ti net-tool-mini:1.0.0-alpine
```
or
```bash
docker run -ti robertwol/net-tool-mini
```

# Network-Multitool
Inspired by 
https://github.com/Praqma/Network-MultiTool
**Tools included:**
* apk package manager
* Nginx Web Server (port 80, port 443)
* wget, curl, iperf3
* dig, nslookup
* ip, ifconfig, mii-tool, route
* ping, nmap, arp, arping
* awk, sed, grep, cut, diff, wc, find, vi editor
* netstat, ss
* gzip, cpio
* tcpdump
* telnet client, ssh client, ftp client, rsync
* traceroute, tracepath, mtr
* netcat (nc), socat
* jq
* git

# netshoot: a Docker + Kubernetes network trouble-shooting swiss-army container
