Hello World!
# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

# Your challenge:

We have a site that displays users from our jsonplaceholder website.

For this challenge, we're going to display todos from users using the JSONPlaceholder API. You should be familiar with this API from past exercises.

### Success Criteria
#### Functionality:

- Users load from https://jsonplaceholder.typicode.com/users and are displayed on the page.
- The page displays the name of the user
- When the user is clicked, the user's posts are fetched from https://jsonplaceholder.typicode.com/users/${userId}/todos.
- The page displays the title property of all the todos for a user after clicking on the user's name.
### Specific Instructions and helpful tips
#### Users have this structure:
```js {
  "id": 1,
  "name": "Leanne Graham",
  "username": "Bret",
  "email": "Sincere@april.biz",
  "address": {
    "street": "Kulas Light",
    "suite": "Apt. 556",
    "city": "Gwenborough",
    "zipcode": "92998-3874",
    "geo": {
      "lat": "-37.3159",
      "lng": "81.1496"
    }
  },
  "phone": "1-770-736-8031 x56442",
  "website": "hildegard.org",
  "company": {
    "name": "Romaguera-Crona",
    "catchPhrase": "Multi-layered client-server neural-net",
    "bs": "harness real-time e-markets"
  }
  ```

- You will only need to show the user's name, but you will need the userId to query for the todos
- Your solution should handle multiple todos
#### The todos have the following structure:
```js {
  "userId": 5,
  "id": 84,
  "title": "sunt veritatis ut voluptate",
  "completed": false
}
```

- A user's todos should only show after the user's name is clicked.

- All information can be displayed on the same page.

- The tests will first check that the users load and then check if the todos load once a user's name is clicked.