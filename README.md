# Design Your Way

This template uses [Svelte](https://svelte.dev/) + [Sapper](https://sapper.svelte.dev/) + [Tailwind CSS](https://tailwindcss.com/) + [Firebase Functions](https://firebase.google.com/products/functions) + [Firebase Hosting](https://firebase.google.com/products/hosting).

[Demo](https://designyourway.web.app)


## Getting started


```bash
npx degit "anujkarn002/designyourway" design-your-way && cd $_
```

### Running the project


```bash
cd functions
npm install
```

Run `npm run dev:tailwindcss` and `npm run dev` in two separate terminal.

Open up [localhost:3000](http://localhost:3000) and start clicking around.


### Deploying the project

Setup Firebase if haven't already!!

```bash
npm install -g firebase-tools
firebase login
```

Edit [.firebaserc](blob/master/.firebaserc) with your firebase project id. Also make sure you have that project created at [Firebase Console](https://console.firebase.google.com)

```json
{
  "projects": {
    "default": "YOUR-FIREBASE-PROJECT-ID"
  }
}
```

Then run

```bash
npm run deploy
```

Open up [YOUR-PROJECT-ID.web.app](http://YOUR-PROJECT-ID.web.app) and start clicking around.
