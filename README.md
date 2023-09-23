# Node Doggy

This is a little demonstration of async/await and promises in Node JS

## Things I learned

- Spent quite a bit of time chasing down a 404 error from the API

  ```
      {
      status: 'error',
      message: 'Breed not found (master breed does not exist)',
      code: 404
      }
  ```

  The issue was an extra line in the dog.txt file where the Breed: ${data} was being pulled from. I had just done a return after putting in the word hound. Structure matters! 😉

- First exercise is to create a callback hellscape 😣
  This is where many callback functions are nested. None of them are asynchronous and things can get messy fast. Look for the "triangle" that is being made in the code with indents of nested callbacks.

  ![](./README-screenshots/callback-hell-triangle.png)

## Useful Links

[Dog CEO API](https://dog.ceo/dog-api/documentation/breed) - fun API used to generate dog images and breed names
[Super Agent ](https://www.npmjs.com/package/superagent) -
