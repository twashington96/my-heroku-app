# my-heroku-app README

# Dev Lab BETA/486 Story Card 

## User Story (Story Points = med👕) 

**As a** user

**I want** Use the `NodeJS` application online

**So That** I dont have to take unnecessary steps to download code, etc.

## Step-by-step

### Create Project
1. Open `vsCode`
2. Open project folder in vsCode.  File >> Open folder, or drag project folder on desktop to vsCode
3. Open Command Palette View >> Command Palette or `ctrl+shift+p` >> type "Select Default Profile"

### Code
1. Create file for project.  File >> New file from menu
2. Verify the current terminal directory. Open new terminal: `ctrl+shift+~`
3. Initialize project.  At terminal type: `npm init`.
4. Copy and paste the code below into `index.js` file.

```
const express = require('express');
const app = express();

app.get('/', function(req, res){

    res.send('<h3>Hello NodeJs on Heroku</h3>');
});
app.listen(process.env.PORT || 3000);
```

## Test App
1. Open terminal Terminal >> New Terminal, or `ctrl+shift+~`. 
1. Start nodejs server.  Type `node (filename).js`
1. Open web browser (Chrome preferably).  In your address bar type: "localhost:3000 

## Heroku
1. Create a [Heroku account](https://www.heroku.com/).
2. Create new app.
3. Select a name for your app. (Names limited. Use unique identifier)
4. Hit the purple **`Create App`** button
5. Select **`Connect with GitHub`**
6. Select your GitHub repository.
7. Select **`Automatic Deploy`**
8. Select **`Deploy Branch`**
9. DONE!


