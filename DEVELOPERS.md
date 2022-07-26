# Developers

Whirlpool can be integrated in several ways:

## I. Using the library `whirlpool-client`
This is the best way to integrate Whirlpool into your Java or Android application.  
The library can be found within the [`whirlpool-client`](https://code.samourai.io/whirlpool/whirlpool-client) repository.  
Read [whirlpool-client/doc/DEVELOPERS.md](https://code.samourai.io/whirlpool/whirlpool-client/-/blob/develop/doc/DEVELOPERS.md) for getting started.

Examples:
- See [Sparrow integration](https://github.com/sparrowwallet/sparrow/tree/master/src/main/java/com/sparrowwallet/sparrow/whirlpool)
- See [samourai-wallet-android](https://code.samourai.io/wallet/samourai-wallet-android/-/tree/develop/app/src/main/java/com/samourai/whirlpool/client/wallet)

## II. Remote-controlling `whirlpool-client-cli`
The [`whirlpool-cli`](https://code.samourai.io/whirlpool/whirlpool-client-cli) is a standalone Whirlpool client which can be run on Linux, Mac or Windows environments.  
A [REST API](https://code.samourai.io/whirlpool/whirlpool-client-cli/-/blob/develop/doc/API.md) is made available to quickly bootstrap your own applications on top of Whirlpool.  
Examples:
- See [whirlpool-gui](https://code.samourai.io/whirlpool/whirlpool-gui/-/tree/develop/app/mainProcess) integration

## III. Using your own implementation of the protocol
Review the [architecture](ARCHITECTURE.md) and implement it in your own way.
