#Build a Resume With NodeJS

##Install NodeJS

1. `node -v` - To check the version of node

2. `sudo npm init -y` - For Installation

3. `sudo npm install express` - For install express

4. `sudo npm install path` - For Path (i don't know yet)


##Using the Express JS

1. we just grab the 2 line of code from express js for the express js documention

```
const express = require('express');
const app = express();
const path = require('path');
```

path is added last

copy paste the code inside the index.js file created at first using
			[x]. `touch index.js` 

2. Create the PORT first 

```
const PORT = process.env.PORT || 5000;
```

3. Check wheather it is working 

```
app.listen(PORT, () => console.log('Server is listening on port '+ PORT));
``` 


4. Make Directory for the templates to put it

[x] make direcory named `public` in side the main directory to set static folder 

[x] Add the following code inside the index.js file

```
app.use(express.static(path.join(__dirname, 'public')));
```
[x] Drop the downloaded template inside the `public` folder