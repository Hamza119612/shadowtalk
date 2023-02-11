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

### User Management

-   `POST /register` - Register a new user.
-   `POST /login` - Log in an existing user.
-   `PUT /profile` - Update the user's profile information.
-   `GET /profile/:id` - Retrieve the profile information of the user with the given ID.

### Personalized Feed

-   `GET /feed` - Retrieve the personalized feed for the authenticated user.
-   `POST /post` - Create a new post.
-   `DELETE /post/:id` - Delete a post with the given ID.
-   `PUT /post/:id` - Update a post with the given ID.
-   `GET /post/:id` - Retrieve a post with the given ID.
-   `POST /post/:id/like` - Like a post with the given ID.
-   `DELETE /post/:id/like` - Unlike a post with the given ID.
-   `POST /post/:id/comment` - Comment on a post with the given ID.
-   `DELETE /post/:id/comment/:commentId` - Delete a comment with the given ID on a post with the given ID.

### Virtual Events

-   `GET /events` - Retrieve a list of all virtual events.
-   `GET /event/:id` - Retrieve information about a virtual event with the given ID.
-   `POST /event` - Create a new virtual event.
-   `PUT /event/:id` - Update a virtual event with the given ID.
-   `DELETE /event/:id` - Delete a virtual event with the given ID.
-   `POST /event/:id/rsvp` - RSVP to a virtual event with the given ID.

### Multi-Language Support

-   `GET /languages` - Retrieve a list of all supported languages.
-   `POST /language` - Set the preferred language for the authenticated user.

### E-commerce Integration

-   `GET /products` - Retrieve a list of all products.
-   `GET /product/:id` - Retrieve information about a product with the given ID.
-   `POST /product` - Create a new product.
-   `PUT /product/:id` - Update a product with the given ID.
-   `DELETE /product/:id` - Delete a product with the given ID.
-   `POST /product/:id/purchase` - Purchase a product with the given ID.

### Social Causes

-   `GET /causes` - Retrieve a list of all social causes.
-   `GET /cause/:id` - Retrieve information about a social cause with the given ID.
-   `POST /cause` - Create a new social cause.
-   `PUT /cause/:id` - Update a social cause with the given ID.
-   `DELETE /cause/:id` - Delete a social cause with the given ID.
-   `POST /cause/:id/donate` - Donate to a social cause with the given ID.

### Podcast Integration

- `GET /podcasts` - Retrieve a list of all podcasts. This endpoint will return a list of all available podcasts, along with basic information such as the title, description, and author.

- `GET /podcast/:id` - Retrieve information about a podcast with the given ID. This endpoint will return detailed information about a specific podcast, including its title, description, author, and any associated content such as audio files or images.

- `POST /podcast` - Create a new podcast. This endpoint will allow users to create a new podcast by submitting the necessary information, including the title, description, author, and any associated content.

- `PUT /podcast/:id` - Update an existing podcast. This endpoint will allow users to modify an existing podcast by submitting updated information, such as changes to the title, description, author, or content.

- `DELETE /podcast/:id` - Delete a podcast. This endpoint will allow users to delete an existing podcast, removing it from the list of available podcasts.

### AI-based Chatbot

- `GET /chatbot` - Retrieve chatbot information. This endpoint will return information about the AI-based chatbot, including its capabilities and features.

- `POST /chatbot` - Interact with the chatbot. This endpoint will allow users to interact with the chatbot by submitting messages and receiving responses. The chatbot will use natural language processing and machine learning algorithms to generate its responses.


## Deployment
- GitHub Actions is used for building and deploying the application to a production environment.

## Maintenance
- The application is monitored for errors and performance issues
- Bugs are fixed and new features are added as needed
- Regular updates


