### Node & NPM
- Node: Allows developers to write and run JavaScript applications on the server. Developers started using node.js to also write tools to help them with **local web development**.
- NPM: Is a simple command line interface that allows developers to **install and manage packages** on their local computers. There are all kinds of open-source **tools, libraries and frameworks** needed for moder development. Modern web development could simply not exist without a package manager.

##### Install Tools
In order to install required tools in our project, first we need to create our `package.json` file, for that we need to execute `npm init`
- sass: `npm install node-sass --save-dev`

For example if we need a dependency for the project:
- jquery: `npm install jquery --save`
- jquery: `npm uninstall jquery --save`

For using `sass` once installed, we will need to add a script in `package.json` as follows:

```json
{
  "name": "magical-nature",
  "version": "1.0.0",
  "description": "Landing page for Magical-Nature",
  "main": "index.js",
  "scripts": {
    "compile:sass": "node-sass sass/main.scss css/style.css"
  },
  "author": "Franco Arratia",
  "license": "ISC",
  "devDependencies": {
    "node-sass": "^4.14.1"
  }
}
```
This can be executed as: `npm run compile:sass`. For keep watching we would need to have: `"compile:sass": "node-sass sass/main.scss css/style.css -w"`

- Live-Server: `npm install live-server -g` This we need to install globally, that is why it does not have --save or --save-dev. Since this is installed globally we can call it from the command line.

Command is: First go to the folder where your index.html is located then `live-server`

###### Note:
- --save-dev: is `dev` dependencies that is used as a developer tool for development.
- --save: is a dependency that the project needs.


##### 7-1 Pattern
- abstracts
- base
- components
- layout
- pages
- themes
- vendors

