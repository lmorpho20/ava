# Avakitchen.com Netlify URL Shortener and Redirect App

## The Scope

To develop a Netlify function and app that will take the url "https://avakitchen.com" and generate a Netlify domain redirect such as "https://avakitchen.netlify.app/".

## The Basics

There are two ways to use this app.

### The Url Builder
For basic redirects, change the html address to start with **https://avakitchen.netlify.app/.netlify/functions/redirect?url=** then the url to redirect to.

example:
https://avakitchen.netlify.app/.netlify/functions/redirect?url=https://avakitchen.com/baked-catfish-with-herbs/



### The Node method

1. install [node.js](https://nodejs.org/en/download/)
2. [Clone the git repository to your drive](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)
3. run terminal from the the repo
4. enter this in your terminal:
```
node run shorten (the long url) (the shortened text)

```

example: 

```

node run shorten https://avakitchen.com/baked-catfish-with-herbs/ baked-catfish-with-herbs

```

this will create an entry in the ***_redirect*** file then commit the changes to github.


### Edit from Github Repo

1. edit the _redirects file in the parent directory.

example: ``` /texas-chocolate-quarter-sheet-cake   https://avakitchen.com/texas-chocolate-quarter-sheet-cake/ ```

