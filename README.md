# hget
![](https://i.gyazo.com/641166ab79e196e35d1a0ef3f9befd80.png)

Rocket fast download accelerator written in golang. Current program working in unix system only.

**NOTE** : hget is currently on highly development, its usage, architecture and code may change anytime at the future. It would be great if you can contribute whatever features that you want to use, I will take a look when have time.

**Build Status**: [![Build Status](https://travis-ci.org/huydx/hget.svg?branch=master)](https://travis-ci.org/huydx/hget)

## Install

```
$ go get github.com/huydx/hget
```

You can even `alias wget hget` to replace wget totally :P

## Usage

```
hget [Url] [-n parallel] [-skip-tls false] //to download url, with n connections, and not skip tls certificate
hget tasks //get interrupted tasks
hget resume [TaskName | URL] //to resume task
```

To interrupt any on-downloading process, just ctrl-c or ctrl-d at the middle of the download, hget will safely save your data and you will be able to resume later

### Download
![](https://i.gyazo.com/89009c7f02fea8cb4cbf07ee5b75da0a.gif)

### Resume
![](https://i.gyazo.com/caa69808f6377421cb2976f323768dc4.gif)
