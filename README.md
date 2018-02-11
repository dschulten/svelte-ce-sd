# Sveltejs custom-element with shadow-dom in IE11

This is a project template for a [Svelte](https://svelte.technology) webcomponent with shadow dom which supports IE11.

To create a new project based on this template using [degit](https://github.com/Rich-Harris/degit):

```bash
npm install -g degit # you only need to do this once

degit sveltejs/dschulten/svelte-ce-sd
cd svelte-app
```

*Note that you will need to have [Node.js](https://nodejs.org) installed.*


## Get started

Install the dependencies...

```bash
cd svelte-ce-sd
npm install
```

...then start [Rollup](https://rollupjs.org):

```bash
npm run dev
```

Navigate to [localhost:5000](http://localhost:5000). You should see your app running. Edit a component file in `src`, save it, and reload the page to see your changes.


## IE11

Please note that this project includes the [tuespetre/shadow-dom](https://github.com/tuespetre/shadow-dom) polyfill as a static resource in index.html and transpiles classes to ES5 with *Babel*. That combination turned out to be a combination that runs with IE11 and uses a real shadow dom in Chrome.

Buble seems to have an [issue](https://github.com/sveltejs/svelte/issues/1171) caused by the way it transpiles class constructors, at least in the default setup.


## Deploying to the web

### With [now](https://zeit.co/now)

Install `now` if you haven't already:

```bash
npm install -g now
```

Then, from within your project folder:

```bash
now
```

As an alternative, use the [Now desktop client](https://zeit.co/download) and simply drag the unzipped project folder to the taskbar icon.

### With [surge](https://surge.sh/)

Install `surge` if you haven't already:

```bash
npm install -g surge
```

Then, from within your project folder:

```bash
npm run build
surge public
```
