# wiki

a full-stack demo

## front-end

### scaffold

The react project is created by 
```bash
npx create-react-app react-wiki-frontend
```

### routing

This is a SPA (Single Page Application), where the URL reflects current state of the application.

Routing is done with `react-router-dom` 
which utilize HTML5 history API to synchonize UI with the URL.

The homepage `'/'` is redirected to `/view/FrontPage`.

### request

`useEffect` and `axios` are used to make asynchronous requests.

#### `useEffect`

```js
useEffect(() => {
    // fetch data
    return cleaning_func;
}, [dependencies])
```

runs at component mounts and modification to dependencies (e.g. page title).

#### `axios`

a promise-based HTTP client.

## backend

The backend is a gin RESTful server

### interface

- GET `view/:title` - get the content of the page `title`
- POST `save/` - save the posted page