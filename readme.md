> :warning: *IMPORTANT* this repository is out of date.
> From Couchbase Server 7.0, please see https://github.com/couchbaselabs/try-cb-frontend-v2

<hr />

Angular 2 Front End for CB Reference Application
===============

Travel-Sample Application for CB 4.5 including support for new features :
- CBFT
- Subdoc
- Array Indexing  

This application uses Angular 2.0 and typescript.  The developer environment requires Angular-CLI to build.

## Versioning

**This is version `2.0.1`**

The aim is to build a distributable package that can be embedded in the various `try-cb` backend implementations.

Each time a new stabilized version is made, the version minor or major number should be increased and the build should be copied over to all try-cb backends.

The distribution's version number should be reflected in a tag and be also visible in the app's footer (see `app/app.component.html`).

## Steps to Build
 - [1] Install NPM 6.0.0 or later

 - [2] Clone this repo.

 - [3] Make sure you have `angular-cli` installed (**this was built using angular-cli `1.0.0-beta.14`**):

```
npm install -g angular-cli@1.0.0-beta.14
```

 - [3] Install node dependencies, build and serve using angular-cli:

```
npm install
ng serve
```

To build a distributable version that can be embedded in a try-cb backend implementation, you can also use production mode:

```
rm -rf dist/*
ng build --prod
```

Then copy the content of `dist/` over to the backend application.

**If you have globally installed an different angular-cli**:

```
npm uninstall -g angular-cli
npm install -g angular-cli@1.0.0-beta.14
```

Note the `latest` version of anglular-cli doesn't work with the version that was used to build this example (1.0.0-beta14).
