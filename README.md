# 1RickZeta7

#concept
A digital licensing platform that encourages collaboration between creators.

#getting DB setup
I recommend creating a keys_dev.js file in the config file the file should follow the format below
module.exports = {
    mongoURI: 'mongodb://<dbuser>:<dbuser>.mlab.com:56789/mydb',
    secretOrKey: 'secret'
  };

----------------------------------------------------------------------------
also create a keys.js file with the following script:

if(process.env.NODE_ENV === 'production') {
  module.exports = require('./keys_prod');
} else {
  module.exports = require('./keys_dev');
}

#getting the repo running
first run npm i in both the root folder and in the client folder

To start the app from the command line execute " npm run dev "

#heroku live site
https://arcane-wildwood-54985.herokuapp.com/