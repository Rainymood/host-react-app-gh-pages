# Host react app using gh-pages

1. Add `"homepage": "https://github.com/Rainymood/host-react-app-gh-pages"` to `package.json`
2. Install `gh-pages` with `npm install --save gh-pages`
3. Add this to scripts:
```JS
"scripts": {
+   "predeploy": "npm run build",
+   "deploy": "gh-pages -d build",
    "start": "react-scripts start",
    "build": "react-scripts build",
```
4. `npm run deploy`

https://create-react-app.dev/docs/deployment/#github-pages