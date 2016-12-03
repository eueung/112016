class: split-40 nopadding
background-image: url( bkgs/daun.jpg )

.column_t2.center[.vmiddle.pushfront[
.figplaint-maxh450.opacity7[
![]( images/react.png)
]
]]
.column_t2.shadelightdark.add-left-border.pushfront[.vmiddle.nopadding[
.boxtitle4[
### Starter Kit Basic Examples
# .fsize95[React Examples]

### [Eueung Mulyana](https://github.com/eueung)
### https://eueung.github.io/112016/react-cont
#### CodeLabs | [Attribution-ShareAlike CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/)
#### 
]
]]
---
class: column_t1 middle center

#React Version: **15.4.1**

.fonth5[Introduction to React already covered here: **https://eueung.github.io/112016/react** ]



---
class: split-60 nopadding 
background-image: url( images/fbreact.jpg )

.column_t2[.vmiddle.center[

]]
.column_bt[.vmiddle.pushfront[
#React Releases

.fonth5[@github]







]]


---
class: column_t1 middle

.fonth4[
.tabtype1.fullwidth[
| Outline   |
|:-------------:|
|Starter Kit - Overview|
|Basic Examples|








]]


---
class: split-30 nopadding
background-image: url( bkgs/daun.jpg )

.column_t2.center[.vmiddle[
.figplaint-maxh550.opacity7[
![]( images/react.png)
]
]]
.column_t2[.vmiddle.nopadding[
.shadelightdark[.boxtitle1[
### 
# .fsize85[Starter Kit Overview]

### 
### 
#### 
#### 
]]
]]

---
class: split-40 nopadding 

.column_t1[.vmiddle.pushfront.right[

#Structure









]]
.column_t2[.vmiddle.pushfront.defaultalign[







```bash
*react-15.4.1$ tree -L 2
.
|-- build
|------ react-dom-fiber.js
|   |-- react-dom-fiber.min.js
|   |-- react-dom.js
|   |-- react-dom.min.js
|   |-- react-dom-server.js
|   |-- react-dom-server.min.js
|   |-- react.js
|   |-- react.min.js
|   |-- react-with-addons.js
|   |-- react-with-addons.min.js
|-- examples
*|   |-- basic
*|   |-- basic-click-counter
*|   |-- basic-commonjs
*|   |-- basic-jsx
*|   |-- basic-jsx-external
*|   |-- basic-jsx-harmony
*|   |-- basic-jsx-precompile
*|   |-- fiber
|   |-- jquery-bootstrap
|   |-- jquery-mobile
|   |-- quadratic
|   |-- README.md
|   |-- shared
|   |-- transitions
|   |-- webcomponents
|-- README.md

```



]]


---
class: split-30 nopadding
background-image: url( bkgs/daun.jpg )

.column_t2.center[.vmiddle[
.figplaint-maxh550.opacity7[
![]( images/react.png)
]
]]
.column_t2[.vmiddle.nopadding[
.shadelightdark[.boxtitle1[
### 
# .fsize95[Basic Examples]

### 
### 
#### 
#### 
]]
]]

---
class: split-40 nopadding 

.column_t1[.vmiddle.pushfront.right[

#Basic Examples









]]
.column_t2[.vmiddle.pushfront.defaultalign[







###One HTML
- basic
- basic-jsx
- basic-jsx-harmony
- .red[**basic-click-counter**] (.uline[state])
- **fiber** (react-dom-fiber)

###One HTML + One JS
- basic-jsx-external (`src/example.js`)
- .blue[**basic-jsx-precompile**] (`build/example.js`)

###HTML+JS+package.json (npm)
- .blue[**basic-commonjs**] (`bundle.js`)



]]


---
class: split-70 nopadding 

.column_t2[.vmiddle.pushfront.defaultalign[









```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Basic Example</title>
*   <link rel="stylesheet" href="../shared/css/base.css" />
  </head>
  <body>
    <h1>Basic Example</h1>
    <div id="container">
      <p> To install React, follow the instructions on <a href="https://github.com/facebook/react/">GitHub</a>. </p>
      <p> If you can see this, React is <strong>not</strong> working right. If you checked out the source from GitHub make sure to run <code>grunt</code>. </p>
    </div>
    <h4>Example Details</h4>
*   <p>This is written in vanilla JavaScript (without JSX) and transformed in the browser.</p>
    <p>
      Learn more about React at <a href="https://facebook.github.io/react" target="_blank">facebook.github.io/react</a>.
    </p>
*   <script src="../../build/react.js"></script>
*   <script src="../../build/react-dom.js"></script>
*   <script> ... </script>
  </body>
</html>
```



]]
.column_t1[.vmiddle.pushfront.defaultalign[

#HTML




.fonth5[
**basic**<br/>
**basic-jsx**<br/>
**basic-jsx-harmony**<br/>
**fiber**<br/>
.bluelight[**basic-click-counter**]<br/>
]



]]


---
class: split-70 nopadding 

.column_t2[.vmiddle.pushfront.defaultalign[









```javascript
*<script>
*  var ExampleApplication = React.createClass({
*    render: function() {
*      var elapsed = Math.round(this.props.elapsed  / 100);
       var seconds = elapsed / 10 + (elapsed % 10 ? '' : '.0' );
       var message =
         'React has been successfully running for ' + seconds + ' seconds.';

*      return React.DOM.p(null, message);
     }
   });

   // Call React.createFactory instead of directly call ExampleApplication({...}) in React.render
*  var ExampleApplicationFactory = React.createFactory(ExampleApplication);

   var start = new Date().getTime();
   setInterval(function() {
     ReactDOM.render(
       ExampleApplicationFactory({elapsed: new Date().getTime() - start}),
*      document.getElementById('container')
     );
   }, 50);
*</script>
```



]]
.column_t1[.vmiddle.pushfront.defaultalign[

#basic




.fonth5[Vanilla JS<br/>]
<br/>**render**<br/>**this.props**<br/>React.DOM.p()



]]


---
class: split-70 nopadding 

.column_t2[.vmiddle.pushfront.defaultalign[









```javascript
*<p>This is written with JSX and transformed in the browser.</p>
*<script src="https://cdnjs.cloudflare.com/ajax/libs/babel-core/5.8.24/browser.min.js"></script>
*<script type="text/babel">
   var ExampleApplication = React.createClass({
    render: function() {
      var elapsed = Math.round(this.props.elapsed  / 100);
      var seconds = elapsed / 10 + (elapsed % 10 ? '' : '.0' );
      var message =
        'React has been successfully running for ' + seconds + ' seconds.';

*     return <p>{message}</p>;
    }
  });
  var start = new Date().getTime();
  setInterval(function() {
    ReactDOM.render(
*     <ExampleApplication elapsed={new Date().getTime() - start} />,
      document.getElementById('container')
    );
   }, 50);
</script>

```



]]
.column_t1[.vmiddle.pushfront.defaultalign[

#basic-jsx




.fonth5[JS+.yellow[JSX]<br/>.yellow[Requires **babel**]<br/>]
<br/>**render**<br/>**this.props**<br/>.yellow[Element `<p>`]<br/>.yellow[Passing `props.elapsed`]



]]


---
class: split-70 nopadding 

.column_t2[.vmiddle.pushfront.defaultalign[









```javascript
*<p>This is written with JSX with Harmony (ES6) syntax and transformed in the browser.</p>
<script src="https://cdnjs.cloudflare.com/ajax/libs/babel-core/5.8.24/browser.min.js"></script>
<script type="text/babel">
* class ExampleApplication extends React.Component {
*   render() {
      var elapsed = Math.round(this.props.elapsed  / 100);
      var seconds = elapsed / 10 + (elapsed % 10 ? '' : '.0' );
      var message =
*       `React has been successfully running for ${seconds} seconds.`;

      return <p>{message}</p>;
    }
  }
  var start = new Date().getTime();
* setInterval(() => {
    ReactDOM.render(
      <ExampleApplication elapsed={new Date().getTime() - start} />,
      document.getElementById('container')
    );
  }, 50);
</script>
```



]]
.column_t1[.vmiddle.pushfront.defaultalign[

#basic-jsx-harmony




.fonth5[.yellow[ES2015]+JSX<br/>Requires **babel**<br/>]
<br/>**render**<br/>**this.props**<br/>Element `<p>`



]]


---
class: split-70 nopadding 

.column_bt[.vmiddle.pushfront.defaultalign[








.figplaint[
![](images/basic1.png)
]


]]
.column_t1[.vmiddle.pushfront.defaultalign[

#basic






]]


---
class: split-70 nopadding 

.column_bt[.vmiddle.pushfront.defaultalign[








.figplaint[
![](images/basic2.png)
]


]]
.column_t1[.vmiddle.pushfront.defaultalign[

#basic-jsx






]]


---
class: split-70 nopadding 

.column_bt[.vmiddle.pushfront.defaultalign[








.figplaint[
![](images/basic3.png)
]


]]
.column_t1[.vmiddle.pushfront.defaultalign[

#basic-jsx-harmony






]]


---
class: split-70 nopadding 

.column_t2[.vmiddle.pushfront.defaultalign[









```javascript
*<script src="../../build/react-dom-fiber.js"></script>
<script>
* function ExampleApplication(props) {
    var elapsed = Math.round(props.elapsed  / 100);
    var seconds = elapsed / 10 + (elapsed % 10 ? '' : '.0' );
    var message =
      'React has been successfully running for ' + seconds + ' seconds.';

    return React.DOM.p(null, message);
  }

  // Call React.createFactory instead of directly call ExampleApplication({...}) in React.render
  var ExampleApplicationFactory = React.createFactory(ExampleApplication);

  var start = new Date().getTime();
  setInterval(function() {
*   ReactDOMFiber.render(
      ExampleApplicationFactory({elapsed: new Date().getTime() - start}),
      document.getElementById('container')
    );
  }, 50);
</script>
```



]]
.column_t1[.vmiddle.pushfront.defaultalign[

#fiber




.fonth5[**basic** with fiber]
.yellow[<br/>function vs. React.createClass()<br/>ReactDOMFiber vs. ReactDOM]

Ref: **React Fiber** is an ongoing reimplementation of React's core algorithm. It is the culmination of over two years of research by the React team. \[ [React Fiber](https://github.com/acdlite/react-fiber-architecture) \]



]]


---
class: split-70 nopadding 

.column_bt[.vmiddle.pushfront.defaultalign[








.figplaint[
![](images/basic4.png)
]


]]
.column_t1[.vmiddle.pushfront.defaultalign[

#fiber






]]


---
class: split-70 nopadding 

.column_t2[.vmiddle.pushfront.defaultalign[









```javascript
<script src="https://cdnjs.cloudflare.com/ajax/libs/babel-core/5.8.24/browser.min.js"></script>
<script type="text/babel">
  var Counter = React.createClass({
*   getInitialState: function () {
*     return { count: 0 };
*   },
*   handleClick: function () {
*     this.setState({
*       count: this.state.count + 1,
*     });
    },
    render: function () {
      return (
        <button onClick={this.handleClick}>
*         Click me! Number of clicks: {this.state.count}
        </button>
      );
    }
  });
  ReactDOM.render(
    <Counter />,
    document.getElementById('container')
  );
</script>

```



]]
.column_t1[.vmiddle.pushfront.defaultalign[

# .bluelight[basic-click-counter]




.fonth5[JS+JSX<br/>Requires **babel**<br/>]
.yellow[<br/>**this.state**<br/>**this.setState**<br/>**getInitialState**]<br/>render



]]


---
class: split-70 nopadding 

.column_bt[.vmiddle.pushfront.defaultalign[








.figplaint[
![](images/basic5.png)
]


]]
.column_t1[.vmiddle.pushfront.defaultalign[

#.bluelight[basic-click-counter]






]]


---
class: split-30 nopadding 

.column_t1[.vmiddle.pushfront.defaultalign[

# basic-jsx-external






.fonth5[JS+JSX<br/>Requires **babel**<br/>]
<br/>basic-jsx<br/>
.yellow[<br/>index.html<br/>example.js]<br/>



]]
.column_bt[.vmiddle.pushfront.defaultalign[






.figplaint[
![](images/basic6.png)
]
```javascript
*<script type="text/babel" src="example.js"></script>
```



]]


---
class: split-30 nopadding 

.column_t1[.vmiddle.pushfront.defaultalign[

# basic-jsx-external









]]
.column_bt[.vmiddle.pushfront.defaultalign[






.figplaint[
![](images/basic6s.png)
]



]]


---
class: split-30 nopadding 

.column_t1[.vmiddle.pushfront.defaultalign[

# basic-jsx-external









]]
.column_t2[.vmiddle.pushfront.defaultalign[







```bash

*react-15.4.1$ python -m SimpleHTTPServer
Serving HTTP on 0.0.0.0 port 8000 ...
127.0.0.1 - - [04/Dec/2016 03:28:06] "GET /examples/basic-jsx-external/ HTTP/1.1" 200 -
127.0.0.1 - - [04/Dec/2016 03:28:06] "GET /examples/shared/css/base.css HTTP/1.1" 200 -
127.0.0.1 - - [04/Dec/2016 03:28:06] "GET /build/react.js HTTP/1.1" 200 -
127.0.0.1 - - [04/Dec/2016 03:28:06] "GET /build/react-dom.js HTTP/1.1" 200 -
127.0.0.1 - - [04/Dec/2016 03:28:06] "GET /examples/basic-jsx-external/example.js HTTP/1.1" 200 -

```



]]


---
class: split-30 nopadding 

.column_t1[.vmiddle.pushfront.defaultalign[

# basic-jsx-precompile






.fonth5[JS+JSX<br/>.yellow[**babel** @dev .uline[NOT] @browser<br/>]]
<br/>basic-jsx
<br/><br/>index.html<br/>example.js<br/>



]]
.column_bt[.vmiddle.pushfront.defaultalign[






.figplaint[
![](images/basic7.png)
]
```javascript
*<script src="build/example.js"></script>
```



]]


---
class: split-30 nopadding 

.column_t1[.vmiddle.pushfront.defaultalign[

# basic-jsx-precompile









]]
.column_t2[.vmiddle.pushfront.defaultalign[







```bash
*$ npm install -g babel-cli 
*$ npm install -g babel-preset-react 
$ npm install -g babel-preset-es2015

*$ babel version
6.18.0 (babel-core 6.18.2)
*$ babel --presets react example.js --out-dir=build
example.js -> build\example.js

*react-15.4.1/examples/basic-jsx-precompile$ tree
.
|-- example.js
|-- index.html
*|-- build
*|--- example.js
```



]]


---
class: split-30 nopadding 

.column_t1[.vmiddle.pushfront.defaultalign[

# basic-jsx-precompile






.fonth5[Vanilla JS after Build<br/>]
Testing: .yellow[HTTP Server .uline[NOT] Required]



]]
.column_bt[.vmiddle.pushfront.defaultalign[






.figplaint[
![](images/basic7s.png)
]



]]


---
class: split-30 nopadding 

.column_t1[.vmiddle.pushfront.defaultalign[

# basic-commonjs






.fonth5[JS+JSX<br/>.yellow[**react** &amp; **babel** @dev .uline[NOT] @browser<br/>]]
<br/>basic-jsx
<br/><br/>index.html<br/>index.js<br/>package.json<br/>



]]
.column_bt[.vmiddle.pushfront.defaultalign[






.figplaint[
![](images/basic8.png)
]
```javascript
*<script src="bundle.js"></script>
```



]]


---
class: split-30 nopadding 

.column_t1[.vmiddle.pushfront.defaultalign[

# basic-commonjs






.fonth5[index.html<br/>index.js<br/>]



]]
.column_t2[.vmiddle.pushfront.defaultalign[







```html
<!DOCTYPE html>
<html>
  <head>...</head>
  <body>
    <h1>Basic CommonJS Example with Browserify</h1>
    <div id="container"> <p>To install React, ...</p> </div>
    <h4>Example Details</h4> <p>This is written ...</p>
*   <script src="bundle.js"></script>
  </body>
</html>
```

```javascript
*'use strict';

*var React = require('react');
*var ReactDOM = require('react-dom');

var ExampleApplication = React.createClass({
  render: function() {
    var elapsed = Math.round(this.props.elapsed  / 100);
    var seconds = elapsed / 10 + (elapsed % 10 ? '' : '.0' );
    var message =
      'React has been successfully running for ' + seconds + ' seconds.';

    return <p>{message}</p>;
  }
});
*...
```



]]


---
class: split-30 nopadding 

.column_t1[.vmiddle.pushfront.defaultalign[

# basic-commonjs






.fonth5[package.json]



]]
.column_t2[.vmiddle.pushfront.defaultalign[







```json
{
  "name": "react-basic-commonjs-example",
  "description": "Basic example of using React with CommonJS",
  "private": true,
* "main": "index.js",
* "dependencies": {
    "babel-preset-es2015": "^6.6.0",
    "babel-preset-react": "^6.5.0",
    "babelify": "^7.3.0",
    "browserify": "^13.0.0",
    "react": "^15.0.2",
    "react-dom": "^15.0.2",
    "watchify": "^3.7.0"
  },
  "scripts": {
    "build": "browserify ./index.js -t babelify -o bundle.js",
*   "start": "watchify ./index.js -v -t babelify -o bundle.js"
  }
}
```



]]


---
class: split-30 nopadding 

.column_t1[.vmiddle.pushfront.defaultalign[

# basic-commonjs









]]
.column_t2[.vmiddle.pushfront.defaultalign[







```bash
*basic-commonjs$ npm install
*basic-commonjs$ npm start

> react-basic-commonjs-example@ start /home/em/basic-commonjs
> watchify ./index.js -v -t babelify -o bundle.js

721641 bytes written to bundle.js (2.18 seconds)

*basic-commonjs$ tree -L 1
.
*|-- bundle.js
|-- index.html
|-- index.js
*|-- node_modules
|-- package.json
```



]]


---
class: split-30 nopadding 

.column_t1[.vmiddle.pushfront.defaultalign[

# basic-commonjs






.fonth5[Vanilla JS after Build<br/>.yellow[Everything Bundled]<br/>]
Testing: HTTP Server .uline[NOT] Required



]]
.column_bt[.vmiddle.pushfront.defaultalign[






.figplaint[
![](images/basic8s.png)
]



]]


---
class: split-50 nopadding 
background-image: url(bkgs/minion-bubble-right910.jpg)

.column_t2[.vmiddle.center[

]]
.column_t2[.vmiddle.xkcd_font.pushfront.center[
#That's All

for the basics ... we'll continue later ... piece of cake, no?



]]


---
class: split-30 nopadding
background-image: url( bkgs/daun.jpg )

.column_t2.center[.vmiddle[
.figplaint-maxh550.opacity7[
![]( images/react.png)
]
]]
.column_t2[.vmiddle.nopadding[
.shadelightdark[.boxtitle1[
### 
# .fsize95[Refs]

### 
### 
#### 
#### 
]]
]]


---
# Refs

.fonth5[
1. [A JavaScript library for building user interfaces | React](https://facebook.github.io/react/)
1. [facebook/react: A declarative, efficient, and flexible JavaScript library for building user interfaces.](https://github.com/facebook/react)
1. [acdlite/react-fiber-architecture: A description of React's new core algorithm, React Fiber](https://github.com/acdlite/react-fiber-architecture)
1. [Intro and Concept - Learning React](https://eueung.github.io/112016/react)
]

---
class: split-40 nopadding
background-image: url( bkgs/daun.jpg )

.column_t2.center[.vmiddle.pushfront[
.figplaint-maxh550.opacity7[
![]( images/react.png)
]
]]
.column_t2.shadelightdark.add-left-border.pushfront[.vmiddle.nopadding[
.boxtitle4[
### 
# .fsize95[END]

### [Eueung Mulyana](https://github.com/eueung)
### https://eueung.github.io/112016/react-cont
#### CodeLabs | [Attribution-ShareAlike CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/)
#### 
]
]]


