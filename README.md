# Coperacha for iOS and Android   
![Imgur Image](https://i.imgur.com/MaJM1KE.png)  

Coperacha is a React Native app which make fundraising easy, borderless, and fee-free for you and your community. It is built on the Celo blockchain. 

## Name

"Hacer coperacha" is a phrase used in Central Mexico for putting money together towards a shared goal. The Coperacha app makes this easy.

Usage: *"Vamos a hacer coperacha para la gasolina"* means "Let's put some money together to pay for gas". 

## Demo 

[![Video](https://i.imgur.com/Ek9OOLX.png)](https://www.youtube.com/watch?v=xLD6wRkHRAU)


## App download

If you're on Android, you can scan the QR code on the [Expo Go](https://play.google.com/store/apps/details?id=host.exp.exponent&hl=en_US&gl=US) app to run Coperacha instantly:

<img src="https://i.imgur.com/mKo5Bm0.png" width="300" height="250" />


Alternatively, you can download the .ipa (ios) or .apk (android) files to directly load it on your device from the [releases page](https://github.com/Alex-Neo-Projects/Coperacha-app/releases). 

The third option is to run the code from the repo on your computer. Instructions can be found below under "running Coperacha locally". We weren't able to get a testflight approved in time for the hackathon. 

**Note: This app uses testnet cUSD exclusively, and requires a [Celo test wallet](https://celo.org/developers/wallet) in order to work** 

## Background info 
Celo is a mobile-first blockchain. It is a fork of Ethereum and is built to be a global payments infrastructure targeting the developing world. Celo has two native cryptocurrencies, cUSD (a currency that's pegged to the Dollar, 1 cUSD = 1 USD) and Celo gold (a volatile currency used for Celo governance and utility). Coperacha uses cUSD exclusively to transact. 

# About us

Alex is a student at Penn State University and Neo is a student at the University of Central Florida. We met on Discord in a React study group a little over a month ago, and we decided to team up to build things together. Coperacha is our second collaborative project so far, and the first one we're launching. We made this app for the ["Make it Mobile Hackathon with Celo" hackathon](https://gitcoin.co/issue/celo-org/gitcoin/8/100024939). 

## Why we made Coperacha 

We built this app because we think that the ability to crowdfund towards causes you and your community care about is an important feature to have on the Celo network. Since gas prices are extremely low, it's feasible to do this while giving 100% of proceeds (no fees!) to the people who need it. 

We envision Coperacha as being used in communities that already use Celo, for causes big and small. As the Celo network grows, our hope is that Coperacha will have the opportunity to grow with it. 

Some ideas for fundraisers on Coperacha include: 
 - Raising money to fix a road in the community 
 - Raising money to put on an event for the community
 - Raising money to pay for an individual's medical bills
 - Small things like raising money for a road trip among a handful of friends

## Coperacha's potential for impact

We are building Coperacha to be global from day one. Since we can't support all the regions we'd like to right away, we're focusing on making it work for English & Spanish speakers. More specifically, we're focused on North America and Latin America to start out, as we know there are many Celo users in Latin America. We wanted to have the app translated to Spanish for the hackathon (Alex is a native speaker), but due to time constraints we weren't able to do it before the hackathon deadline. 

Our target audience is Celo users and communities who rely on the Celo network for banking and need a way to fundraise in their community. 

## Our experience building Coperacha

The first thing we built out was the [smart contracts](https://github.com/Alex-Neo-Projects/Coperacha-contracts) for Coperacha. The initial prototype was very short (160 lines of code) and brought us to a realization: 

![infrastructure](https://i.imgur.com/3PqEjaF.png)

Using Celo meant we could accept payments without all the infrastructure overhead of doing it with the traditional financial system. Replicating the functionality of the smart contract using the traditional financial system would likely take Plaid (banking), Stripe (payments), AWS (server hosting), and MongoDB (storing user data). The smart contract we wrote in 160 lines of code and a few hours covered all of that with a comparably tiny amount of hassle. 

After we had the smart contract ready, we were able to focus on the Coperacha app (this repo!) for the remainder of time we worked on this hackathon project. This was our first time building a React Native app, so there was a learning curve but overall it went a lot quicker than if we would have built native apps. 

Overall, the biggest piece of feedback I have for the Celo organization is that writing more extensive documentation would make the development process much, much easier for developers building on Celo. There were a couple of times where I ran into incomplete/outdated documentation or documentation that felt unfinished on the Celo developer website. Extensive documentation and more examples would really help out Celo developers everywhere. 

## Features

Coperacha currently supports the following features: 

- Users can create, donate, and manage their own fundraisers 
- Users can view all listed fundraisers
- Integration with the Celo Alfajores Wallet to handle payments

# Running Coperacha locally

```
git clone https://github.com/Alex-Neo-Projects/Coperacha-app

cd Coperacha-app

npm install --save --legacy-peer-deps

expo start
```

``npm install --save --legacy-peer-deps`` is used because running ``npm install`` by itself returns a dependency tree error. 

# Links

We're building this for the ["Make it Mobile Hackathon with Celo" hackathon](https://gitcoin.co/issue/celo-org/gitcoin/8/100024939). 

Website: [coperacha.app](https://www.coperacha.app)

Smart contracts: [here](https://github.com/Alex-Neo-Projects/Coperacha-contracts)

Mockups + design board: [here](https://whimsical.com/coperacha-ExoT2t7gobgXMG3Vpv5RxD)

Icon design board: [here](https://www.figma.com/file/tbGJBHQ2sXIGS71g7Rv4If/Coperacha-Icons?node-id=18%3A152)

# License

This project uses the MIT license. [Full license available here.](https://github.com/Alex-Neo-Projects/Coperacha-app/blob/master/LICENSE)
