# use-socket.io-client 
[![Build Status](https://travis-ci.org/iamgyz/use-socket.io-client.svg?branch=master)](https://travis-ci.org/iamgyz/use-socket.io-client.svg?branch=master)

React(^16.8.0) hook for socket.io-client, manipulate socket.io client without any side effect.

```javascript
import useSocket from 'use-socket.io-client';

const [socket] = useSocket('ws://localhost:8080',{
    autoConnect: false,
    //any other options
  });
  
//connect socket
socket.connect();

//add event
socket.on('message',(text)=>{
  console.log(text);
});

//emit
socket.emit('message','this is demo..');
```

## Installation

```
$ npm i use-socket.io-client
```
