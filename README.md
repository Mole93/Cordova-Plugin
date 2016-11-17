# Cordova Plugin how to create it

Step to create a Cordova plugin and publish it in the community.

I spend few days to understand how I can create an publish an plugin on Cordova, because all tutorials online were not updated, this is the region because i  create this guide.

## You need to know
**Cordova decided that from CLI 5.0.0 all plugins have to migrate on [NPM website](https://www.npmjs.com/)** 

# Steps

## Step 1
 Go to [NPM website](https://www.npmjs.com/) and create an user, it will be the user that you will use to publish your plugin.

## Step 2 
Check if in your computer was installed `plugman`, if it wasn't installed you need to install it so you need to run the following code snippet to install plugman.

    npm install -g plugman

## Step 3 - Create plugin with plugman
To show you how to create an Cordova plugin using plugman

    plugman create --name [plugin_name] --plugin_id [plugin_id] --plugin_version [plugin_version] --path [local_path]

after you need to add the platform to your plugin

    plugman platform add [platform]

So after you need to create all logic that you need.

## Step 4 
You need to create the packege json 

    plugman createpackagejson [PLUGIN DIRECTORY]

## Step 5 adduser and publish

You need to add your user to publish the plugin so you need to ran the following code snippet

     npm adduser
after you can publish your plugin 

     npm publish [PLUGIN DIRECTORY]

So now your plugin can be installed with the following code snippet

    cordova plugin add [plugin_id]
