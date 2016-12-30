class: split-40 nopadding
background-image: url( bkgs/rambutan.jpg )

.column_t2.center[.vmiddle.pushfront[
.figplaint-maxh550.opacity7[
![]( images/firebase.png)
]
]]
.column_t2.shadelightdark.add-left-border.pushfront[.vmiddle.nopadding[
.boxtitle4[
### Introduction - Realtime Database
# .fsize175[.yellow[Firebase]]

### [Eueung Mulyana](https://github.com/eueung)
### https://eueung.github.io/112016/firebase
#### CodeLabs | [Attribution-ShareAlike CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/)
#### 
]
]]
---
class: column_t1 middle center

.fonth3[.yellow[**Firebase**] Version: **3.6.4**]<br/>.fonth4[.yellow[**Vue.JS**] **2.1.6** | .yellow[**VueFire**] **1.3.0** | .yellow[**Vue Material**] **0.5.2** ]




---
class: column_t1 middle

.fonth4[
.tabtype1.fullwidth[
| Outline   |
|:-------------:|
|Introduction|
|Quick Start|
|VueFire|







]]

---
class: split-30 nopadding
background-image: url( bkgs/rambutan.jpg )

.column_t2.center[.vmiddle[
.figplaint-maxh550.opacity7[
![]( images/firebase.png)
]
]]
.column_t2[.vmiddle.nopadding[
.shadelightdark[.boxtitle1[
### 
# .fsize95[Introduction]

### 
### 
#### 
#### 
]]
]]
---
class: split-60 nopadding 

.column_t1[.vmiddle.pushfront.right[








.fonth4[
The Firebase Realtime Database is a **cloud-hosted** database. Data is stored as .uline[JSON] and **synchronized** in realtime to .uline[every] connected client. ]
.fonth5[
When you build cross-platform apps with Firebase iOS, Android, and JavaScript SDKs, **all** of your clients share .uline[one] Realtime Database instance and automatically receive .uline[updates] with the newest data.
]
<br/>



]]
.column_t2[.vmiddle.pushfront.center[

# Firebase Realtime Database




.figplaint[
![](images/firebase.png)
]


]]

---
class: split-60 nopadding 

.column_t2[.vmiddle.pushfront.right[








The Firebase Realtime Database lets you build rich, collaborative applications by allowing secure access to the database directly from **client-side** code. 
.fonth5[
Data is persisted locally, and even while offline, realtime events continue to fire, giving the end user a responsive experience. When the device regains connection, the Realtime Database synchronizes the local data changes with the remote updates that occurred while the client was offline, merging any conflicts automatically.
]
The Realtime Database provides a flexible, expression-based rules language, called Firebase Realtime Database **Security Rules**, to define how your data should be structured and when data can be read from or written to. When integrated with Firebase Authentication, developers can define who has access to what data, and how they can access it.

Ref: [Firebase Realtime Database ](https://firebase.google.com/docs/database/)



]]
.column_t1[.vmiddle.pushfront.defaultalign[






.fonth5[
The Realtime Database is a **NoSQL** database and as such has .uline[different] optimizations and functionality compared to a .uline[relational] database. The Realtime Database API is designed to only allow operations that can be executed **quickly**. 
]
This enables you to build a great realtime experience that can serve **millions** of users without compromising on responsiveness. Because of this, it is important to think about **how** users need to access your data and then **structure** it accordingly.


]]


---
class: split-30 nopadding
background-image: url( bkgs/rambutan.jpg )

.column_t2.center[.vmiddle[
.figplaint-maxh550.opacity7[
![]( images/firebase.png)
]
]]
.column_t2[.vmiddle.nopadding[
.shadelightdark[.boxtitle1[
### 
# .fsize95[Quick Start]

### 
### 
#### 
#### 
]]
]]
---
class: split-40 nopadding 

.column_t1[.vmiddle.pushfront.right[

# Firebase Setup






.fonth5[
Quickstart Sample Project for Web
]


]]
.column_t2[.vmiddle.pushfront.defaultalign[






.fonth5[
- Create Project
- Firebase Client Snippet
- Check DB Rules
- Enable Firebase Auth - Google Sign-In
- Adjust Authorized Domains
]


]]


---
class: bkgpos_00 nopadding
background-image: url(images/fbase-01.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# Firebase Console - Create Project
]]

---
class: bkgpos_00 nopadding
background-image: url(images/fbase-02.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# Firebase Console - Add Firebase
]]

---
class: bkgpos_00 nopadding
background-image: url(images/fbase-03.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# Snippet - Load &amp; Initialize Firebase
]]

---
class: bkgpos_00 nopadding
background-image: url(images/fbase-04.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# Database - Default Rules
]]

---
class: bkgpos_00 nopadding
background-image: url(images/fbase-05.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# Authentication - Enable Google Sign-In
]]

---
class: bkgpos_00 nopadding
background-image: url(images/fbase-06.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# Authentication - Authorized Domains
]]

---
class: split-40 nopadding 

.column_t1[.vmiddle.pushfront.right[

#Running Quickstart Sample









]]
.column_t2[.vmiddle.pushfront.defaultalign[







```bash
*$ sudo npm install -g firebase-tools

*$ git clone https://github.com/firebase/quickstart-js.git
*$ cd quickstart-js/database

*quickstart-js/database$ tree
.
|-- firebase.json
|-- firebase-logo.png
*|-- index.html
*|-- main.css
|-- pics
|   |-- enable.png
|   |-- redcircle.png
|   |-- snippet.png
|-- README.md
|-- scripts
*|   |-- main.js
|-- silhouette.jpg


*quickstart-js/database$ firebase serve -o 0.0.0.0

Starting Firebase development server...

Project Directory: /home/em/fbasedir/quickstart-js/database
Public Directory: ./

Server listening at: http://0.0.0.0:5000
```



]]


---
class: bkgpos_00 nopadding
background-image: url(images/fbase-07.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# .yellow[quickstart-js/database] - Splash Page
]]

---
class: bkgpos_00 nopadding
background-image: url(images/fbase-08.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# .yellow[quickstart-js/database] - Access Permissions
]]

---
class: bkgpos_00 nopadding
background-image: url(images/fbase-09.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# .yellow[quickstart-js/database] - Landing (Signed-In)
]]

---
class: bkgpos_00 nopadding
background-image: url(images/fbase-10.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# .yellow[quickstart-js/database] - Sample Posts
]]

---
class: bkgpos_00 nopadding
background-image: url(images/fbase-11.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# Firebase DB Console - Data
]]

---
class: bkgpos_00 nopadding
background-image: url(images/fbase-12.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# Firebase DB Console - Data
]]

---
class: split-70 nopadding 

.column_t2[.pushfront.defaultalign[








.fullcode[

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="description" content="Demonstrates the use of Google Cloud Database with a Firebase DB">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Firebase Database Quickstart</title>

  <!-- Disable tap highlight on IE -->
  <meta name="msapplication-tap-highlight" content="no">

  <!-- Add to homescreen for Chrome on Android -->
  <meta name="mobile-web-app-capable" content="yes">
  <meta name="application-name" content="Firebase Database Quickstart">
  <meta name="theme-color" content="#303F9F">

  <!-- Add to homescreen for Safari on iOS -->
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
  <meta name="apple-mobile-web-app-title" content="Firebase Database Quickstart">
  <meta name="apple-mobile-web-app-status-bar-style" content="#303F9F">

  <!-- Tile icon for Win8 -->
  <meta name="msapplication-TileColor" content="#3372DF">
  <meta name="msapplication-navbutton-color" content="#303F9F">

  <!-- Material Design Lite -->
  <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
  <link rel="stylesheet" href="https://code.getmdl.io/1.1.3/material.blue_grey-orange.min.css">
  <script src="https://code.getmdl.io/1.1.3/material.min.js"></script>

  <link rel="stylesheet" href="main.css">

  <!-- Firebase -->
* <script src="https://www.gstatic.com/firebasejs/3.6.4/firebase.js"></script>
  <script>
   var config = {
*    apiKey: "AIzaSyCyzw3nfQvyr38Yh127RPy_12345_aHefU",
     authDomain: "fbase-test-54a62.firebaseapp.com",
*    databaseURL: "https://fbase-test-54a62.firebaseio.com",
     storageBucket: "fbase-test-54a62.appspot.com",
     messagingSenderId: "989408983123"
   };
   firebase.initializeApp(config);
  </script>

</head>
<body>
<div class="demo-layout mdl-layout mdl-js-layout mdl-layout--fixed-header">

* <!-- Splash screen -->
  <section id="page-splash">
    <h3 class="logo">Database Web Quickstart</h3>
    <div>
      <button id="sign-in-button" class="mdl-button--raised mdl-button mdl-js-button mdl-js-ripple-effect"><i class="material-icons">account_circle</i> Sign in with Google</button>
    </div>
  </section>

* <!-- Header section containing logo and menu -->
* <header class="header mdl-layout__header mdl-color-text--white mdl-color--light-blue-700">

    <div class="mdl-layout__header-row titlebar">
      <h3 class="logo">Database Web Quickstart</h3>
      <button id="sign-out-button" class="mdl-button--raised mdl-button mdl-js-button mdl-js-ripple-effect"><i class="material-icons">account_circle</i> Sign out</button>
    </div>

    <!-- Navigation Bar -->
    <div class="tab mdl-layout__header-row mdl-color--light-blue-600">
      <div class="mdl-tab">
        <div id="menu-recent" class="mdl-layout__tab is-active mdl-button mdl-js-button mdl-js-ripple-effect">
          <i class="material-icons">new_releases</i> Recent
        </div>
        <div id="menu-my-posts" class="mdl-layout__tab mdl-button mdl-js-button mdl-js-ripple-effect">
          <i class="material-icons">home</i> My posts
        </div>
        <div id="menu-my-top-posts" class="mdl-layout__tab mdl-button mdl-js-button mdl-js-ripple-effect">
          <i class="material-icons">trending_up</i> My top posts
        </div>
        <button class="mdl-button mdl-js-button mdl-button--fab mdl-color--amber-400 mdl-shadow--4dp mdl-js-ripple-effect" id="add">
          <i class="material-icons">mode_edit</i>
        </button>
      </div>
    </div>
* </header>

* <main class="mdl-layout__content mdl-color--grey-100">

*   <!-- Show the add post form -->
    <section class="mdl-grid content" id="add-post" style="display:none">
      <div class="mdl-cell mdl-cell--12-col mdl-grid">

          <!-- Card containing the inputs to add a new messages -->
          <div class="mdl-card mdl-shadow--2dp mdl-cell mdl-cell--12-col mdl-cell--8-col-tablet
                  mdl-cell--6-col-desktop">
            <div class="mdl-card__title mdl-color--light-blue-600 mdl-color-text--white">
              <h2 class="mdl-card__title-text">New Post</h2>
            </div>
            <div class="mdl-card__supporting-text mdl-color-text--grey-600">
              <form id="message-form" action="#">
                <div class="mdl-textfield mdl-js-textfield mdl-textfield--floating-label">
                  <input class="mdl-textfield__input" type="text" id="new-post-title">
                  <label class="mdl-textfield__label" for="new-post-title">Post title...</label>
                </div>
                <div class="mdl-textfield mdl-js-textfield mdl-textfield--floating-label">
                  <textarea class="mdl-textfield__input" rows="3" id="new-post-message"></textarea>
                  <label class="mdl-textfield__label" for="new-post-message">Post message...</label>
                </div>
                <button type="submit" class="mdl-button mdl-js-button mdl-button--raised mdl-js-ripple-effect">
                  Add post
                </button>
              </form>
            </div>
        </div>
      </div>
    </section>

*   <!-- Show a list of recent posts -->
    <section class="mdl-grid content" id="recent-posts-list" style="display:none">
      <div class="posts-container mdl-cell mdl-cell--12-col mdl-grid">
      </div>
    </section>

*   <!-- Show the list of user's posts -->
    <section class="mdl-grid content" id="user-posts-list" style="display:none">
      <div class="posts-container mdl-cell mdl-cell--12-col mdl-grid">
      </div>
    </section>

*   <!-- Show the list of top user's posts -->
    <section class="mdl-grid content" id="top-user-posts-list" style="display:none">
      <div class="posts-container mdl-cell mdl-cell--12-col mdl-grid">
      </div>
    </section>
* </main>
</div>

*<script src="scripts/main.js"></script>
</body></html>
```
]



]]
.column_t1[.vmiddle.pushfront.defaultalign[

# index.html




.fonth5[]
<br/>



]]


---
class: split-70 nopadding 

.column_t2[.pushfront.defaultalign[








.fullcode[

```css
html, body {
    font-family: 'Roboto', 'Helvetica', sans-serif;
}
a {
    text-decoration: underline;
    color: #039BE5;
}
.mdl-menu a {
    text-decoration: none;
}
.content {
    max-width: 1024px;
}
.mdl-card {
    display: block;
}
h3 {
    background: url('firebase-logo.png') no-repeat;
    background-size: 40px;
    padding-left: 50px;
    background-position-y: -2px;
}
.mdl-textfield {
    width: 100%;
}

*/* Fixes an MDL bug where the header does not scroll on small devices */
.mdl-layout__container .mdl-layout--fixed-header .mdl-layout__content {
    overflow-y: visible;
    overflow-x: visible;
    overflow: visible;
}
*/* Overrides MDL colors */
.mdl-layout.is-upgraded .mdl-layout__tab.is-active::after,
.header .mdl-textfield__label:after {
    background-color: #FFCA28;
}
.mdl-snackbar__action {
    color: #FFCA28;
}
.mdl-textfield__label:after {
    background-color: #0288D1;
}
.mdl-textfield--floating-label.is-focused .mdl-textfield__label {
    color: #0288D1;
}

*/* Header */

.logo {
    font-family: 'Amaranth', sans-serif;
}
.logo .material-icons {
    top: 4px;
    font-size: 32px;
    margin-right: -2px;
    position: relative;
}
.header .mdl-layout__header-row {
    max-width: 1024px;
    width: 100%;
    height: auto;
    padding: 10px 20px;
    margin: auto;
    position: relative;
}
@media screen and (max-width: 840px) {
    .header .mdl-layout__header-row.titlebar {
        height: 56px;
    }
    .titlebar h3 {
        font-size: 24px;
    }
    .titlebar h3 .material-icons {
        top: 2.5px;
        font-size: 23px;
    }
}
@media screen and (max-width: 479px) {
    .mdl-grid {
        padding: 0;
    }
    .mdl-card {
        font-size: 14px;
    }
}

*/* Signed-in user */

.avatar {
    height: 32px;
    width: 32px;
    display: inline-block;
    background-size: 32px 32px;
    border-radius: 32px;
    border: 2px white solid;
    margin-right: 10px;
    background-image: url('./silhouette.jpg');
}
.username {
    display: inline-block;
    line-height: 38px;
    vertical-align: top;
    width: calc(100% - 46px);
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    text-align: left;
}
#sign-in-button {
    margin-left: 10px;
    color: inherit;
}
#sign-out-button {
    margin: 10px;
    color: inherit;
}
.mdl-button .material-icons {
    margin-top: -2px;
}
.mdl-button.mdl-button--icon .material-icons,
.mdl-button.mdl-button--fab .material-icons {
    margin-top: 0;
}

*/* Navigation Bar */

.header .mdl-tab {
    padding-left: 23px;
    box-sizing: border-box;
    width: 100%;
    height: 100%;
    overflow: visible;
    position: relative;
    margin: auto;
    max-width: 1024px;
}
@media screen and (max-width: 609px) {
    .header .mdl-tab {
        width: auto;
    }
}
.header .tab {
    padding: 0;
    max-width: none;
}
#add {
    position: absolute;
    right: 20px;
    top: 18px;
    z-index: 998;
}
@media screen and (max-width: 840px) {
    #add {
        position: fixed;
        bottom: 10px;
        right: 10px;
        z-index: 998;
        top: auto;
    }
}
#sign-out-button {
    right: 0;
    position: absolute;
}

*/* Drawer */

.mdl-layout__drawer-button {
    display: none;
}
.mdl-layout__drawer .mdl-navigation .mdl-navigation__link.is-active,
.is-active .mdl-menu__item {
    color: black;
    background-color: #EBEBEB;
}
.mdl-layout__drawer {
    border-right-width: 0;
}
.mdl-navigation__link .material-icons, .mdl-menu__item .material-icons {
    position: relative;
    margin-top: -2px;
    margin-right: 10px;
}
.mdl-menu__item .material-icons {
    top: 7px;
}
@media screen and (max-width: 479px) {
    .mdl-layout__drawer-button {
        display: block;
        top: 3px;
    }
}

*/* New Post Page */

#page-add {
    display: block;
    text-align: center;
}
#page-add .mdl-cell {
    width: auto;
    min-width: 300px;
}
#newPictureContainer {
    margin: 0;
    max-width: 100%;
    max-height: 400px;
}
@media screen and (max-width: 479px) {
    .mdl-snackbar__action {
        margin-right: 60px;
    }
}
.comments-container .username {
    width: auto;
}
.comments-container .comment{
    display: inline-block;
    vertical-align: top;
    padding-left: 10px;
    color: grey;
    line-height: 25px;
}
.comments-container .username {
    line-height: 25px;
}

*/* Post */

.post .mdl-card {
    height: 100%;
    top: 0;
    left: 0;
    min-height: 0;
}
.post .header {
    padding: 10px;
    width: calc(100% - 100px);
    display: inline-block;
}
.post .star-count {
    color: #444;
    padding: 0 10px 0 5px;
    font-weight: bold;
    display: inline-block;
    top: -10px;
    position: relative;
}
.post .comments-container {
    padding: 15px 10px 0 10px;
}
.post .text {
    padding: 0 10px;
    color: grey;
}
.post .comments-container .text {
    margin-left: 5px;
    color: #444;
    transition: all 0.2s;
}
.post .add-comment{
    flex-grow: 1;
    padding: 0 10px;
    margin-bottom: -10px;
}
.post .add-comment.mdl-textfield {
    width: 100%;
}
.post .star {
    position: absolute;
    top: 10px;
    right: 0;
}
.post .star .material-icons {
    font-size: 35px;
    color: #ffcb0c;
    cursor: pointer;
}
.post .star .material-icons:HOVER {
    opacity: 0.6;
}
.post .star .starred {
    display: none;
}

*/* Splash Page */

#page-splash {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: #0288D1;
    background: radial-gradient(circle, #039BE5, #01579b);
    z-index: 10000;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    flex-direction: column;
}
```
]



]]
.column_t1[.vmiddle.pushfront.defaultalign[

# main.css




.fonth5[]
<br/>



]]


---
class: split-70 nopadding 

.column_t2[.pushfront.defaultalign[








.fullcode[

```javascript
'use strict';

*// Shortcuts to DOM Elements.
var messageForm = document.getElementById('message-form');
var messageInput = document.getElementById('new-post-message');
var titleInput = document.getElementById('new-post-title');
var signInButton = document.getElementById('sign-in-button');
var signOutButton = document.getElementById('sign-out-button');
var splashPage = document.getElementById('page-splash');
var addPost = document.getElementById('add-post');
var addButton = document.getElementById('add');
var recentPostsSection = document.getElementById('recent-posts-list');
var userPostsSection = document.getElementById('user-posts-list');
var topUserPostsSection = document.getElementById('top-user-posts-list');
var recentMenuButton = document.getElementById('menu-recent');
var myPostsMenuButton = document.getElementById('menu-my-posts');
var myTopPostsMenuButton = document.getElementById('menu-my-top-posts');
var listeningFirebaseRefs = [];

*/**
* * Saves a new post to the Firebase DB.
* */
// [START write_fan_out]
function writeNewPost(uid, username, picture, title, body) {
  // A post entry.
  var postData = {
    author: username,
    uid: uid,
    body: body,
    title: title,
    starCount: 0,
    authorPic: picture
  };

  // Get a key for a new Post.
  var newPostKey = firebase.database().ref().child('posts').push().key;

  // Write the new post's data simultaneously in the posts list and the user's post list.
  var updates = {};
  updates['/posts/' + newPostKey] = postData;
  updates['/user-posts/' + uid + '/' + newPostKey] = postData;

  return firebase.database().ref().update(updates);
}
// [END write_fan_out]

*/**
* * Star/unstar post.
* */
// [START post_stars_transaction]
function toggleStar(postRef, uid) {
  postRef.transaction(function(post) {
    if (post) {
      if (post.stars && post.stars[uid]) {
        post.starCount--;
        post.stars[uid] = null;
      } else {
        post.starCount++;
        if (!post.stars) {
          post.stars = {};
        }
        post.stars[uid] = true;
      }
    }
    return post;
  });
}
// [END post_stars_transaction]

*/**
* * Creates a post element.
* */
function createPostElement(postId, title, text, author, authorId, authorPic) {
  var uid = firebase.auth().currentUser.uid;

  var html =
      '<div class="post post-' + postId + ' mdl-cell mdl-cell--12-col ' +
                  'mdl-cell--6-col-tablet mdl-cell--4-col-desktop mdl-grid mdl-grid--no-spacing">' +
        '<div class="mdl-card mdl-shadow--2dp">' +
          '<div class="mdl-card__title mdl-color--light-blue-600 mdl-color-text--white">' +
            '<h4 class="mdl-card__title-text"></h4>' +
          '</div>' +
          '<div class="header">' +
            '<div>' +
              '<div class="avatar"></div>' +
              '<div class="username mdl-color-text--black"></div>' +
            '</div>' +
          '</div>' +
          '<span class="star">' +
            '<div class="not-starred material-icons">star_border</div>' +
            '<div class="starred material-icons">star</div>' +
            '<div class="star-count">0</div>' +
          '</span>' +
          '<div class="text"></div>' +
          '<div class="comments-container"></div>' +
          '<form class="add-comment" action="#">' +
            '<div class="mdl-textfield mdl-js-textfield">' +
              '<input class="mdl-textfield__input new-comment" type="text">' +
              '<label class="mdl-textfield__label">Comment...</label>' +
            '</div>' +
          '</form>' +
        '</div>' +
      '</div>';

  // Create the DOM element from the HTML.
  var div = document.createElement('div');
  div.innerHTML = html;
  var postElement = div.firstChild;
  if (componentHandler) {
    componentHandler.upgradeElements(postElement.getElementsByClassName('mdl-textfield')[0]);
  }

  var addCommentForm = postElement.getElementsByClassName('add-comment')[0];
  var commentInput = postElement.getElementsByClassName('new-comment')[0];
  var star = postElement.getElementsByClassName('starred')[0];
  var unStar = postElement.getElementsByClassName('not-starred')[0];

  // Set values.
  postElement.getElementsByClassName('text')[0].innerText = text;
  postElement.getElementsByClassName('mdl-card__title-text')[0].innerText = title;
  postElement.getElementsByClassName('username')[0].innerText = author || 'Anonymous';
  postElement.getElementsByClassName('avatar')[0].style.backgroundImage = 'url("' +
      (authorPic || './silhouette.jpg') + '")';

  // Listen for comments.
  // [START child_event_listener_recycler]
  var commentsRef = firebase.database().ref('post-comments/' + postId);
  commentsRef.on('child_added', function(data) {
    addCommentElement(postElement, data.key, data.val().text, data.val().author);
  });

  commentsRef.on('child_changed', function(data) {
    setCommentValues(postElement, data.key, data.val().text, data.val().author);
  });

  commentsRef.on('child_removed', function(data) {
    deleteComment(postElement, data.key);
  });
  // [END child_event_listener_recycler]

  // Listen for likes counts.
  // [START post_value_event_listener]
  var starCountRef = firebase.database().ref('posts/' + postId + '/starCount');
  starCountRef.on('value', function(snapshot) {
    updateStarCount(postElement, snapshot.val());
  });
  // [END post_value_event_listener]

  // Listen for the starred status.
  var starredStatusRef = firebase.database().ref('posts/' + postId + '/stars/' + uid)
  starredStatusRef.on('value', function(snapshot) {
    updateStarredByCurrentUser(postElement, snapshot.val());
  });

  // Keep track of all Firebase reference on which we are listening.
  listeningFirebaseRefs.push(commentsRef);
  listeningFirebaseRefs.push(starCountRef);
  listeningFirebaseRefs.push(starredStatusRef);

  // Create new comment.
  addCommentForm.onsubmit = function(e) {
    e.preventDefault();
    createNewComment(postId, firebase.auth().currentUser.displayName, uid, commentInput.value);
    commentInput.value = '';
    commentInput.parentElement.MaterialTextfield.boundUpdateClassesHandler();
  };

  // Bind starring action.
  var onStarClicked = function() {
    var globalPostRef = firebase.database().ref('/posts/' + postId);
    var userPostRef = firebase.database().ref('/user-posts/' + authorId + '/' + postId);
    toggleStar(globalPostRef, uid);
    toggleStar(userPostRef, uid);
  };
  unStar.onclick = onStarClicked;
  star.onclick = onStarClicked;

  return postElement;
}

*/**
* * Writes a new comment for the given post.
* */
function createNewComment(postId, username, uid, text) {
  firebase.database().ref('post-comments/' + postId).push({
    text: text,
    author: username,
    uid: uid
  });
}

*/**
* * Updates the starred status of the post.
* */
function updateStarredByCurrentUser(postElement, starred) {
  if (starred) {
    postElement.getElementsByClassName('starred')[0].style.display = 'inline-block';
    postElement.getElementsByClassName('not-starred')[0].style.display = 'none';
  } else {
    postElement.getElementsByClassName('starred')[0].style.display = 'none';
    postElement.getElementsByClassName('not-starred')[0].style.display = 'inline-block';
  }
}

*/**
* * Updates the number of stars displayed for a post.
* */
function updateStarCount(postElement, nbStart) {
  postElement.getElementsByClassName('star-count')[0].innerText = nbStart;
}

*/**
* * Creates a comment element and adds it to the given postElement.
* */
function addCommentElement(postElement, id, text, author) {
  var comment = document.createElement('div');
  comment.classList.add('comment-' + id);
  comment.innerHTML = '<span class="username"></span><span class="comment"></span>';
  comment.getElementsByClassName('comment')[0].innerText = text;
  comment.getElementsByClassName('username')[0].innerText = author || 'Anonymous';

  var commentsContainer = postElement.getElementsByClassName('comments-container')[0];
  commentsContainer.appendChild(comment);
}

*/**
* * Sets the comment's values in the given postElement.
* */
function setCommentValues(postElement, id, text, author) {
  var comment = postElement.getElementsByClassName('comment-' + id)[0];
  comment.getElementsByClassName('comment')[0].innerText = text;
  comment.getElementsByClassName('fp-username')[0].innerText = author;
}

*/**
* * Deletes the comment of the given ID in the given postElement.
* */
function deleteComment(postElement, id) {
  var comment = postElement.getElementsByClassName('comment-' + id)[0];
  comment.parentElement.removeChild(comment);
}

*/**
* * Starts listening for new posts and populates posts lists.
* */
function startDatabaseQueries() {
  // [START my_top_posts_query]
  var myUserId = firebase.auth().currentUser.uid;
  var topUserPostsRef = firebase.database().ref('user-posts/' + myUserId).orderByChild('starCount');
  // [END my_top_posts_query]
  // [START recent_posts_query]
  var recentPostsRef = firebase.database().ref('posts').limitToLast(100);
  // [END recent_posts_query]
  var userPostsRef = firebase.database().ref('user-posts/' + myUserId);

  var fetchPosts = function(postsRef, sectionElement) {
    postsRef.on('child_added', function(data) {
      var author = data.val().author || 'Anonymous';
      var containerElement = sectionElement.getElementsByClassName('posts-container')[0];
      containerElement.insertBefore(
          createPostElement(data.key, data.val().title, data.val().body, author, data.val().uid, data.val().authorPic),
          containerElement.firstChild);
    });
    postsRef.on('child_changed', function(data) {	
		var containerElement = sectionElement.getElementsByClassName('posts-container')[0];
		var postElement = containerElement.getElementsByClassName('post-' + data.key)[0];
		postElement.getElementsByClassName('mdl-card__title-text')[0].innerText = data.val().title;
		postElement.getElementsByClassName('username')[0].innerText = data.val().author;
		postElement.getElementsByClassName('text')[0].innerText = data.val().body;
		postElement.getElementsByClassName('star-count')[0].innerText = data.val().starCount;
    });
    postsRef.on('child_removed', function(data) {
		var containerElement = sectionElement.getElementsByClassName('posts-container')[0];
		var post = containerElement.getElementsByClassName('post-' + data.key)[0];
	    post.parentElement.removeChild(post);
    });
  };

  // Fetching and displaying all posts of each sections.
  fetchPosts(topUserPostsRef, topUserPostsSection);
  fetchPosts(recentPostsRef, recentPostsSection);
  fetchPosts(userPostsRef, userPostsSection);

  // Keep track of all Firebase refs we are listening to.
  listeningFirebaseRefs.push(topUserPostsRef);
  listeningFirebaseRefs.push(recentPostsRef);
  listeningFirebaseRefs.push(userPostsRef);
}

*/**
* * Writes the user's data to the database.
* */
// [START basic_write]
function writeUserData(userId, name, email, imageUrl) {
  firebase.database().ref('users/' + userId).set({
    username: name,
    email: email,
    profile_picture : imageUrl
  });
}
// [END basic_write]

*/**
* * Cleanups the UI and removes all Firebase listeners.
* */
function cleanupUi() {
  // Remove all previously displayed posts.
  topUserPostsSection.getElementsByClassName('posts-container')[0].innerHTML = '';
  recentPostsSection.getElementsByClassName('posts-container')[0].innerHTML = '';
  userPostsSection.getElementsByClassName('posts-container')[0].innerHTML = '';

  // Stop all currently listening Firebase listeners.
  listeningFirebaseRefs.forEach(function(ref) {
    ref.off();
  });
  listeningFirebaseRefs = [];
}

*/**
* * The ID of the currently signed-in User. We keep track of this to detect Auth state change events that are just
* * programmatic token refresh but not a User status change.
* */
var currentUID;

*/**
* * Triggers every time there is a change in the Firebase auth state (i.e. user signed-in or user signed out).
* */
function onAuthStateChanged(user) {
  // We ignore token refresh events.
  if (user && currentUID === user.uid) {
    return;
  }

  cleanupUi();
  if (user) {
    currentUID = user.uid;
    splashPage.style.display = 'none';
    writeUserData(user.uid, user.displayName, user.email, user.photoURL);
    startDatabaseQueries();
  } else {
    // Set currentUID to null.
    currentUID = null;
    // Display the splash page where you can sign-in.
    splashPage.style.display = '';
  }
}

*/**
* * Creates a new post for the current user.
* */
function newPostForCurrentUser(title, text) {
  // [START single_value_read]
  var userId = firebase.auth().currentUser.uid;
  return firebase.database().ref('/users/' + userId).once('value').then(function(snapshot) {
    var username = snapshot.val().username;
    // [START_EXCLUDE]
    return writeNewPost(firebase.auth().currentUser.uid, username,
        firebase.auth().currentUser.photoURL,
        title, text);
    // [END_EXCLUDE]
  });
  // [END single_value_read]
}

*/**
* * Displays the given section element and changes styling of the given button.
* */
function showSection(sectionElement, buttonElement) {
  recentPostsSection.style.display = 'none';
  userPostsSection.style.display = 'none';
  topUserPostsSection.style.display = 'none';
  addPost.style.display = 'none';
  recentMenuButton.classList.remove('is-active');
  myPostsMenuButton.classList.remove('is-active');
  myTopPostsMenuButton.classList.remove('is-active');

  if (sectionElement) {
    sectionElement.style.display = 'block';
  }
  if (buttonElement) {
    buttonElement.classList.add('is-active');
  }
}

*// Bindings on load.
window.addEventListener('load', function() {
  // Bind Sign in button.
  signInButton.addEventListener('click', function() {
    var provider = new firebase.auth.GoogleAuthProvider();
    firebase.auth().signInWithPopup(provider);
  });

  // Bind Sign out button.
  signOutButton.addEventListener('click', function() {
    firebase.auth().signOut();
  });

  // Listen for auth state changes
  firebase.auth().onAuthStateChanged(onAuthStateChanged);

  // Saves message on form submit.
  messageForm.onsubmit = function(e) {
    e.preventDefault();
    var text = messageInput.value;
    var title = titleInput.value;
    if (text && title) {
      newPostForCurrentUser(title, text).then(function() {
        myPostsMenuButton.click();
      });
      messageInput.value = '';
      titleInput.value = '';
    }
  };

  // Bind menu buttons.
  recentMenuButton.onclick = function() {
    showSection(recentPostsSection, recentMenuButton);
  };
  myPostsMenuButton.onclick = function() {
    showSection(userPostsSection, myPostsMenuButton);
  };
  myTopPostsMenuButton.onclick = function() {
    showSection(topUserPostsSection, myTopPostsMenuButton);
  };
  addButton.onclick = function() {
    showSection(addPost);
    messageInput.value = '';
    titleInput.value = '';
  };
  recentMenuButton.onclick();
}, false);
```
]



]]
.column_t1[.vmiddle.pushfront.defaultalign[

# main.js




.fonth5[]
<br/>



]]

---
class: split-70 nopadding 

.column_t2[.pushfront.defaultalign[








.fullcode[

```json
{
* "post-comments" : {
    "-K_BCoYQAFT-CWqlrSoi" : {
      "-K_BCyLLzZZN_uzkv8u3" : {
        "author" : "Eueung Mulyana",
        "text" : "test comment",
        "uid" : "NxxnVoX2OfVAGaGEb52qLeHjQvp1"
      }
    }
  },
* "posts" : {
    "-K_BCoYQAFT-CWqlrSoi" : {
      "author" : "Eueung Mulyana",
      "authorPic" : "https://lh3.googleusercontent.com/-l7Tj7JpdXVo/AAAAAAAAAAI/AAAAAAAABx8/EHbAGOhag-A/photo.jpg",
      "body" : "ini budi. ini wati. wati kakaknya budi.",
      "starCount" : 0,
      "title" : "Interstellar Space",
      "uid" : "NxxnVoX2OfVAGaGEb52qLeHjQvp1"
    },
    "-K_BD4f8RPzb1dmq6FHb" : {
      "author" : "Eueung Mulyana",
      "authorPic" : "https://lh3.googleusercontent.com/-l7Tj7JpdXVo/AAAAAAAAAAI/AAAAAAAABx8/EHbAGOhag-A/photo.jpg",
      "body" : "unyil uncrit usro ndut cuplis\n",
      "starCount" : 0,
      "title" : "Another post",
      "uid" : "NxxnVoX2OfVAGaGEb52qLeHjQvp1"
    }
  },
* "user-posts" : {
    "NxxnVoX2OfVAGaGEb52qLeHjQvp1" : {
      "-K_BCoYQAFT-CWqlrSoi" : {
        "author" : "Eueung Mulyana",
        "authorPic" : "https://lh3.googleusercontent.com/-l7Tj7JpdXVo/AAAAAAAAAAI/AAAAAAAABx8/EHbAGOhag-A/photo.jpg",
        "body" : "ini budi. ini wati. wati kakaknya budi.",
        "starCount" : 0,
        "title" : "Interstellar Space",
        "uid" : "NxxnVoX2OfVAGaGEb52qLeHjQvp1"
      },
      "-K_BD4f8RPzb1dmq6FHb" : {
        "author" : "Eueung Mulyana",
        "authorPic" : "https://lh3.googleusercontent.com/-l7Tj7JpdXVo/AAAAAAAAAAI/AAAAAAAABx8/EHbAGOhag-A/photo.jpg",
        "body" : "unyil uncrit usro ndut cuplis\n",
        "starCount" : 0,
        "title" : "Another post",
        "uid" : "NxxnVoX2OfVAGaGEb52qLeHjQvp1"
      }
    }
  },
* "users" : {
    "NxxnVoX2OfVAGaGEb52qLeHjQvp1" : {
      "email" : "eueung@gmail.com",
      "profile_picture" : "https://lh3.googleusercontent.com/-l7Tj7JpdXVo/AAAAAAAAAAI/AAAAAAAABx8/EHbAGOhag-A/photo.jpg",
      "username" : "Eueung Mulyana"
    }
  }
}
```
]



]]
.column_t1[.vmiddle.pushfront.defaultalign[

# JSON Export




.fonth5[]
<br/>



]]


---
class: split-30 nopadding
background-image: url( bkgs/rambutan.jpg )

.column_t2.center[.vmiddle[
.figplaint-maxh550.opacity7[
![]( images/firebase.png)
]
]]
.column_t2[.vmiddle.nopadding[
.shadelightdark[.boxtitle1[
### 
# .fsize95[VueFire]

### Firebase bindings for Vue.js
### 
#### 
#### 
]]
]]
---
class: bkgpos_00 nopadding
background-image: url(images/fbase-13.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# Prev. Todo App with VueFire
]]

---
class: bkgpos_00 nopadding
background-image: url(images/fbase-14.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# Database Console - Data
]]

---
class: split-70 nopadding 

.column_t2[.pushfront.defaultalign[








.fullcode[

```json
{
  "todos" : {
*   "-K_EGcqwpcgGTziRodqc" : {
      "text" : "todo 1: jambu pak raden"
    },
*   "-K_EGwq_WtLXlz8uLdJ2" : {
      "text" : "todo 2: rujak bu bariyah"
    },
*   "-K_EHHe3zbGb0aiXyF4K" : {
      "text" : "todo 3: kelereng si unyil"
    }
  }
}

# --------------------------------------

*# For Comparison, Previously Equivalent:
*{
* "todos" : [
    {
      "text" : "todo 1: jambu pak raden"
    },
    {
      "text" : "todo 2: rujak bu bariyah"
    },
    {
      "text" : "todo 3: kelereng si unyil"
    }
* ]
*}

```
]



]]
.column_t1[.vmiddle.pushfront.defaultalign[

# JSON Export




.fonth5[]
<br/>



]]

---
class: split-70 nopadding 

.column_t2[.pushfront.defaultalign[








.fullcode[

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Vue.JS</title>

  <link rel="stylesheet" href="//fonts.googleapis.com/css?family=Roboto:300,400,500,700,400italic">
  <link rel="stylesheet" href="//fonts.googleapis.com/icon?family=Material+Icons">
  <link rel="stylesheet" href="//unpkg.com/vue-material@latest/dist/vue-material.css">
  <style> 
    .main-content { padding: 16px; } .red { color:red;} 
    ul {padding-left:0;} 
    li {list-style:none; line-height: 40px;} 
    .md-button {margin-left:0;}
  </style>

* <script src="https://www.gstatic.com/firebasejs/3.6.4/firebase.js"></script>
</head>

<body>

<div id="app">
  <md-toolbar> <h1 class="md-title">Learning Vue.JS</h1> </md-toolbar>
  
  <div class="main-content">
    <md-input-container>
      <label>Enter Todo</label>
      <md-input v-model="newTodo"></md-input>
    </md-input-container>
    <md-button class="md-raised md-primary" v-on:click="addTodo">Add Todo</md-button>

    <ul>
*     <li v-for="todo in todos">
*       <md-button class="md-icon-button md-warn" v-on:click="removeTodo(todo)"><md-icon>remove_circle_outline</md-icon></md-button>
        {{ todo.text }}
      </li>
    </ul>

</div></div>

<script src="//unpkg.com/vue/dist/vue.js"></script>
*<script src="//unpkg.com/vuefire/dist/vuefire.js"></script>
<script src="//unpkg.com/vue-material@latest"></script>

<script type="text/javascript">
  Vue.use(VueMaterial);
* Vue.use(VueFire);

* var config = {
*   apiKey: "AIzaSyC8TM42dWYF123_12345gvMPvYHdtEMWMc",
*   authDomain: "fbase-vue.firebaseapp.com",
*   databaseURL: "https://fbase-vue.firebaseio.com"
* };
* firebase.initializeApp(config);
* var todosRef = firebase.database().ref('todos');

  var App = new Vue({
    el: '#app',
    data: {
      newTodo: ''
    },
*   firebase: {
*     todos: todosRef.limitToLast(25)
*   },
    methods: {
      addTodo: function () {
        var text = this.newTodo.trim();
        console.log(text);
*       if (text) { todosRef.push({ text: text }); this.newTodo = ''; }
      },
*     removeTodo: function (todo) { todosRef.child(todo['.key']).remove(); }
    }
  })
</script>
</body></html>
```
]



]]
.column_t1[.vmiddle.pushfront.defaultalign[

# Code




.fonth5[]
<br/>



]]

---
class: bkgpos_00 nopadding
background-image: url(images/fbase-15.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# [Firebase + Validation - vue.js](https://vuejs.org/v2/examples/firebase.html)
]]

---
class: bkgpos_00 nopadding
background-image: url(images/fbase-16.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# Validation
]]

---
class: bkgpos_00 nopadding
background-image: url(images/fbase-17.jpg)

.shadelightdark.bottom_abs[.boxtitle1.noborder.center[
# Database Console - Data
]]

---
class: split-70 nopadding 

.column_t2[.pushfront.defaultalign[








.fullcode[

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Vue.JS</title>

  <link rel="stylesheet" href="//fonts.googleapis.com/css?family=Roboto:300,400,500,700,400italic">
  <link rel="stylesheet" href="//fonts.googleapis.com/icon?family=Material+Icons">
  <link rel="stylesheet" href="//unpkg.com/vue-material@latest/dist/vue-material.css">
  <style> 
    .main-content { padding: 16px; } .red { color:red;} 
    ul {padding-left:0;} 
    li {list-style:none; line-height: 40px;} 
    .md-button {margin-left:0;}

    .user {
      border-top: 1px solid #eee;
      overflow: hidden;
      transition: all .25s ease;
    }
    .user:last-child { border-bottom: 1px solid #eee; }

    .v-enter, .v-leave-active {
      height: 0;
      padding-top: 0;
      padding-bottom: 0;
      border-top-width: 0;
      border-bottom-width: 0;
    }

    .errors { color: #f00; }
  </style>

  <script src="https://www.gstatic.com/firebasejs/3.6.4/firebase.js"></script>
</head>

<body>

<div id="app">
  <md-toolbar> <h1 class="md-title">Learning Vue.JS</h1> </md-toolbar>
  
  <div class="main-content">

*   <md-input-container>
      <label>Username</label>
      <md-input type="text" v-model="newUser.name" placeholder="Username"></md-input>
*   </md-input-container>

*   <md-input-container>
      <label>Email</label>
      <md-input type="email" v-model="newUser.email" placeholder="email@email.com"></md-input>
*   </md-input-container>
*   <md-button class="md-raised md-primary" v-on:click="addUser">Add User</md-button>

    <ul class="errors">
      <li v-show="!validation.name">Name cannot be empty.</li>
      <li v-show="!validation.email">Please provide a valid email address.</li>
    </ul>

*   <ul is="transition-group">
      <li v-for="user in users" class="user" :key="user['.key']">
        <md-button class="md-icon-button md-warn" v-on:click="removeUser(user)"><md-icon>remove_circle_outline</md-icon></md-button>
        <span>{{user.name}} - {{user.email}}</span>
      </li>
*   </ul>

</div></div>

<script src="//unpkg.com/vue/dist/vue.js"></script>
<script src="//unpkg.com/vuefire/dist/vuefire.js"></script>
<script src="//unpkg.com/vue-material@latest"></script>

<script type="text/javascript">
  Vue.use(VueMaterial);
  Vue.use(VueFire);

  var emailRE = /^(([^<>()[\]\\.,;:\s@\"]+(\.[^<>()[\]\\.,;:\s@\"]+)*)|(\".+\"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/

  var config = {
    apiKey: "AIzaSyC8TM42dWYF123_12345gvMPvYHdtEMWMc",
    authDomain: "fbase-vue.firebaseapp.com",
    databaseURL: "https://fbase-vue.firebaseio.com"
  };
  firebase.initializeApp(config);
  var usersRef = firebase.database().ref('users');

  var App = new Vue({
    el: '#app',
    data: {
*     newUser: {
*       name: '',
*       email: ''
      }
    },
    firebase: {
      users: usersRef.limitToLast(25)
    },
    methods: {
      addUser: function () {
        if (this.isValid) {
          usersRef.push(this.newUser)
          this.newUser.name = ''
          this.newUser.email = ''
        }
      },
      removeUser: function (user) {
        usersRef.child(user['.key']).remove()
      }
    },
*   computed: {
*     validation: function () {
        return {
          name: !!this.newUser.name.trim(),
          email: emailRE.test(this.newUser.email)
        }
*     },
*     isValid: function () {
        var validation = this.validation
        return Object.keys(validation).every(function (key) {
          return validation[key]
        })
*     }
*   }
  })
</script>
</body></html>
```
]



]]
.column_t1[.vmiddle.pushfront.defaultalign[

# Code




.fonth5[]
<br/>



]]


---
class: split-30 nopadding
background-image: url( bkgs/rambutan.jpg )

.column_t2.center[.vmiddle[
.figplaint-maxh550.opacity7[
![]( images/firebase.png)
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
1. [firebase/quickstart-js: Firebase Quickstart Samples for Web](https://github.com/firebase/quickstart-js/)
1. [Firebase Web Codelab](https://codelabs.developers.google.com/codelabs/firebase-web/)
1. [Firebase Realtime Database](https://firebase.google.com/docs/database/)
1. [vuejs/vuefire: Firebase bindings for Vue.js](https://github.com/vuejs/vuefire)
1. [Firebase + Validation - vue.js](https://vuejs.org/v2/examples/firebase.html)
]
---
class: split-40 nopadding
background-image: url( bkgs/rambutan.jpg )

.column_t2.center[.vmiddle.pushfront[
.figplaint-maxh550.opacity7[
![]( images/firebase.png)
]
]]
.column_t2.shadelightdark.add-left-border.pushfront[.vmiddle.nopadding[
.boxtitle4[
### 
# .fsize95[END]

### [Eueung Mulyana](https://github.com/eueung)
### https://eueung.github.io/112016/firebase
#### CodeLabs | [Attribution-ShareAlike CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/)
#### 
]
]]

