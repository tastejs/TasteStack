# TasteStack

> Compare backend stack implementations


## Implementations

- Node.js, Google App Engine, and gcloud - [Source](https://github.com/GoogleCloudPlatform/gcloud-node-todos), [Demo](http://gcloud-todos.appspot.com)
- Python, Google App Engine, and Morepath - [Source](https://github.com/webmaven/appengine-todos-morepath)
- Symfony, Chaplin.js, and Backbone.js - [Source](https://github.com/dunglas/DunglasTodoMVCBundle)


### Creating a Backend Implementation

Your implementation will not directly modify TodoMVC. Instead, it will only respond to API requests prefixed with `/api/` following the [specification](https://github.com/tastejs/todomvc-api/blob/master/todos.apib).

#### Node.js
If Node.js is a part of your implementation's stack, you may use [todomvc-api (npm)](https://npmjs.org/package/todomvc-api) to validate your API, then [todomvc (npm)](http://npmjs.org/package/todomvc) to pull in the front-end dependencies and [Express](http://expressjs.com/) server. *If your own project involves Express, see [gcloud-node-todos](https://github.com/GoogleCloudPlatform/gcloud-node-todos/blob/master/server.js#L13) for an example.*

The TodoMVC frontend implementations (e.g. AngularJS, Backbone.js, etc) can be brought into your project as a dependency via [npm](http://npmjs.org/package/todomvc) or git.

#### Other Backend Architectures
If you're not sure where to begin for Framework/Language "X", please open an issue so we can help guide you.

#### Being Featured
To be featured on [TodoMVC.com](https://todomvc.com), you will need to maintain a hosting environment for us to link to. If that is not possible, we will still gladly feature a link from this document.
