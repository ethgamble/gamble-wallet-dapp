# Gamble Wallet Ðapp

The Ethereum Gamble wallet Ðapp.

**NOTE** The wallet is not yet official released,
can contain severe bugs!


## Development

Start an `geth` node and and the app using meteor and open http://localhost:3000 in your browser:

    $ geth --rpccorsdomain "http://localhost:3000" --rpc --unlock <your account>

Starting the wallet dapp using [Meteor](https://meteor.com/install)

    $ cd gamble-wallet-dapp/app
    $ meteor

Go to http://localhost:3000


## Deployment

To create a build version of your app run:

    // install meteor-build-client
    $ npm install -g meteor-build-client

    // bundle dapp
    $ cd gamble-wallet-dapp/app
    $ meteor-build-client ../build --path ""

This will generate the files in the `../build` folder. Double click the index.html to start the app.
To make routing work properly you need to build it using:

    $ meteor-build-client ../build

And start a local server which points with its document root into the `../build` folder,
so that you can open the app using `http://localhost:80/`

## Test

Using Metamask and test the wallet on Ropsten Network at http://ethgamble.github.io
