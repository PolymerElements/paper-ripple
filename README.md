[![Published on NPM](https://img.shields.io/npm/v/@polymer/paper-ripple.svg)](https://www.npmjs.com/package/@polymer/paper-ripple)
[![Build status](https://travis-ci.org/PolymerElements/paper-ripple.svg?branch=master)](https://travis-ci.org/PolymerElements/paper-ripple)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://webcomponents.org/element/@polymer/paper-ripple)

## &lt;paper-ripple&gt;
`paper-ripple` provides a visual effect that other paper elements can
use to simulate a rippling effect emanating from the point of contact. The
effect can be visualized as a concentric circle with motion.

<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="paper-ripple.html">
    <style is="custom-style">
      div {
        height: 100px;
        width: 100%;
        box-shadow: 0 12px 15px 0 rgba(0, 0, 0, 0.24);
      }
      
      paper-ripple {
        color: #4285f4;
      }
    </style>
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->

See: [Documentation](https://www.webcomponents.org/element/@polymer/paper-ripple),
  [Demo](https://www.webcomponents.org/element/@polymer/paper-ripple/demo/demo/index.html).

## Usage

### Installation
```
npm install --save @polymer/paper-ripple
```

### In an html file
```html
<html>
  <head>
    <script type="module">
      import '@polymer/paper-ripple/paper-ripple.js';
    </script>
  </head>
  <body>
    <div style="position: relative">
      <paper-ripple></paper-ripple>
    </div>
  </body>
</html>
```
### In a Polymer 3 element
```js
import {PolymerElement, html} from '@polymer/polymer';
import '@polymer/paper-ripple/paper-ripple.js';

class SampleElement extends PolymerElement {
  static get template() {
    return html`
      <div style="position: relative">
        <paper-ripple></paper-ripple>
      </div>
    `;
  }
}
customElements.define('sample-element', SampleElement);
```

## Contributing
If you want to send a PR to this element, here are
the instructions for running the tests and demo locally:

### Installation
```sh
git clone https://github.com/PolymerElements/paper-ripple
cd paper-ripple
npm install
npm install -g polymer-cli
```

### Running the demo locally
```sh
polymer serve --npm
open http://127.0.0.1:<port>/demo/
```

### Running the tests
```sh
polymer test --npm
```
