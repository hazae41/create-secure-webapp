# Create Secure Webapp

Make a secure webapp with React and Tailwind

## Features

- Built on web standards and fundamentals
- Works with any client-side and/or static-side library (e.g. React, jQuery)
- Focused on security and simplicity without degrading performances
- Supply-chain hardened with the bare minimum dependencies
- Built for Deno but backward compatible with Node/Bun
- Deploy it anywhere HTML/CSS/JS files can be stored
- Builds are cross-platform cross-runtime reproducible
- Immutably cached with a 1-year cached service worker

## Stack

- `deno` for the runtime
- `react` and `react-dom` for rendering
- `tailwindcss` via [`@hazae41/rewind`](https://github.com/hazae41/rewind) and [`@hazae41/labase`](https://github.com/hazae41/labase) for the styles
- `esbuild` via [`@hazae41/glace`](https://github.com/hazae41/glace) for bundling
- [`@hazae41/immutable`](https://github.com/hazae41/immutable) for immutable caching

## Setup

### Development

Clone this repository

```bash
git clone https://github.com/hazae41/create-secure-webapp.git starter && cd ./starter
```

Reset the Git history

```bash
rm -rf ./.git && git init
```

Install dependencies

```bash
npm install
```

Start developing

```bash
npm run develop
```

### Vercel

Just setup the build command

```bash
npm run examine && npm run prepack
```

The output directory

```path
./out
```

The install command

```bash
npm install
```

#### Warning

Vercel may add, modify, or remove some parts of your website with some feature slop

This can make your website less secure or brick its integrity mechanisms, making your users see weird errors or unable to use your website at all

So you have to disable the following options and any option you can suspect of modifying your website

Both in your Vercel project (`https://vercel.com/<account>/starter/settings/general`) and in your Vercel account (`https://vercel.com/<account>/~/settings/general`) if wanted

- General > Vercel Toolbar: disable everything

## Usage

- Develop

```bash
npm run develop
```


- Test

```bash
npm run examine
```


- Build

```bash
npm run prepack
```

- Serve

```bash
npm run produce
```