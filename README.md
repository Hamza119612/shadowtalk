# ShadowTalk

ShadowTalk is a social media web application that allows users to share posts anonymously and interact with other users.

## Tech Stack
- React.js for building the front-end
- Node.js, Express.js for building the back-end
- MongoDB for storing data
- Mongoose for interacting with the database
- Passport.js for handling user authentication and authorization
- JWT for securely transmitting information between parties
- Webpack for bundling assets
- Babel for transpiling JavaScript
- ESLint for enforcing coding style
- Jest for unit testing
- Axios for making API calls
- Socket.io for real-time communication
- GitHub Actions for building and deploying the application

## Features
- User registration and login
- Profile creation and editing
- Post creation, deletion, and editing
- Anonymous posting
- User interactions such as likes and comments
- Personalized content feeds
- Virtual events
- Multi-language support
- E-commerce integration
- Social causes
- Podcast integration
- AI-based chatbot

## APIs 

#### User Management:
- Register: Allows a new user to sign up with their basic information (username, password, email, etc.).
- Login: Allows an existing user to log in with their credentials.
- Profile: Allows a user to view and edit their profile information (username, password, email, profile picture, etc.).


#### Post Management:
- Create Post: Allows a user to create a new post and share it with other users.
- View Posts: Allows a user to view a list of posts and filter them based on different criteria (e.g. date, popularity, etc.).
- Edit Post: Allows a user to edit an existing post.
- Delete Post: Allows a user to delete an existing post.


#### Interactions:
- Like Post: Allows a user to like a post.
- Comment on Post: Allows a user to comment on a post.
- View Likes: Allows a user to view the number of likes a post has received.
- View Comments: Allows a user to view the comments on a post.


#### Personalized Feed:
- View Feed: Allows a user to view a personalized feed of posts based on their interests and interactions.
- Update Feed Preferences: Allows a user to update the preferences that determine their feed (e.g. interests, interactions, etc.).


#### Virtual Events:
- Create Event: Allows a user to create a new virtual event.
- View Events: Allows a user to view a list of virtual events and filter them based on different criteria (e.g. date, popularity, etc.).
- RSVP to Event: Allows a user to RSVP to a virtual event.
- View RSVPs: Allows a user to view the number of RSVPs an event has received.


#### Multi-Language Support:
- Translate: Allows a user to translate a post or comment into a different language.
- View Translation: Allows a user to view a translation of a post or comment.


#### E-commerce Integration:
- Add to Cart: Allows a user to add an item to their shopping cart.
- View Cart: Allows a user to view the items in their shopping cart.
- Checkout: Allows a user to checkout and purchase the items in their shopping cart.


#### Social Causes:
 - Donate: Allows a user to make a donation to a social cause.
- View Causes: Allows a user to view a list of social causes and filter them based on different criteria (e.g. popularity, etc.).


#### Podcast Integration:
- Subscribe: Allows a user to subscribe to a podcast.
- View Podcasts: Allows a user to view a list of podcasts and filter them based on different criteria (e.g. popularity, etc.).
- Listen to Podcast: Allows a user to listen to a podcast episode.


#### AI-based Chatbot:
- Chat with Chatbot: Allows a user to chat with an AI-based chatbot and get answers to their questions.


## API Reference

### User Registration API
- Method: POST
- Endpoint: /api/users/register
- Body:
{
"name": "User Name",
"email": "user@example.com",
"password": "password123"
}
- Description: This API is used to register a new user by providing a name, email and password. The API will return a success message if the registration is successful and an error message if it fails.

#### Login User

- Method: POST
- Endpoint: /api/users/login
- Body:
{
"email": "user@example.com",
"password": "password123"
}
- Description: This API is used to log in an existing user by providing an email and password. The API will return a JWT token if the login is successful and an error message if it fails.

### Profile Management

#### View Profile

- Method: GET
- Endpoint: /api/profile
- Description: This API is used to view the profile of the logged-in user. It requires an authorization token to be passed in the header.

#### Update Profile

- Method: PUT
- Endpoint: /api/profile
- Body:
{
"name": "Updated User Name",
"email": "updateduser@example.com"
}
- Description: This API is used to update the profile of the logged-in user. It requires an authorization token to be passed in the header.

### Post Management

#### Create Post

- Method: POST
- Endpoint: /api/posts
- Body:

{
"text": "This is my new post"
}
- Description: This API is used to create a new post by providing text. The API will return the created post if it is successful and an error message if it fails.

#### View Posts

- Method: GET
- Endpoint: /api/posts
- Description: This API is used to view all posts.

#### View Post

- Method: GET
- Endpoint: /api/posts/:id
- Description: This API is used to view a specific post by its ID.

#### Update Post

- Method: PUT
- Endpoint: /api/posts/:id
- Body:
{
"text": "This is my updated post"
}

- Description: This API is used to update a specific post by its ID.

#### Delete Post

- Method: DELETE
- Endpoint: /api/posts/:id
- Description: This API is used to delete a specific post by its ID.


## Deployment
- GitHub Actions is used for building and deploying the application to a production environment.

## Maintenance
- The application is monitored for errors and performance issues
- Bugs are fixed and new features are added as needed
- Regular updates


