- Decrease latency-> increase the number of transactions -> increase profitability over time
- Automation, throughput, performance, latency
- High frequency trading (HFT) involves computer architecture, operating systems, networking, and programming.
- Crypto exchanges since 2015, e.g. Coinbase, Binance.
- HFT vs regular trading; HFT focuses on speed and automation.

What an HFT needs:
- Fast computers: single-core throughput to avoid context switching etc. No parallelism.
- Exchange proximity: participants co-locate their servers to decrease latency and shorten time to complete a deal.
- Low latency: latency=(time for data to reach trader's computer + time for trader to make an order + time for order to be accepted) Microseconds or even nanoseconds.
- Computer algorithms: the heart of AT/HFT, real-time data feeds

**Strategies**
- Scalping: benefits from small price changes. Let your gains run.
- Statistical arbitrage: profit from mispricing of assets. This can be price discrepancies in the same security sold on separate venues or in related securities.
- Latency arbitrage: takes advantage of market players' different speeds through high-speed fiber optics, superior bandwidth, co-located servers, and direct-price feeds.
- Information-driven strategies: e.g. sentiment analysis
- Momentum ignition: attempt to make market players believe that a large price movement will occur. E.g. sending enormous volumes of orders and then cancelling them.
- Pinging: strategy for learning about huge orders in exchanges and dark pools by placing tiny marketable orders
- Front-running: placing an order based on on information not publicly released. Illegal in traditional markets.
- Spoofing: placing an order not intended to be executed so that market reacts. Illegal in traditional markets.
- Layering: similar to spoofing but orders placed at different prices.

## Trading Systems
### What to consider
- Asset class: Each has its own characteristics. Number of symbols and number of exchanges will shape the architecture.
- Strategy type (high frequency, long-term position: For HFT (microseconds/nanoseconds) C++ or Java are better suited. For long-term positions (days) Python is appropriate.
- Number of users/traders/trading techniques: More traders->MORE ORDERS.

### Architecture
#### Venues
- Any platform matching buy/sell orders.
- Trading systems communicate with venues to collect price updates.

#### Gateways
- Ensure communication between trading system and venues.
- The most demanding in terms of execution time, systems resources, and OS.
- They need to be able to process a variety of protocols.

#### Book builder
- Builds the limit order book from data collected by Gateways.

#### Strategy
- Sends the order to the venues through the Order Manager.
- Once coded becomes part of the trading system. Input: price data, output: orders. This gives trading signals.
- The trade takes place on a different computer than the one running the strategy.
