# Node and Express Start

## What do you need to start?

- Install Node

```sh
mkdir your_folder_name
cd your_folder_name
npm init
npm install express --save
```

Create app.js file and require expressJs:

```javascript
var express = require('express');
var app = express();
```

Define a server to respond the requests:

```javascript
var server = app.listen(4000, function(){
	var host = server.address().address;
	var port = server.address().port;
	console.log('Example app listening at http://%s:%s', host, port);
})
```

Set a root route:

```javascript
app.get('/', function(req, res){
	res.send('It works!');
})
```

Access your http://localhost:4000