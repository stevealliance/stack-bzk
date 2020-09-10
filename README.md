# Bazookka tech


## Projects 
=========
```text
Bazookka commercial website 
Bazookka job and internship management service 
Bazookka AI color friendly service 
```

## Stack

### Backend

```text
NodeJS
Python
Goland
```
### Frontend

```text
React 
Vues
```

## Tools

```text
Strapi
JIRA 
GIT
Google suit
Atlassian
```

## Links 

1. [Install NodeJS English](https://nodejs.org/en/)
1. [Install NodeJS Francais](https://nodejs.org/fr/)

## NodeJS 
By example 


Creating first node project

```terminal
npm init 
```

install ExpressJS to run a small footprint 
```terminal
npm i express --save
```

Create file `index.js` and add the following code
```javascript
const express = require('express')
const route = require('./route')
const app = express()

app.use("/", route)


app.listen("5005")
```

Create a *route.js* file to contain all routes function
In this file we have some example using async await + Promises.


```javascript
const route = require('express').Router()

function time(v, t){
    return new Promise(function(resolve, reject){
        setTimeout(()=> {
            resolve(v)
        }, t)
    });

}

async function charles(v, t){
    let response = await time(v, t)
    return response;
}


route.get('/', async (request, response) => {
    console.log("one")
    charles("Hey binu", 5000).then( r => {
        console.log(r)
    })
    console.log(await charles("hey felix", 4500))
    console.log("three")

    response.send({message: "chat"})
})


module.exports = route

```

## Video

1. [NodeJS Crash course](https://www.youtube.com/watch?v=U8XF6AFGqlc) 
1. [NodeJS Another course](https://www.youtube.com/watch?v=ENrzD9HAZK4)
1. [NodeJS API with mongodb](https://www.youtube.com/watch?v=fsCjFHuMXj0)


1. [NodeJS API intro en francais eps 1](https://www.youtube.com/watch?v=6F1kvoHgjNY)
1. [NodeJS API intro en francais eps 2](https://www.youtube.com/watch?v=7Ym-GxeR-HI)
1. [NodeJS API intro en francais eps 3](https://www.youtube.com/watch?v=hggvCij14F0)
1. [NodeJS API intro en francais eps 4](https://www.youtube.com/watch?v=NPJms-kg2F8)


# React intro 


Since in the previous day we installed 'npm' and 'node'
You can use the following command line
```terminal
npx create-react-app [the name the app]
```
This will allow you to have a start up React app.

```terminal
npm run start
```
This command will use port 3000 in your default browser
all code can be found in this repo [course](https://github.com/stevealliance/bzk-course)
# 

## Video

1. [React video tutorial](https://www.youtube.com/watch?v=-MlNBTSg_Ww&t=137s)



