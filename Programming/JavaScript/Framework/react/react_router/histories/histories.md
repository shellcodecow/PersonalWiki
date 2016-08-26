## Histories [Back](./../react_router.md)

A history knows how to listen to the browser's address bar for changes and parses the URL into a `location` object that the router can use to match routes and render the correct set of components.

In React Router, there are 3 types of histories which are come across most often:

- `browserHistory`
- `hashHistory`
- `createMemoryHistory`

### Usage

Just import them separately and pass them into a `<Router>`:

{%ace edit=false, lang='jsx', theme='tomorrow'%}
import React from 'react';
import ReactDOM from 'react-dom';
import { browserHistory } from `react-router`;

ReactDOM.render(
    <Router history={browserHistory} routes={routes}></Router>,
    document.getElementById('content')
);
{%endace%}

### `browserHistory`

Browser history is recommended to used in a **browser application** with React Router.