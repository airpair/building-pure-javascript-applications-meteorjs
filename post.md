## 1. My Background 

Back in 2012, I started my web development career. I was already familar with HTML, CSS, SQL and a bit of PHP. I had learned PHP and some PHP frameworks in order to build web applications, but I still needed to learn jQuery for front-end stuff, so I learned front-end framework, Bootstrap. After a year, I had solid knowledge of full stack web development.

## 2. First Experience of Javascript

It was when I found myself building a large application in PHP that I came across JavaScript/jQuery for the first time. It was when I was trying to implement some front-end features in JavaScript/jQuery that I got my first big surprise, trying and failing to concatenate strings with .= instead of +=. When googling some JavaScript functions, I got another surprise - the function names that I was familiar with from PHP had totally different names in JavaScript.

## 3. First Experience of Meteor

I came across [Meteor.js](https://meteor.com) shortly after that. I used it in a project and I [fell in love](http://meteor.hromnik.com/blog/why-i-love-javascript-and-meteor-js), so much so that I don't use PHP anymore, and have been developing pure JavaScript applications ever since. 

I have tried to write applications in [Express.js](http://expressjs.com/), as well as other JavaScript frameworks like [Sails.js](http://sailsjs.org/), [Geddy.js](http://geddyjs.org/), and [Tower.js](http://tower.github.io/) but I've always switched back to Meteor. They were either too lightweight or they didn't meet my needs. 

## 4. Key Features of Meteor

- Meteor is the only framework that has it's own built-in front-end solution ([Blaze](https://www.meteor.com/blaze)), so you don't have to think about what front-end framework to use (Angular or Ember etc.).
- You can write applications in pure JavaScript, or you can use syntax sugar like CoffeeScript or LiveScript.
- Real-time from scratch. Just create/update model in database and all changes are shown for all connected clients.
- [Latency compensation](https://meteorhacks.com/introduction-to-latency-compensation.html).
- Minimongo - client-side MongoDB implementation. You can work with data in client-side JavaScript.
- Isomorphic code. You can share code between client and server.
- [Packages](http://atmospherejs.com/). Meteor has its own packaging system. All Meteor packages are on [Atmosphere](http://atmospherejs.com/). Unlike NPM, Meteor packages are isomorphic. They can contain server-side and client-side code. This means that you can, for example, add packages that will take care of [registration and logging in users](https://atmospherejs.com/meteor/accounts-ui).
- Easy deploy. You can use `meteor deploy appname` command to deploy on appname.meteor.com subdomain or [Meteor up](https://github.com/arunoda/meteor-up) tool for deploying to your own server.
- [Mobile applications](https://github.com/meteor/meteor/wiki/Meteor-Cordova-Phonegap-integration) in Meteor.
- Community. The Meteor community is super passionate about Meteor (because it's the coolest stuff in the universe). There is a Facebook group [Learn MeteorJS properly](https://www.facebook.com/groups/1498505377066142/), [Meteor meetups](http://meteor.meetup.com/) all around the world, and tons of Meteor geeks like [Arunoda](https://twitter.com/arunoda) and [Josh Owens](https://twitter.com/joshowens) who contribute incredible tools, articles and learning resources.  

## 5. Learning Resources for Meteor

- [Official Meteor Tutorial](https://www.meteor.com/install) and [Meteor Docs](http://docs.meteor.com/#/full/).
- [Meteor.js on Twitter](twitter.com/meteorjs) and [Facebook](https://www.facebook.com/meteorjs).
- The first and the best book about Meteor - [Discover Meteor](https://www.discovermeteor.com/). It also has a [blog](https://www.discovermeteor.com/blog).
- [Metorhacks](https://meteorhacks.com/) by [Arunoda](https://twitter.com/arunoda).
- [Josh Owens' blog](http://joshowens.me/).
- [Meteortips](http://meteortips.com/tutorials/) with tutorials, screencasts, blog, book etc.
- [Evented Mind](https://www.eventedmind.com/) screencasts.
- [Build Your First Real-Time Application with MeteorJS](udemy.com/build-your-first-real-time-web-application-with-meteorjs/) video course.
- And a lot of other resources can be found in [this blog](https://www.yauh.de/best-learning-resources-for-meteorjs/).

## 6. Conclusion

The main advantage of writing pure JavaScript applications is avoiding context switching between server-side language and JavaScript. Another advantage is isomorphic code. Writing pure JavaScript applications can be faster than writing traditional PHP or Rails applications. I feel I am much more productive in Meteor than I was in PHP. [Josh Owens](http://differential.com/blog/meteor-killin-rails) is also much more productive in Meteor than he was in Rails.

If you try to build pure JavaScript applications, you will never go back to PHP, Rails or another mature technology.

