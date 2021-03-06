#Marionette CLI

Marionette CLI is the command line utility that provides RequreJS/CommonJS app structure.

##Install

Run `npm install -g marionette-cli` or add dependency in your `package.json` file and run `npm install`

##Features
* Generate app skeleton
* Generate backbone/marionette files
* Support different module types (RequreJS, CommonJS)

##Commands
###Set
```
set [options] <type>  Change module type. Short - s
Usage: set [options] <type>
```

Example: `mt set rjs` <br />
Example: `mt s rjs`

###New
```
new [options] Create new project. Short - n
Usage: new [options]
```

Example: `mt new` <br />
Example: `mt n` <br />
Example: `mt n folderName` - will genarate app in `folderName` folder<br />

Will generate app with basic files: `config.js, main.js, app.js, controller.js, router.js, layout.js, collection.js, model.js`


###Generate
```
Usage: generate [options] [folder]
Generate files for marionette. Short - g
```

Options:
```
    -l --layout [name]       Layout
    -c --collection [name]   Collection
    -m --model [name]        Model
    -r --router [name]       Router
    -o --object [name]       Object or controller
    -v --itemView [name]     Item view
    --collectionView [name]  Collection view
    --compositeView [name]   Composite view
```

Example: `mt generate -l` - will create marionette layout file `layout.js` <br />
Example: `mt g -l` - the same as above

Example: `mt generate -l myName` - will create marionette layout file `myName.js` <br />
Example: `mt g -l` - the same as above

Example: `mt generate -l myName myFolder` - will create marionette layout file `myName.js` in folder `myFolder` <br />
Example: `mt g -l myName myFolder` - the same as above
