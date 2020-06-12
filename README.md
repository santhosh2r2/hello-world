# Instruction

## exports from module
```
greeting = "Hi from Santhosh!"
```

Example using express-js

```
mkdir test-app && cd test-app
npm install express @santhosh2r2/hello-world --save
touch index.js
## copy the contents of index.js
node index.js
```

`navigate to http://localhost:3000`

## contents of index.js

```
const express = require("express");
const helihalo = require("@santhosh2r2/hello-world");

var app = express();

app.get("/", function (req, res) {
  res.send(helihalo.greeting);
});

app.listen(3000, function () {
  console.log("Server started at port 3000");
});

```
