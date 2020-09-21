# qBittorrent Client 

Node.js client for qBittorrent

## Requirements

At this time, this has only been partially tested with version 4.2.0 alpha of the qbittorrent-nox. 

## Installation

If you have the node package manager, npm, installed:

```shell
npm install --save qbittorrent-client
```

## Getting Started
Examples below.
###getTorrents
```coffee-script
qBittorrent  = require('qbittorrent-client').API4

client = new qBittorrent
  username: 'admin'
  password: 'adminadmin'
  proto: 'http'
  host: 'localhost'
  port: 8080
    
client.getTorrents (err, torrents) ->
  console.log err if err
  console.log torrents if torrents
```
