# SOCKET.IO PLAY v0.0.1b
2015.JAN.11

###Change Log
2015.JAN.11: (v0.0.1b)
- adding serialport monitoring. (WIP)

Experimenting and documenting SOCKET.IO.

Tutorials:
[Lynda.com Node.JS Essential Training](http://www.lynda.com/Node-js-tutorials/Creating-WebSockets-Socket-IO/417077/454470-4.html)

### Basic Workflow
- bring in Express module
- bring in HTTP module
- create main application with ```app = express()```
- create http server, but instead of a port, pass in your application and chain the ```.listen(3000)``` with port 3000.
```var server = http.createServer(app).listen(3000)```
- create socket.io connection with ``` var io = require('socket.io')(server);```.  It's actually a function, so pass in your server here.

- host static files with express middleware using ```app.use(express.static("./public/");```
- setup listener with ```io.on('connection', function(socket) { socket.emit('message'});```

- NOTE: we don't send anything like websockets, we're "emitting" messages.

(( CONTINUE HERE ))

### Socket.IO
- requires 'http' module (no longer creates one on it's own)


### More Links

