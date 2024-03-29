#Firebase

##Table of contents
<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [Introduction](#introduction)
- [How to install](#how-to-install)
  - [CLI](#cli)
    - [Bower](#bower)
    - [Npm](#npm)
    - [CDN](#cdn)
- [How to use](#how-to-use)
  - [Web](#web)
    - [AngularFire (AngularJS)](#angularfire-angularjs)
    - [EmberFire (Ember)](#emberfire-ember)
    - [BackboneFire (Backbone.js)](#backbonefire-backbonejs)
    - [ReactFire (ReactJS)](#reactfire-reactjs)
    - [Ionic](#ionic)
  - [Mobile](#mobile)
    - [iOS](#ios)
    - [Android](#android)
  - [REST](#rest)
- [Account](#account)
  - [Login](#login)
    - [Email & Password](#email-&-password)
    - [Facebook](#facebook)
    - [Twitter](#twitter)
    - [Github](#github)
    - [Google](#google)
    - [Anonymous](#anonymous)
    - [Custom](#custom)
  - [Security & Rules](#security-&-rules)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->
##Introduction

Firebase can power your app's backend, including data storage, user authentication, static hosting, and more. We provide these services so you can focus on creating extraordinary user experiences.

###### Realtime Database
Store & sync data with our NoSQL cloud database. Data is stored as JSON, synced to all connected clients in realtime, and available when your app goes offline.

###### Authentication
Authenticate users with email & password, Facebook, Twitter, GitHub, Google, anonymous auth, or easily integrate with your existing authentication system.

###### Hosting
Deploy your web app in seconds with our production-grade static asset hosting. From acquiring the SSL cert to serving your content on our global CDN, we do it all for you.

## How to install

### CLI

#### Bower

```bash
$ bower install firebase --save
```

#### Npm
```bash
$ npm install firebase --save
```

#### CDN
```javascript
<script src="https://cdn.firebase.com/js/client/2.3.2/firebase.js"></script>
```

## How to use

## Create an account

The first thing you need to do to get started with Firebase is sign up for a free account. A brand new Fase app will automatically be created for you with its own unique database URL ending in `firebaseio.com`. We'll use this database URL to store and sync data.

### Web

#### AngularFire (AngularJS)

AngularFire is the officially supported AngularJS binding for Firebase. Firebase is a full backend so you don't need servers to build your Angular app!

AngularFire is a complement to the core Firebase client. It provides you with three Angular services:
  * `$firebaseObject` - synchronized objects
  * `$firebaseArray` - synchronized collections
  * `$firebaseAuth` - authentication, user management, routing

  ##### Downloading AngularFire

  In order to use AngularFire in your project, you need to include the following files in your HTML

  ```html
  <!-- AngularJS -->
  <script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/angularjs/1.4.6/angular.min.js"></script>

  <!-- Firebase -->
  <script type="text/javascript" src="https://cdn.firebase.com/js/client/2.3.0/firebase.js"></script>

  <!-- AngularFire -->
  <script type="text/javascript" src="https://cdn.firebase.com/libs/angularfire/1.1.3/angularfire.min.js"></script>
  ```

  You can also install AngularFire via npm and Bower and its dependencies will be downloaded automatically

  ```bash
  $ npm install angularfire --save
  ```

  ```bash
  $ bower install angularfire --save
  ```

  Once we have our libraries installed, we can include the AngularFire services by declaring `firebase` as a module dependency in our application.

  ```javascript
  var app = angular.module("sampleApp", ['firebase']);
  ```

  We now will have access to thress services provided by AngularFire: `$firebaseObject`, `$firebaseArray` and `$firebaseAuth`. To use these services, we nedd to inject then into a controller, factory or service.

  ```javascript
  app.controller("SampleController", ["$scope", "$firebaseArray",
    function($scope, $firebaseArray){
        // ...
      }
    ]);
  ``

#### EmberFire (Ember)

> EmberFire is the officially supported adapter for using Firebase with Ember Data. The DS.FirebaseAdapter provides all of the standard DS.Adapter methods and will automatically synchronize the store with a Firebase database.

#### BackboneFire (Backbone.js)

> BackboneFire is the officially supported Backbone binding for Firebase. The bindings let you use special model and collection types that will automatically synchronize with Firebase, and also allow you to use regular Backbone.Sync based synchronization methods.

#### ReactFire (ReactJS)

> ReactJS is a framework for building large, complex user interfaces. Firebase complements it perfectly by providing an easy-to-use, realtime data source for populating the state of React components. With ReactFire, it only takes a few lines of JavaScript to integrate Firebase into React apps via the ReactFireMixin.

#### Ionic

> Ionic is a front-end SDK for developing hybrid mobile apps with HTML5. Because Ionic uses Angular, developers can use AngularFire to easily wire up a Firebase backend with an Ionic app.

### Mobile

#### iOS

#### Android

### REST

## Account

### Login

#### Email & Password

#### Facebook

#### Twitter

#### Github

#### Google

#### Anonymous

#### Custom

### Security & Rules
