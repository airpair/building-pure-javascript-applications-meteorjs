Back in 2012, I was starting my web development career. I already knew HTML, CSS, SQL and a bit PHP. I learned PHP and some PHP frameworks so I could build web applications. I needed to learn jQuery for front-end stuff. Then I learned front-end framework Bootstrap. After a year, I had solid knowledge of full stack web development.

## I was building applications in PHP

I was building one larger application in PHP and after a few days I needed to do some front-end features in JavaScript/jQuery. Then I was shocked. I tried to concatenate strings with .= instead of +=. I needed to google some JavaScript functions, then I got another shock. I was googling function names which I knew from PHP but they had totally different name in JavaScript.

## I found Meteor

One day, I found [Meteor.js](https://meteor.com). I tried it for one project and I wrote an article about it - [Why I love JavaScript and Meteor.js](http://meteor.hromnik.com/blog/why-i-love-javascript-and-meteor-js). I have been developing pure JavaScript applications since end of 2013. I don't need to use PHP anymore. I have tried to write one application in [Express.js](http://expressjs.com/) but then I switched back to Meteor. Express was too lightweight. I have also tried JavaScript frameworks like [Sails.js](http://sailsjs.org/), [Geddy.js](http://geddyjs.org/), [Tower.js](http://tower.github.io/) but they were either too lightweight or something did not work. Meteor worked like a charm. Moreover, Meteor is the only framework which has its own front-end solution ([Blaze](https://www.meteor.com/blaze)). You don't have to think about what front-end framework to use (Angular, Ember,...). And Meteor is real-time from scratch. If you insert or update model in database, the change is published to all connected clients in real-time, WOW.

## Key features of Meteor

- You are writting applications in pure JavaScript. Or you can use syntax suggar like CoffeeScript or LiveScript.
- Real-time from scratch. Just create/update model in database and all changes are shown for all connected clients.
- Built-in front-end solution. No need to use Angular, Ember or something else.
- [Latency compensation](https://meteorhacks.com/introduction-to-latency-compensation.html).
- Minimongo - client-side MongoDB implementation. You can work with data in client-side JavaScript.
- Isomorphic code. You can share code between client and server.
- [Packages](http://atmospherejs.com/). Meteor has its own packaging system. All Meteor packages are on [Atmosphere](http://atmospherejs.com/). Unlike NPM, Meteor packages are isomorphic. They can contain server-side and client-side code. It means that you can for example add package which will take care of [registration and logging in users](https://atmospherejs.com/meteor/accounts-ui).
- Easy deploy. You can use `meteor deploy appname` command to deploy on appname.meteor.com subdomain or [Meteor up](https://github.com/arunoda/meteor-up) tool for deploying to your own server.
- [Mobile applications](https://github.com/meteor/meteor/wiki/Meteor-Cordova-Phonegap-integration) in Meteor.
- Community. Meteor community is passionate about Meteor. Because it's the coolest stuff in the universe. There is Facebook group [Learn MeteorJS properly](https://www.facebook.com/groups/1498505377066142/). There are Meteor geeks [Arunoda](https://twitter.com/arunoda), [Josh Owens](https://twitter.com/joshowens) who brings incredible tools, articles and learning resources. There are [Meteor meetups](http://meteor.meetup.com/) all around the world.

## Learning resources for Meteor

- [Official Meteor tutorial](https://www.meteor.com/install) and [Meteor docs](http://docs.meteor.com/#/full/).
- [Meteor.js Twitter](twitter.com/meteorjs) and [Facebook](https://www.facebook.com/meteorjs).
- The first and the best book about Meteor - [Discover meteor](https://www.discovermeteor.com/). It has also [blog](https://www.discovermeteor.com/blog).
- [Metorhacks](https://meteorhacks.com/) by [Arunoda](https://twitter.com/arunoda).
- [Josh Owens blog](http://joshowens.me/).
- [Meteortips](http://meteortips.com/tutorials/) tutorials, screencasts, blog, book,...
- [Evented Mind](https://www.eventedmind.com/) screencasts.
- [Build your first real-time application with MeteorJS](udemy.com/build-your-first-real-time-web-application-with-meteorjs/) video course.
- And a lot of other resources can be found in [this blog](https://www.yauh.de/best-learning-resources-for-meteorjs/).

## Conclusion

The main advantage of writing pure JavaScript applications is avoiding context switching between server-side language and JavaScript. Another advantage is isomorphic code. Writing pure JavaScript applications can be faster than writting traditional PHP or Rails applications. I feel I am much more productive in Meteor than I was in PHP. [Josh Owens](http://differential.com/blog/meteor-killin-rails) is also much more productive in Meteor than he was in Rails.

If you try to build pure JavaScript applications, you will never get back to PHP, Rails or another mature technology.

