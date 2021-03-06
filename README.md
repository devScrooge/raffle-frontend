# RAFFLE FRONT END ✅

This is a full stack decentralized Raffle App using Chainlink VRF and Chainlink Keepers, Solidity and Next.js from workshop from Chainlink Hackathon Spring 2022 and which is also complemented by Patrick Alpha's Free Code Camp course.

This repo contains all the stuff for the front-end part, the back-end is hold on [raffle-frontend](https://github.com/JMariadlcs/raffle-full-stack).

To achieve fully descentralization the Front-End has been uploaded to IPFS and fleek: ipfs://QmexxqxhViwpFsbWnbMktNhG3qsukTA58rLyLQaCpg8vy3, https://curly-butterfly-3592.on.fleek.co/

The workshop followed to complete this repo is [this one](https://www.youtube.com/watch?v=8bMrko6iD9Q&t=5445s).

The used repos from Patricks are the followings:

1. [Hardhat Smart Contract Lottery](https://github.com/PatrickAlphaC/hardhat-smartcontract-lottery-fcc): Patrick's repo that we are building.
2. [Front-end Smart Contract Lottery](https://github.com/PatrickAlphaC/nextjs-smartcontract-lottery-fcc): Patrick's repo for the Front-end part.
3. [Patricks Hardhat course video](https://www.youtube.com/watch?v=gyMwXuJrbJQ&t=15996s).

## DEPENDENCIES AND SET-UP

-   Create Next.js project:

```bash
yarn create next-app .
```

-   Add Moralis to interact with front-end:

```bash
yarn add moralis react-moralis
```

-   Add Moralis web3uikit to interact with front-end:

```bash
yarn add web3uikit

```

-   Add tailwindcss (CSS formarter):

```bash
yarn add --dev tailwindcss postcss autoprefixer
```

or

```bash
npm install tailwindcss postcss autoprefixer
```

-   Initialize tailwindcss:

```bash
yarn tailwindcss init -p
```

or

```bash
npx tailwindcss init -p
```

-   Override [tailwind.config.js](https://github.com/JMariadlcs/raffle-frontend/blob/main/tailwind.config.js) with the code inside this file.
-   Override [global.css](https://github.com/JMariadlcs/raffle-frontend/blob/main/styles/globals.css)

## RUN LOCAL SERVER:

```bash
yarn dev
```

You will have your local server running at: `http://localhost:3000`.

-   Open new bash terminal to use while yarn server is running

## EXPORT CODE

Once our Front-End code is finished..

1. Export our code to a Bundle.
2. Upload the Bundle to IPFs to be fully decentralized.

-   Execute:

```bash
yarn next build
yarn next export
```

A file called `out` is going to be generated with our exported code.

## UPLOAD TO IPFS

We want our Front-End to be fully decentralized. To achive this goal we are uploading the `out` file to IPFS.

1. Open IPFS.
2. Go to Files.
3. Import `out` directory.
4. Click 'set pinning'.

DONE! ✅

5. Copy CID.
6. Go to Browher and paste ipfs://CID.

NOTICE: It is possible to use [fleekhq](https://fleekhq.eth.link) or [pinata](https://www.pinata.cloud) to host our ipfs in a normal domain in order to make it easier for people to reach our page.

**REMINDER**: if you use [fleekhq](https://fleekhq.eth.link) (recomended) -> add: buildcommand: 'yarn install && yarn run build && yarn run export'

## RESOURCES

-   [Full-stack-web3-connectors](https://github.com/PatrickAlphaC/full-stack-web3-metamask-connectors): a repo that contains different ways of using web3 connectors.
-   [Nextjs repo](https://github.com/PatrickAlphaC/nextjs-moralis-metamask-connect/tree/cd4ff2ce34ecec6874e8fa32df8f44cef962b6e7): repo that we are going to work with.
-   [Hardhat simple storage](https://github.com/PatrickAlphaC/hardhat-simple-storage): Patricks repo clonned to run our own local Blockchain network and interact with its Smart Contracts.
-   [web3uikit](https://github.com/web3ui/web3uikit): Can be used for the front end to interact when user changes account or connect/disconnect.
-   [tailwindcss with Nextjs](https://tailwindcss.com/docs/guides/nextjs): CSS formater.# raffle-frontend
