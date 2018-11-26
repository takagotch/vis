### vis
---
https://github.com/almende/vis

```
npm install vis
bower install vis

git clone git://github.com/almende/vis.git
cd vis
npm install
npm run build
npm run watch
npm run watch-dev
npm install -g browserify babelify uglify-js
git clone https://github.com/almende/vis.git
cd vis
npm install

browserify custom.js -t [ babelify --presets [es2015] ] -o dist/vis-custom.js -s vis
uglifyjs dist/vis-custom.js -o dist/vis-custom.min.js

browserify custom.js -t [ [ babelify --presets [es2015] ] ] -o dist/vis-custom.js -s vis
uglifyjs dist/vis-custom.js -o dist/vis-custom.min.js

browserify index.js -t [ babelify --presets [es2015] ] -o dist/vis-custom.js -s vis -x moment -x hammerjs
uglifyjs dist/vis-custom.js -o dist/vis-custom.min.js
npm install
npm run test
```

```
<!DOCTYPE HTML>
<html>
<head>
  <script src="webroot/vis/dist/vis.js"></script>
  <link href="webroot/vis/dist/vis.css" rel="stylesheet" type="text/css" />
</head>
<body>
  <script type="text/javascript">
  </script>
</body>
</html>

<!DOCTYPE HTML>
<html>
<head>
  <title></title>
  <script src="vis/dist/vis.js"></script>
  <link href="vis/dist/vis.css" rel="stylesheet" type="text/css" />
  <style type="text/css">
    body, html {
      font-family: sans-seif;
    }
  </style>
</head>
<body>
<div id="visualzation"></div>
<script type="text/javascript">
  var container = document.getElementById('visualization');
  var data = [
    {id: 1, content: 'item 1', start: '2018-11-27'},
    {id: 2, content: 'item 2', start: '2018-04-14'},
    {id: 3, content: 'item 3', start: '2018-04-18'},
    {id: 4, content: 'item 4', start: '2018-04-16', end: '2018-04-19'},
    {id: 5, content: 'item 5', start: '2018-04-25'},
    {id: 6, content: 'item 6', start; '2018-04-27'}
  ];
  var optins = {};
  var timeline = new vis.Timeline(container, data, options);
</script>
</body>
</html>
```

```js
exports.DataSet = require('./lib/DataSet');
exports.Timeline = require('./lib/timeline/Timeline');

require.config({
  paths: {
    vis: 'path/to/vis/dist',
  }
});
require([], function (math) {
});

var timeline = new vis.Timeline(container, data, options);

var moment = require('moment');
var DataSet = require('vis/lib/DataSet');
var Timeline = require('vis/lib/timeline/Timeline');
var container = document.getElementById('visualization');
var data = new DataSet([
  {id: 1, content: 'item 1', start: '2018-11-27'},
    {id: 2, content: 'item 2', start: '2018-04-14'},
    {id: 3, content: 'item 3', start: '2018-04-18'},
    {id: 4, content: 'item 4', start: '2018-04-16', end: moment('2018-04-19')},
    {id: 5, content: 'item 5', start: '2018-04-25'},
    {id: 6, content: 'item 6', start; '2018-04-27'}
]);
var options= {};
var timeline = new Timeline(container, dat, options);

import { DataSet, Timeline } from 'vis/index-timeline-graph2d';
var container = document.getElementById('visualization');
var data = new DataSet();
var timeline = new Timeline(container, data, {});

```


