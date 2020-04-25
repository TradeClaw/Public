# TradeClaw.net
Releasing in 2020
* Trading signals (free & paid subscriptions, Summer 2020)
* Automated trading bot (Fall 2020)

For more up to date information, join our Discord
https://discord.gg/MJfsnD9

### CHANGELOG : 2020-04-25 ###

### Known issues
- None

### Feature request list
- None

### Phase 1 Priorities
- REST API for database
- Centralized exchange configs
- Bitmex production addition
- Add Binance
- Fetch and store candle data
- Integration with Taapi.io
- Indicator calculation
- Add Trade8
- Add Bitmart
- Add Huobi Global
- Add Bitfinex
- Add Kraken
- Add LaToken
- Add UpBit
- Add Binance US
- Add ByBit
- Add Deribit
- Add KuCoin
- Add Poloniex
### Phase 2 Priorities
- Strategy composition
- Leverage trading
- Order placement
- Order follow-up
- Order follow-up (advanced)
- Leverage trading (advanced)
- User interface
- User exchange delegation
### Phase 3 Priorities
- User graphing interface
- User exchange delegation (Advanced)

## [0.0.4] SLOTH - 2020-04-25
### Summary
Update on development progress:
Still adding more exchanges, 8 onboarded in the framework. (Bitmex, Binance, Bitfinex, Bitmart, ByBit, Huobi Global, KuCoin, Trade8)
CoinAPI added, that might come in handy one day for additional features like planned for Taapi.io
Decided that this might be a better approach because we already have the code for the next phase and it will only require slight adjustment from v2.
Expanding to more exchanges at the start, gives insight in their differences to not run into issues with the framework in the future, first time right!
Most time in May will be spent in rigorous testing and writing a decent simulation module.
Next up are GDAX, HitBTC, Bittrex, Cex.io, FTX, Poloniex, Deribit, Kraken ... more requests?
We're going to use acronyms for framework functionality to make it more clear what/where is changing.

### Added
- Testing the result of REST calls
- Generalized the getting candles from REST
- Framework logic to get kline/candle data on websockets that do not provide it (No known public solution for in existence!)

### Changed 
- A lot of framework code for centralized error handling
- Retry mechanisms where needed, for instance when the kline data on REST was behind of the websocket for a few seconds

### Planned
- Add 6 exchanges to the Dynamic Exchange Framework (DEF)
- Historical database design for kline/indicators
- Fill up history
- Calculate indicators historically
- Dynamic Strategy Engine (DSE)
- Centralized Simulation Evaluator (CSE)

## [0.0.3] SLOTH - 2020-04-17
### Summary
Update on development progress:
Focussing on adding more exchanges to test out the core layer stability!

### Added
- REST interface for the database
- GZIP stream decoding
- Users & accounts modules
- Binance addition
- Bitmex addition
- Huobi Global addition
- Huobi Global Test addition
- Bitmart addition (inactive for now, that API is a disaster)
- Trade8 addition (crypto/forex/stocks/bonds)
- KuCoin addition
- KuCoin Test addition

### Changed 
- Improve websocket error handling
- Improve websocket dynamic endpoints


## [0.0.2] SLOTH - 2020-04-12
### Summary
First release, basically everything added.
Starting from scratch but re-using all the working v2 code where applicable, keeping the good stuff!

### Added
- Websocket
- Discord integration
- Centralized database
- Fail-over with heartbeat
- Dynamic scalability
- Database creation (meta+data)
- Bitmex Test addition

### Changed (template for future changelogs)
- Rewrite something.
- Improve something.
- Merge something.
- Fix something.

### Removed (template for future changelogs)
- Something could be removed.
