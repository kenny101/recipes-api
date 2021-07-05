# Recipes-API

An API with a large collection of recipes collected from youtube videos. Each property of a JSON object includes the video's title, image url, list of ingredients as a string, video url, and unique id.

- API Endpoint URL Here: https://recipes-database-api.herokuapp.com/yt-recipes

- Here's the script I made to collect this data: https://github.com/kenny101/Youtube-Recipes-Dataset-with-Ingredients

- RESTful API created using: https://github.com/typicode/json-server

- Hosted with Heroku: https://recipes-database-api.herokuapp.com/

# Dependencies:
```bash
npm install node-fetch
```

# Example Code Snippet:

```js
const fetch = require("node-fetch");
const api_url = "https://recipes-database-api.herokuapp.com/yt-recipes";

fetch(api_url)
  .then(function (res) {
    return res.json();
  })
  .then(function (data) {
    console.log(data);
  });
```

# Example of JSON Data:

![Figure 1-1](example.jpg)
