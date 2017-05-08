# Set up

- `npm install -g hexo-cli firebase-tools`
- `npm install`

Use hexo cli to make posts. `hexo new [layout] <title>`

Deploy by

1. `hexo clean`
2. `hexo generate`
3. `firebase deploy`

Optional

1. `brew update`
2. `brew install libtool automake autoconf nasm libpng`

Spellcheck

`npm run spellcheck`

Content Security Policy

if needed

```
<meta http-equiv="Content-Security-Policy" content="
    default-src *;
    style-src 'self' 'unsafe-inline' https:;
    script-src 'self' 'unsafe-inline' 'unsafe-eval' https: code.jquery.com maxcdn.bootstrapcdn.com cdnjs.cloudflare.com *.disqus.com *.disquscdn.com data:">
```

## Todo
- [ ] Add "Wedding Party" page
- [x] Add "Our Story" page
- [x] Remodel site
  - [x] See `themes/mock up` folder