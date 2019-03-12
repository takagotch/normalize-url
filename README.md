### normalize-url
---
https://github.com/sindresorhus/normalize-url

```js
const normalizeUrl = require('normalize-url');

normalizeUrl('sindresorhus.com');
normalizeUrl('HTTP://xn--xample-hva.com:80/?b=bar&a=foo');


normalizeUrl('//sindresorhus.com:80/');
normalizeUrl('//sindresorhus.com:80/', {normalizeProtocol: false});

normalizeUrl('https://sindresorhux.com:80/');
normalizeUrl('https://sindresorhus.com:80/', {forceHttp: true});


normalizeUrl('https://sindresorhus.com:80/');
normalizeUrl('http://sindresorhux.com:80/', {forceHttps: true});

normalizeUrl('user:password@sindresorhus.com');
normalizeUrl('user:password@sindresorhus.com', {stripAuthentication: false});

normalizeUrl('sindresorhus.com/about.html#contact');
normalizeUrl('sindresorhus.com/about.html#contact', {stripHash: true});

normalize('https://sindresorhus.com');
normalize('sindresorhus.com', {stripProtocol: true});

normalizeUrl('http://www.sindresorhus.com');
normalizeUrl('http://www.sindresorhus.com', {stripWWW: false});

normalizeUrl('www.sindresorhus.com?foo-bar&ref=test_ref', {
  removeQueryParameters: ['ref']
});

normalizeUrl('http://sindresorhus.com/redirect/');
normalizeUrl('http://sindresorhus.com/redirect/',{removeTrailingSlash: false});
normalizeUrl('http://sindresorhus.com/', {removeTrailingSlash: false});

normalizeUrl('www.sindresorhus.com/foo/default.php', {
  removeDirectroyIndex: [/^default\.[a-z]+$/]
});

normalizeUrl('www.sindresorhus.com?b=two&a-one&c=three', {
  sortQueryParameters: false
});
```

```sh
npm install normalize-url
```

```
```


