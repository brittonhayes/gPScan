
![Logo](https://i.postimg.cc/N07v7BTq/white-gp-Scan-Thumb.png)


[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
[![GitHub tag (latest SemVer)](https://img.shields.io/github/tag/alexpfaller/gPScan)](https://github.com/alexpfaller/gPScan)
[![made-with-Go](https://img.shields.io/badge/Made%20with-Go-1f425f.svg)](https://go.dev/)
[![GoDoc reference example](https://img.shields.io/badge/godoc-reference-blue.svg)](https://godoc.org/github.com/alexpfaller/gPScan/cmd/gpscan)


# gPScan

gPScan is a simple CLI tool, to check if specific ports are opened or closed.



## Installation

To install/ build the binary, make sure that you have installed the go compiler.

```bash
  git clone https://github.com/alexpfaller/gPScan
  cd gPScan
```
```bash
  sudo make build
```
This will build the gPScan binary in your /bin/ directory.
    
## Usage

It always follows this schema, where you first specify one of the two protocols (tcp, udp), after that you can insert your destination, which you want to check for open ports(localhost, any IP address). Last but not least, append the port that should be checked.
```sh
gpscan <protocol> <destination> <port>
```

Example:
```sh
gpscan tcp localhost 8080
```
To check if port 8080 on your machine is currently open, or closed.
```sh
gpscan tcp 132.203.220.211 443
```
To check if port 443 (https) on another machine is open.
