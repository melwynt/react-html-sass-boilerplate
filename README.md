# A simple React and SASS Boilerplate with Parcel bundler.

## Table of contents

- [A simple React and SASS Boilerplate with Parcel bundler.](#a-simple-react-and-sass-boilerplate-with-parcel-bundler)
  - [Table of contents](#table-of-contents)
  - [Description](#description)
  - [Why should you use this boilerplate?](#why-should-you-use-this-boilerplate)
  - [Things I've added to get you up and running](#things-ive-added-to-get-you-up-and-running)
  - [HMR (Hot Module Replacement)](#hmr-hot-module-replacement)
  - [Troubleshooting](#troubleshooting)
  - [Fork](#fork)
  - [Contact](#contact)

## Description

- [parceljs](https://parceljs.org/)
- react
- react-dom
- sass

Node version in use (`node -v`):<br>
`v16.13.0`

Run `npm ci` locally to install all required modules.

Run `npm start` to start the live server locally.

Please give this repo a ⭐ if you found it useful! Thanks

## Why should you use this boilerplate?

Parcel is fast!<br>

And this boilerplate makes it super easy to get you up and running.

## Things I've added to get you up and running

In the `index.html` file, I've added the bare minimum.<br>

In `index.js` and `app.js`, you can replace the code with your React app.<br>

The code below will only apply in development.<br>

> Hot Module Replacement (HMR) improves the development experience by automatically updating modules in the browser at runtime without needing a whole page refresh. This means that application state can be retained as you change small things.

```javascript
if (module.hot) {
  module.hot.accept();
}
```

## HMR (Hot Module Replacement)

You might have noticed in `package.json` this line:

```
"start": "rm -rf public/* && parcel src/index.html --dist-dir public --port 1234 --hmr-port 4326 --host localhost --open"
```

Normally it would have been enough to just enter:

```
"start": "parcel src/index.html"
```

HMR might fail on some machines hence the need to specify `--port`, `--hmr-port` and `--host`.

Source: [https://github.com/parcel-bundler/parcel/issues/6334#issuecomment-868853192](https://github.com/parcel-bundler/parcel/issues/6334#issuecomment-868853192)

```
rm -rf public/*
```

Each time we are running `npm start`, we delete all the files inside the `public` folder to avoid stale files.

## Troubleshooting

![](./404.png)

If you get a `404` error, try to delete the cache first by running this command:

```
rm -rf .parcel-cache
```

## Fork

You should fork this repo if you would like to use it.

If you decide to clone this repo, don't forget to change your Git remote URL:<br>
Here's a quick [How-To](https://devconnected.com/how-to-change-git-remote-origin/) guide.

```
git remote set-url origin <your-remote_url>
git remote -v
```

## Contact

🐦 Twitter: [@melwyncode](https://twitter.com/melwyncode)<br>
🧑‍💻 LinkedIn: [melwynturbant](https://www.linkedin.com/in/melwynturbant)
