# Space Cards

This is a flash card app to teach people about our galaxy, space, planets and stars. Using NASA's API, the search returns an image related to the text entered into the search box.

## Built With

- Bootstrap
- CSS 3
- Font Awesome
- HTML5
- Express
- AngularJS
- NASA's Open Image [API](https://api.nasa.gov/api.html#images-endpoints)
- Node.js
- npm 
- Passport.js
- PostGreSQL
## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Link to software that is required to install the app (e.g. node).

- PostGreSQL  - Can be installed using Homebrew
  * Open a terminal
  * Type ```brew install postgres``` and hit enter key
- [Postico](https://eggerapps.at/postico)
  * Create database and copy and paste the queries below
- [Node.js](https://nodejs.org/en/)
- For npm install, make sure you're in the project directory and run this code from the terminal ```npm install npm@latest -g```

### Database Setup
Steps to get the development environment running. Here are the SQL database tables.

```sql
CREATE TABLE "users" (
  "id" serial primary key,
  "username" varchar(80) not null UNIQUE,
  "password" varchar(240) not null
);

CREATE TABLE messages (
  id integer serial primary key,
  description character varying(2000) NOT NULL,
  image character varying(100) NOT NULL,
  user_id integer not null
);
```
**Run ```npm install``` in the project directory to install all project dependiencies**

## Screen Shot
![Welcome User](/images/spaceCards)


### Completed Features

High level list of items completed.

- [x] Search box
- [x] API returns image and description
- [x] Search items can be saved to the database
- [x] Flash Cards can be deleted
- [x] The flip button displays the the description on the back of the card


### Next Steps

Features that you would like to add at some point in the future.

- [ ] Angular Card Flip
- [ ] Angular Material

## Deployment


## Authors

* ale-cia
