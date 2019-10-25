# Frontend Developer Project

This project is a demo project setup for candidates who are applying for frontend UI/UX developer role at [Quaero 3 India](www.quaero.com). Please clone this project and follow the steps mentioned in the test shared with you. 


### How to run this?

1. Download [node](https://nodejs.org/en/). For a step by step process see [this](https://docs.npmjs.com/getting-started/installing-node).
2. `cd <your-proect-folder>` and type `npm install` in you terminal.
3. finally type `node .`

You would see something like this in you terminal
```
User 1:  [ {
      username: 'User 1',
      password: '$2a$10$5mdfxBnr9YDURhOohjM.iO175XgNXelP.3kyN50YGwN/iSE7RlHxu',
      email: 'user1@quaero.com',
      id: 1
    },
  false ]
User 2:  [ {
      username: 'User 2',
      password: '$2a$10$aLYbkFoJUU1l0ZEM5IFAuOMl2NkUC.dCT8cAqwZJygrRGs3LQQWxK',
      email: 'user2@quaero.com',
      id: 2
    },
  false ]
Web server listening at: http://0.0.0.0:3000
Browse your REST API at http://0.0.0.0:3000/explorer
```
Now you have your server up and running. Now just redirect to `http://0.0.0.0:3000` and you would see a success message something like this `{"started":"2016-10-27T17:44:16.743Z","uptime":568.03}`

### Client folder setup

This project helps you with all backend setup and seed data, but to pass the frontend developer test you need to setup
the client folder and create angular app. For details how to setup the client folder you can follew this [tutorial](http://loopback.io/doc/en/lb2/AngularJS-JavaScript-SDK.html)

### Test Requirements

1. This project creates three [loopback models](http://loopback.io/doc/en/lb2/Defining-models.html) for you `User`,`Category` and Sub-category`. 
2. You have two seed user data in you backend which you can use for login and testing. (You still need to create signup form)
3. Sub-category belongs to Category model as defined in [loopback relations](http://loopback.io/doc/en/lb2/Creating-model-relations.html) and Category is a kind of parent model for Sub-category model. 
4. You can map Sub-category to Category for understanding purpose through loopback-explorer. Just go to http://0.0.0.0:3000/explorer and try creating the relationships. [More](http://loopback.io/doc/en/lb2/Use-API-Explorer.html)

### Problem Statement

Category and Sub-category both have a property named as `type` which defines what type of category it is. Sub-category has an extra property as `parent-type` which just stores its parent category type. Sub-category type depends on its parent category so in html form when you are trying to create a Sub-category the values should be filtered based on parent category type.

Here is the list of category and their Sub-category types: 
```
1. Electronics 
	* Tv
	* AC
	* Mobiles
	* Laptops
2. Fashion 
	* Shirts
	* Trousers
	* Jackets
	* Kurta
3. Furniture 
	* Bed
	* Sofa
	* Chair
	* Wardrobes
4. Home Decors 
	* Wall clock
	* Wallpapers
	* Curtains
5. Automobiles 
	* Engine Oil
	* Car Wax
	* Bike Lock
	* Headgear

```

If you have any further questions just drop a mail at indiahr@quaero.com and we will help you.





