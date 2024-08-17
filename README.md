# osscom
Open source software components

## Steps

```
==> npm create vue@latest

Vue.js - The Progressive JavaScript Framework

✔ Project name: … osscom-frontend
✔ Add TypeScript? … No / Yes YES
✔ Add JSX Support? … No / Yes YES
✔ Add Vue Router for Single Page Application development? … No / Yes YES
✔ Add Pinia for state management? … No / Yes YES
✔ Add Vitest for Unit Testing? … No / Yes
✔ Add an End-to-End Testing Solution? › Playwright
✔ Add ESLint for code quality? … No / Yes YES
✔ Add Prettier for code formatting? … No / Yes YES
✔ Add Vue DevTools 7 extension for debugging? (experimental) … No / Yes YES

Scaffolding project in /Users/coder/repos/arunabhdas/githubrepos/osscom/osscom-vue/osscom-frontend...

Done. Now run:

  cd osscom-frontend
  npm install
  npm run format
  npm run dev
```

## Add NuxtUI

- Add NuxtUI to the project from the steps outlined in https://ui.nuxt.com/getting-started/installation

```
cd osscom-vue

cd osscom-frontend

npx nuxi@latest module add ui

```

## Initialize NuxtJS 

- Initialize NuxtJS project 
```
==> npx nuxi@latest init osscom

✔ Which package manager would you like to use?
npm
◐ Installing dependencies...                                                                  11:32:31 PM
npm warn deprecated inflight@1.0.6: This module is not supported, and leaks memory. Do not use it. Check out lru-cache if you want a good and tested way to coalesce async requests by a key value, which is much more comprehensive and powerful.
npm warn deprecated npmlog@5.0.1: This package is no longer supported.
npm warn deprecated rimraf@3.0.2: Rimraf versions prior to v4 are no longer supported
npm warn deprecated are-we-there-yet@2.0.0: This package is no longer supported.
npm warn deprecated glob@8.1.0: Glob versions prior to v9 are no longer supported
npm warn deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
npm warn deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
npm warn deprecated gauge@3.0.2: This package is no longer supported.

> postinstall
> nuxt prepare

✔ Types generated in .nuxt                                                                   11:32:52 PM

added 642 packages, and audited 644 packages in 21s

128 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
✔ Installation completed.                                                                    11:32:52 PM

✔ Initialize git repository?
No
                                                                                              11:32:57 PM
✨ Nuxt project has been created with the v3 template. Next steps:
 › cd osscom                                                                                  11:32:57 PM
 › Start development server with npm run dev 
 ```


## Install Nuxt ESLint

- https://eslint.nuxt.com/packages/module

Install Nuxt ESLint

```
npx nuxi module add eslint
```

## Screenshots

![Screenshot 0](https://raw.githubusercontent.com/arunabhdas/osscom/main/screenshots/osscom_0.png)
![Screenshot 1](https://raw.githubusercontent.com/arunabhdas/osscom/main/screenshots/osscom_0.png)

## Steps

==> npm create svelte@latest
```
==> npm create svelte@latest
Need to install the following packages:
create-svelte@6.3.5
Ok to proceed? (y) y

create-svelte version 6.3.5

┌  Welcome to SvelteKit!
│
◇  Where should we create your project?
│  osscom-frontend
│
◇  Which Svelte app template?
│  Skeleton project
│
◇  Add type checking with TypeScript?
│  Yes, using TypeScript syntax
│
◇  Select additional options (use arrow keys/space bar)
│  Add ESLint for code linting, Add Prettier for code formatting, Add Playwright for browser testing, Try the Svelte 5
preview (unstable!)
│
└  Your project is ready!

Install more integrations with:
  npx svelte-add

Next steps:
  1: cd osscom-frontend
  2: npm install
  3: git init && git add -A && git commit -m "Initial commit" (optional)
  4: npm run dev -- --open

To close the dev server, hit Ctrl-C

Stuck? Visit us at https://svelte.dev/chat
```

## AlpineJS Directives
```

* x-data
* x-on
* x-text
* x-model
* x-bind
* x-init
* x-ref
* x-show




## Resources

AlpineJS - https://youtu.be/4c8dpZN0rqM?si=iFkOLfGj9xfVPKLF

FrankenUI - https://github.com/franken-ui/ui 