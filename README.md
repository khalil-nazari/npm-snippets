
# npm Basic

### Introduction 
npm stands for Node Package Manager


### What is a package?
package : a directory has one or more modules with package.json which contains the metadata about the package. 
module : a single js file that has some reasonbale functionality.


### npm usage
- It is used to look into others project and packages. 
- To install packages 
- To uninstall packages
- To update verions of packages 
- To start and test a project 


### npm help
`npm -h` display all npm commands. 
`npm install -h` display specific information about the install command 
`npm help <command>` => `npm help command` head you over to help web page. 


### npm shortcuts
- flag shortcus head over to [npm config](https://docs.npmjs.com/cli/v6/using-npm/config) OR https://docs.npmjs.com/cli/v6/using-npm/config
    `-v` : `--version`
    `-h , -?, --help, -H` : `--usage`
    `-g` : `--global`
    `-m` : `--message`
    `-S` : `--save`
    `-P` : `--save-prod`
    `-D` : `--save-dev`
    `-y` : `--yes`
    `-B` : `--save-Bundle`
    `-f` : `--force`
    `-l`: `--long`
    `-C`: `--prefix`
 

- There are also other shortcuts like  `npm i <package-name>`

### Creating package.json
There are two types of project that you may develop
- Typical wesbite for example a portfolio or an e-commerce web app. This is usually for users.
- A Third Party Package. This is for other developers to consume. 

When developting typical web project, we need to create package.json file 
- to track the dependencies of the packages we are using
- it help to create scripts easier 
- it avoid to install gulp or grunt any time to start the project. 
- `npm init` Or `npm init -y` command creates package.json via npm command


### Installing packages
`npm isntall <package-name>` install a pakcage. package-name is actually the package or the project we install. package-name is sometimes different with product. 
by default the commant will install the package under `"dependencies": {}`

Example: `npm i experss`.

`cat package.json` is used to read the package.json file

`npm instll jshint --save-dev` OR `npm install jshint -D` will isntall the package under `"devDependecies": {}`

### The package-lock.json
Contains the exact version of every package which has been installed. 


### Listing installed packages
`npm list` OR `npm ls` command lists all the packages installed and all of their dependent packages.
`npm list --depth 0` command lists only the package.
`npm list --depth 1` command lists the packages and only the first level of the dependencies.
`npm list --depth 0 --long` command lists packages with more details 
`npm list --depth 0 --json` command lists packages with more details in json format
`npm list --depth 0 --parseable` command lists the packages directories
`npm list --depth 0 -dev` command list out only devDependencies packages
`npm list --depth 0 -prod` command list out dependencies packages


### Installing global packages
We need to install a package globally becuase we need to run it in command line and in more than one project. For examle gulp. 
`npm install <package-name> -g`

To list out global packages
`npm list -g --depth 0`

### Removing a package
`npm uninstall <package-name>` remove a pakcage for node_modules directoy and package.json file. 

Some aliases
`npm rm`
`npm un`
`npm r`

To uninstall a package globally 
`npm uninstall -g <package-name>`



### Installing specific version 
### Installing existing dependencies 
### Update packages
### Setting defaults


# npm Advance