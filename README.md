Connect/Express URL Redirect Middleware
=======================================

Connect/Express middleware for rewriting URLs using regular expressions 
(like mod_rewrite).

Usage
-----
```javascript

// Require the middleware
rewrite = require("connect-url-rewrite");

// Build your redirect rules
rules = [
  "^\/example.html /redirected.html"
]

// Add the middleware to the stack
app.use(rewrite(rules));
```