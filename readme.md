A template Node.js app that uses Redis to cache data.

The route in the app.js file --> app.get('/repos/:username', getRepos);
 - means you can go to the URL: 'localhost:5000' and then add '/repos/toddbrannon', for example, to the URL string -> 'localhost:5000/repos/toddbrannon'
 - you should get a return of the count of repos for the username you input

The cache middleware runs when the 'getRepos' function is called and therefore retains the URL in the Redis cache for the duration of the setex timeout value.

