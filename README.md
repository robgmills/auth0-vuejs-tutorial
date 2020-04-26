# Auth0 VueJS Tutorial

Essentially the output of the [official Auth0 quickstart for Vue](https://auth0.com/docs/quickstart/spa/vuejs) - but with a few minor tweaks.

This was my first foray into VueJS and first hands-on coding experience using Auth0 (I had previous business experience).

## Quickstart

```sh
pushd api
npm run api
popd

pushd front-end
npm run serve
popd

open "http://localhost:8080"
```

## Differences from official tutorial

### Separate front- and back-ends
I separated the Vue single-page application from the API so that I could deploy them to Amazon Web Services (AWS) independently.

### Front-end doesn't proxy API requests
In my use-case, I expect to host and serve my front-end separate from my API.
When serving my front-end, I don't want to have to run a potentially unnecessary middleware layer to proxy requests to the API to avaid cross-origin resource sharing.
This approach allowed me to figure out an approach to CORS locally.

### Minor UI changes
I changed things like the navigation and location of the login and logout buttons from the official tutorial.
