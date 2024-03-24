## To deploy gatsby app to github pages

1. Install `gh-pages`
```bash
npm install gh-pages --save-dev
```

2. In package.json file add script:
```json
"deploy": "gatsby build --prefix-paths && gh-pages -d public"
```

3. Open `gatsby-config.ts` and add to exports:
```js
pathPrefix: "/repo name",
```