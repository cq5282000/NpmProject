# NpmProject instruction

This project is a basic instruction about how to build and manage your front-end web application project through npm, webpack, react,and redux. All of these skills are necessary for you to become a good front-end engineer.It is only suitable for a beginner ,I have learned these skills in the first stage too.If there is something wrong with my blog ,welcome to point it out.

# Tools Installation 

## NPM installation

npm is a package management tools,first you should check whether you have installed the npm or not through:

```bash
# Linux & Mac
$ npm 
```

if not ,it will shows  'zsh: command not found : npm',then you must install npm first.
Install node.js and npm will be installed automatically, here are the steps.

- <a href="https://nodejs.org/en/download/">node.js</a> – click the link and download the node.js,install it
- `$ node -v` – test the version of the node.js that you installed ,the version should be higher than v0.10.32.
- `$ npm install npm@latest -g` – npm gets updated more frequently than Node does, so you'll want to make sure it's the latest version,update it through this command
- `npm -v` – test the version of npm ,The version should be higher than 2.1.8.

go through thses steps ,the npm will be installed

## How to use npm

Most of npm source is supported by the server running in foreign countries,it can be very slow if you install something by npm order directly, you need to change the source first:
 
```bash
$ npm config set registry https://registry.npm.taobao.org
```
here we use the taobao GHO,if you config it successfully ,test the order

```bash
$ npm config get registry
```

it will output 'https://registry.npm.taobao.org/', for more detailed information,

```bash
$ npm info express
```

After all these actions ,you can install what you want by npm ,there is something that you must notice:

- all packages that you installed by the npm will be put in folder node_modules ,when you install something ,it will check the node_modules first,if the folder dosen't exist,npm will create it automatically.
- the property settings of the packages installed by npm will be reserved in `package.json`,you need to create the file manually first.

create the file 'package.json' by order:

```bash
$ npm init
```

run the order,then follow the instructions and complete all the properties you need to set, the 'package.json' will be installed.
now you can install packages by order

```bash
$ npm install express(package names)
```

## webpack installation

install webpack globally

```bash
$ npm install -g webpack webpack-dev-server
```

install webpack locally

```bash
$ npm install --save webpack webpack-dev-server
```

## react installation

To install React with npm, run:

```bash
$ npm install --save react react-dom 
```

To installed Babel for offline conversion:

```bash
$ npm install --save babel-preset-react
```



