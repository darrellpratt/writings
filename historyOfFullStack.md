# History of the Full Stack
As applications have evolved from command line and simple GUIs, to client server and on to n-tier architectures, the technology stack of any given application has become increasingly complex. One approach to simplifying the set of technology used in any web application has driven the adoption of several sets of languages and server applications bundled together into *full stack solutions*. We will take a quick tour of the evolution of the full stack in this article and discuss the direction that web stacks might be evolving towards.

## LAMP (Linux, Apache, MySQL, PHP)
Linux, Apache, MySQL, PHP (Python or Perl) makes up this perennial top choice in the full stack arena. The full stack concept has changed how developers build web based applications because the stacks provide well defined integrations between the layers of the application. Database mapping tools and scaffolding enable the developer to easily model the domain objects of an application without needing to know the full details of the SQL required to create or query the database. PHP has a good number of object relational mapping libraries (ORM), including Eloquent ORM, Propel and Flourish. The LAMP stack has flourished because it significantly reduces the hurdle for developers to build web applications as to what it once required using enterprise tools such as J2EE.

### Progression of the Stack
LAMP has evolved from its original form and now tends to include  other technologies for the “M” including MariaDB and MongoDB, and other languages for the “P” including Perl and Python. The platform has moved onto other operating systems with simple installations on Windows (XAMPP) and OS X (MAMP). 

![](https://raw.githubusercontent.com/darrellpratt/writings/master/lampstack.png)

It will continue to a popular platform with its broad range of tools and community support, but there are new players that are challenging LAMP’s lead.

## Javascript & Node.js
The full stack scene has changed with the introduction of Node.js and the increasing popularity of JavaScript. The creation of Node.js in 2009 by Ryan Dahl marked the point in which the full stack solution could be built using one language. Based on Google’s V8 Javascript engine that is used in the Chrome web browser, Node.js takes this engine and wraps it in an asynchronous event driven model and gives the Javascript community a way to run their code at the application server tier. The module system that was created for Node.js is a key ingredient in the popularity of Node.js and has since morphed into a stand alone company, npm Inc. At last count npmjs.com hosted over 250,000 Node packages.

### Popularity 

>> **Atwood's Law**: any application that can be written in JavaScript, will eventually be written in JavaScript.

The law above was popularized by Jeff Atwood, the founder of Stack Overflow. The law has held up well since it’s first mention in 2007.  Current data on both StackOverflow and GitHub show that JavaScript sits around 14% of both code and posts on the two sites (**http://langpop.corger.nl).

Web applications have become increasingly complex on the client side, using frameworks like Angular, React, Backbone and Ember.js.  With JSON (JavaScript Object Notation) being the format of preference for AJAX requests within these frameworks, the move to JavaScript and Node.js on the server has been accelerating. At this point one stack has emerged to lead in this new space.

## MEAN
- M - MongoDB
- E - ExpressJS
- A - AngularJS
- N - Node.js

The MEAN stack proves the concept of using Javascript across an entire web application stack. We see that each member of the  stack is a JavaScript technology or works very well with JavaScript. The stack consists of the web framework, ExpressJS, a JavaScript web MVC framework, AngularJS, Node.js the JavaScript server and document NoSQL database, MongoDB. As with the earlier LAMP stack, the MEAN stack provides an integrated set of applications and frameworks with many libraries made available by the community to assist the developer with data access, security, caching, routing and other typical web application concerns.

![](https://raw.githubusercontent.com/darrellpratt/writings/master/meanstack.png)

MongoDB fits well with the stack as it provides a JSON data store and a simple querying syntax to load data into the application. MongoDB provides an official Node.js driver for the database and the community backed Mongoose package provides an excellent ODM (Object Document Mapper) tool to simplify the integration of data with the application logic.

## MERN
The elephant in the room with AngularJS 1.x has been the SEO implications of its usage. Even though the framework was written by Google, its client side rendering of content has been impacting the SEO ranking of some of the sites making heavy use of it. In addition to the SEO concern, the heavy CPU usage of the framework led Facebook to move in a different route with the React.js framework. React is quite different from AngularJS in its method for rendering HTML within  an application and makes a great replacement for the “A” of the MEAN stack. Gone is the two-way binding of data in Angular with the Virtual DOM.

The MERN stack has the same general makeup of MEAN, but the React framework does pull in some of its own environment with other controller frameworks such as Flux. The combination of React and Flux have a large community following now and will continue to pull share away from AngularJS and it’s place in the  ME*N stack.

## The Server-less Stack
A large shift that is occurring now is the move to the server-less application stack. With the introduction of Lambda by Amazon Web Services and Cloud Functions from Google, the idea of  a JavaScript function running on a cloud platform only when needed has caught the imagination of developers who have created  at least one example of an application stack that can run on-demand within the Lambda infrastructure and make use of services as needed by the application rather than requiring the developer to configure or maintain other aspects of the stack. Aptly named Serverless, the framework is growing rapidly and ready for use on AWS.

## Summary
The full stack has evolved from the original LAMP stack through to the MEAN and MERN stacks currently in vogue.  Each has brought new ideas to the concept of a holistic set of technology to easily build web applications and have increased the numbers of the individuals who work as web developers. Node.js will continue to drive a new set of full stack systems and the server-less space will merit watching for what type of innovation will be driven there.

