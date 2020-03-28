# Host react app using gh-pages

![](/img.gif)

Learn how to host react apps on github pages.

1. Add `homepage` to `package.json`

```JS
"homepage": "https://github.com/Rainymood/host-react-app-gh-pages"
```

2. Install `gh-pages`

```bash
npm install --save gh-pages
```

3. Add (pre)-deploy scripts to `package.json`

```JS
"scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build",
```
4. Deploy

```bash
npm run deploy
```

## Acknowledgements

* [This tutorial on dev.to](https://dev.to/yuribenjamin/how-to-deploy-react-app-in-github-pages-2a1f)
* [The official facebook tutorial](https://create-react-app.dev/docs/deployment/#step-1-add-homepage-to-packagejson)