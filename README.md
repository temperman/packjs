#packjs

packing javascript file to one file.

##Install

Use bower

```bash
bower install --save packjs
```

##Usage

1. Write include file path (relative) in each heads of javascript files.

```javascript
console.log('foo');
// @include ./module.js
console.log('bar');
```

2. Run command.

```bash
$ packjs sourcefile.js targetfile.js
```

3. Output like this.

```javascript
console.log('foo');
function someModule(){};
console.log('bar');
```

4. If you run with ```-w``` option, then command run as **watching mode** and everytime you update file, do packing automaticaly.

```bash
$ packjs sourcefile.js targetfile.js -w
```
