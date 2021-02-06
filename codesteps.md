## Code Steps

### Prerequisite Steps

 - install touch for adding files   
   `npm install touch-cli -g` 

### Project Steps

- create folder project  
  `mkdir project-name`

- initialize default settings  
  `npm init -y`

- Set Up Express 
  `npm i express`

- create the entry point of the application
  `touch index.js`

- Add Code 
```javascript
const express = require("express");
const path = require("path");

const app = express();
const port = process.env.PORT || "8000";


app.get("/", (req, res) => {
    res.status(200).send("Test Test Test");
  });


  app.listen(port, () => {
    console.log(`Listening to requests on http://localhost:${port}`);
  });
```

- configure npm start
`"start":"node src/app"`

 - install mgeneratejs  
   `npm install -g mgeneratejs`

 - add template.json file  
 ```javascript
 {"name": "$name", "age": "$age", "emails": {"$array": {"of": "$email", "number": 3}}}
 ```

 