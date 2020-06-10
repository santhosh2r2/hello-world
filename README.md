# Instruction

```
greeting = "Hi from Santhosh!"
```

Example using express-js

```
const express = require("express");
const bodyParser = require("body-parser");
const helihalo = require("@santhosh2r2/hello-world");

var app = express();
app.use(bodyParser.urlencoded({ extended: true }));

app.get("/", function (req, res) {
  res.send(helihalo.greeting);
});

app.listen(3000, function () {
  console.log("Server started at port 3000");
});

```
