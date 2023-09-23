# solo: journal

[DEMO SOLO HERE](https://solo-journal.vercel.app/)

this app is under construction. feedback highly encouraged. 

## use on devnet

no signature requests will be made, and no wallet functionality beyond wallet-gating has been implemented

### to-do

- figure out github secrets to add firebase config and go public 
- fix wallet and browser compatibility issues / "it was working on localhost!"
- add view transaction history + trade journaling prompts
- integrate shadow storage solution to decentralize and obfuscate entries 
- add nft/collectibles notes/reclection entry for notes on the drop/art/community or otherwise 

**this dapp is a rewrap of the solana [pay scaffold](https://github.com/solana-labs/solana-pay-scaffold)**

## Getting Started

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Preparation

in order to run this locally, you'll need to replace the following line in `Am.tsx`, `Freewrite.tsx`, `Pm.tsx`, and `ViewEntries.tsx` with your own firebase config:

replace-
```
const firebaseConfig = require('./firebase-config.json'); // Read Firebase config from the file
```
with-
```
const firebaseConfig = {
        apiKey: "YOUR_API_KEY",
        authDomain: "YOUR_AUTH_DOMAIN",
        projectId: "YOUR_PROJECT_ID",
        storageBucket: "YOUR_STORAGE_BUCKET",
        messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
        appId: "YOUR_APP_ID",
        measurementId: "YOUR_MEASUREMENT_ID"
    };
```


## Installation

```bash
npm install
# or
yarn install
```

## Build and Run

Next, run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the transaction request page by modifying `src/pages/index.tsx`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/transaction](http://localhost:3000/api/transaction). This endpoint can be edited in `src/pages/api/transaction.ts`.

