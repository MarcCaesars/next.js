# Electron application example

**You can find a detailed documentation about how to build Electron apps with Next.js [here](https://leo.im/2017/electron-next)!**

## How to use

### Using `create-next-app`

Download [`create-next-app`](https://github.com/segmentio/create-next-app) to bootstrap the example:

```bash
npx create-next-app --example with-electron with-electron-app
# or
yarn create next-app --example with-electron with-electron-app
```

### Download manually

Download the example [or clone the repo](https://github.com/zeit/next.js):

```bash
curl https://codeload.github.com/zeit/next.js/tar.gz/canary | tar -xz --strip=2 next.js-canary/examples/with-electron
cd with-electron
```

Install it and run:

```bash
npm install
npm start
```

## The idea behind the example

This example show how you can use Next.js inside an Electron application to avoid a lot of configuration, use Next.js router as view and use server-render to speed up the initial render of the application.

For development it's going to run a HTTP server and let Next.js handle routing. In production it use `next export` to pre-generate HTML static files and use them in your app instead of running an HTTP server.

You can create the production app using `npm run dist`.
