[![Build Status](https://travis-ci.org/hetznerZA/wc-router.svg?branch=master)](https://travis-ci.org/hetznerZA/wc-router)

The `<wc-router>` element provides super fast and flexible routing inspired by [Express](https://expressjs.com/).

```html
<wc-router params="{{params}}" use-hash>
  <div route="(home)?">Home</div>
  <div route="blog/:author/:id">Named parameters: [[params.id]], [[params.author]].</div>
  <div route="view/(.*)">Unnamed parameters: [[params.0]]</div>
  <div route="**">Page not found.</div>
</wc-router>
```

## Features

- It can extract named and unnamed route paramaters
- It can display the selected content
- It can import custom elements on selection
- It can accept a route object or route-path string
- It can respond to URL hash changes

## Developement

This project requires **[npm](https://www.npmjs.com/)** and **[bower](https://bower.io/#install-bower)** to be installed.

### Setup

```bash
$ npm install && bower update
```

### Run 

Polyserve the web component
```bash
$ npm start
```
_default port is 9099_

### Build

Build a client version of `pathToRegexp.js` using browserify.

```bash
$ npm run build
```

### Test

Run tests from console/terminal
```bash
$ npm test
```

Run tests in browser with locally hosted content

[http://localhost:9099/test/index.html](http://localhost:9099/components/wc-textarea-code/test/index.html)

## Todo

- Improve demo page with more features & iron demo helpers.

## Resources

* [Polymer](https://www.polymer-project.org/)
* [WebComponents](http://webcomponents.org/)
* [Polyserve](https://github.com/PolymerLabs/polyserve)
* [Web Component Tester](https://github.com/Polymer/web-component-tester)
* [Browserify](http://browserify.org/)
* [Express](https://expressjs.com/en/guide/routing.html)
* [path-to-regexp](https://github.com/pillarjs/path-to-regexp/blob/master/Readme.md)