# quasar-serve

### Usage

if your quasar dist structure like
`````
dist/spa
  css
  fonts
  icons
  img
  js
  favicon.ico
  index.html
`````

use code

`````javascript
const quasarServe = require('quasar-serve');
const app = express();
app.use(quasarServe({
  distPath: path.join(__dirname, './../client/dist/spa'),
  replaces: {
    baseUrl: config.baseUrl,
  },
}));

`````
