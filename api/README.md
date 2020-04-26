# API

## Quickstart

```sh
npm install // install the NPM dependencies
npm run api // run the API application on port 3001
```

## Exposed APIs

### `/api/external`

```sh
curl -H "Authorization: Bearer $TOKEN" http://localhost:3001/api/external

{
    msg: "Your Access Token was successfully validated!"
}
```