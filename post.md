## My Background

Back in 2012, I started my web development career. I was already familiar with HTML, CSS, SQL and a bit of PHP. I had learned PHP and some PHP frameworks in order to build web applications. Then I needed to learn jQuery for front-end stuff and front-end UI framework Bootstrap for building user interface easily. After a year, I had solid knowledge of full-stack web development.

## Full-stack development in PHP

I was writing one project in PHP for a long time. Then I needed to implement some front-end features in JavaScript/jQuery. I was trying to concatenate strings with .= instead of +=. My brain couldn't switch to different syntax. When googling some JavaScript functions, I got another surprise - the function names that I was familiar with from PHP had totally different names in JavaScript.

## I found Meteor

One day, I found [Meteor.js](https://meteor.com). I tried it for one project and I wrote an article about it - [Why I love JavaScript and Meteor.js](http://meteor.hromnik.com/blog/why-i-love-javascript-and-meteor-js). I have been developing pure JavaScript applications since end of 2013. I don't need  PHP anymore. I have tried to write one application in [Express.js](http://expressjs.com/) but then I switched back to Meteor. Express was too lightweight. I have also tried JavaScript frameworks like [Sails.js](http://sailsjs.org/), [Geddy.js](http://geddyjs.org/), [Tower.js](http://tower.github.io/) but they were either too lightweight or didn't meet my needs. They have small community and thus not enough learning resources.

## What is Meteor?

Meteor is a full-stack JavaScript platform for building real-time web and mobile applications. Full-stack means that it takes care of both - front-end and back-end. Real-time means that it takes care of the whole development process - from creating application to deploy.

It's built on top of Node.js.

## Key features of Meteor

- You can write applications in pure JavaScript, or you can use syntax suggar like CoffeeScript or LiveScript.
- Real-time from scratch. Just create/update model in database and all changes are shown for all connected clients.
- [Easy to install](https://www.meteor.com/install), just one command in command line: `curl https://install.meteor.com/ | sh` and you are done.
- Built-in [front-end solution](https://www.meteor.com/blaze). No need to use Angular, Ember or something else.
- [Latency compensation](https://meteorhacks.com/introduction-to-latency-compensation.html).
- Minimongo - client-side MongoDB implementation. You can work with data in client-side JavaScript.
- Isomorphic code. You can share code between client and server.
- [Packages](http://atmospherejs.com/). Meteor has its own packaging system. All Meteor packages are on [Atmosphere](http://atmospherejs.com/). Unlike NPM, Meteor packages are isomorphic. They can contain server-side and client-side code. This means that you can, for example, add packages which will take care of [registration and logging in users](https://atmospherejs.com/meteor/accounts-ui).
- Easy deploy. You can use `meteor deploy appname` command to deploy on appname.meteor.com subdomain or [Meteor up](https://github.com/arunoda/meteor-up) tool for deploying to your own server.
- [Mobile applications](https://github.com/meteor/meteor/wiki/Meteor-Cordova-Phonegap-integration) in Meteor.
- Community. The Meteor community is super passionate about Meteor (because it's the coolest stuff in the universe). There is a Facebook group [Learn MeteorJS properly](https://www.facebook.com/groups/1498505377066142/), [Meteor meetups](http://meteor.meetup.com/) all around the world, and tons of Meteor geeks like [Arunoda](https://twitter.com/arunoda) and [Josh Owens](https://twitter.com/joshowens) who contribute incredible tools, articles and learning resources.

## Simplicity of Meteor

I know many PHP and Node.js frameworks but none of them is as simple as Meteor. Even [front-end developer can write full-stack application in Meteor](http://davidwalsh.name/meteor-frontend-engineers). You just need to know JavaScript, MongoDB, HTML, CSS and you will be able to build Meteor app. 

Meteor's code does not look like code of classic Node.js framework. It's an abstraction of Node.js and it's more beautiful.

For example client code consists of helpers, events, sessions and templates:

```javascript
Session.setDefault('counter', 0);
Template.hello.helpers({
  counter: function() {
    return Session.get('counter');
  }
});

Template.hello.events({
  'click button': function() {
    Session.set('counter', Session.get('counter') + 1);
  }
});
```
    
Hello template:

```html
<template name="hello">
  <button>Click me</button>
  <p>You have pressed the button {{counter}} times.</p>
</template>
```
    
I believe that code above is self-explanatory. You can easily find out what it does.
    
We can communicate with server via Meteor calls on the client:

```javascript
//client code
Meteor.call('sayHello', 'Tom', function(err, response) {
  if (err)
    console.log('An error ocured: ', err);
  else
    console.log('response from the server: ', response);
});
```

Server code:
    
```javascript
//server code
Meteor.methods({
  sayHello: function(name) {
    //here can be more code than just one return statement
    return 'Hello ' + name;
  }
});
```
    
Code above demonstrates communication between client and server via Meteor calls and methods. We define methods on the server and call them on the client. Read more about methods in [Meteor Docs](http://docs.meteor.com/#/full/meteor_methods).

## Learning resources for Meteor

- [Official Meteor tutorial](https://www.meteor.com/install), [Meteor Docs](http://docs.meteor.com/#/full/), [Meteor forum](https://forums.meteor.com/).
- [Meteor.js on Twitter](twitter.com/meteorjs) and [Facebook](https://www.facebook.com/meteorjs).
- The first and the best book about Meteor - [Discover Meteor](https://www.discovermeteor.com/). It also has a [blog](https://www.discovermeteor.com/blog).
- [Metorhacks](https://meteorhacks.com/) by [Arunoda](https://twitter.com/arunoda).
- [Josh Owens blog](http://joshowens.me/).
- [Meteortips](http://meteortips.com/tutorials/) with tutorials, screencasts, blog, book, etc.
- [Evented Mind](https://www.eventedmind.com/) screencasts.
- [Build Your First Real-Time Application with MeteorJS](https://www.udemy.com/build-your-first-real-time-web-application-with-meteorjs/) video course.
- Extensive article [Learn Meteor.js Properly](http://javascriptissexy.com/learn-meteor-js-properly/).
- Facebook group [Learn Meteor.js properly](https://www.facebook.com/groups/1498505377066142/).
- And a lot of other resources can be found in [this blog](https://www.yauh.de/best-learning-resources-for-meteorjs/).

## Conclusion

The main advantage of writing pure JavaScript applications is avoiding context switching between server-side language and JavaScript. Another advantage is isomorphic code. Writing pure JavaScript applications can be faster than writing traditional PHP or Rails applications. I feel I am much more productive in Meteor than I was in PHP. [Josh Owens](http://differential.com/blog/meteor-killin-rails) is also much more productive in Meteor than he was in Rails.

If you try to build pure JavaScript applications, you will never go back to PHP, Rails or another mature technology.

