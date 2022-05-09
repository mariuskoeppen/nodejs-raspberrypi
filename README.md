# How to install Node.js on a raspberry pi

1. Figure out what system architecture you're running on by typing `arch` into the console. 
2. Find the version you want to use at [the official Node.js download page](https://nodejs.org/en/download/current/). You might need to click on _All download options_. Grab the corresponding `.tar.xz`-Link, e.g. `https://nodejs.org/dist/v18.1.0/node-v18.1.0-linux-arm64.tar.xz`. 
3. Download the package: `curl -o node18.tar.xz https://nodejs.org/dist/v18.1.0/node-v18.1.0-linux-arm64.tar.xz`.
4. Extract the package `tar xvf node18.tar.xz`.
5. Navigate into the newly created folder by `cd [name of folder]`. If you don't know the name of the folder type `ls`. 
6. Execute the following commands line by line: 
```
sudo cp -R bin/* /usr/bin/
sudo cp -R lib/* /usr/lib/
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install build-essential
```
7. Run `node -v` to check if it worked. 
