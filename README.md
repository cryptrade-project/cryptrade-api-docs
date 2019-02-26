# API Docs For Cryptrade DEX

API documents for Cryptrade decentralized exchange.

## Endpoint
The base endpoint is: [https://api.cryptrade.io](https://api.cryptrade.io)

## Request Limits
* The maximum access rate is 200 requests per minute, any clients initiates more requests will be throttled with status code 429.

## Public API

### [All Tickers]

**Description**

Return all available tickers

**URL**
```
GET /api/v1/tickers
```

**Example Response**
```json
[
    {
        "id": "BTC_BTS",
        "quote": "BTC",
        "base": "BTS",
        "latest": "0.00000000",
        "lowestAsk": "0.00000000",
        "highestBid": "0.00000000",
        "percentChange": "0.00",
        "baseVolume": "0.00000000",
        "quoteVolume": "0.00000000"
    },
    {
        "id": "CRCO_BTS",
        "quote": "CRCO",
        "base": "BTS",
        "latest": "0.00000000",
        "lowestAsk": "0.00000000",
        "highestBid": "0.00000000",
        "percentChange": "0.00",
        "baseVolume": "0.00000000",
        "quoteVolume": "0.00000000"
    },
    {
        "id": "CRCO_BTC",
        "quote": "CRCO",
        "base": "BTC",
        "latest": "0.00000000",
        "lowestAsk": "0.00000000",
        "highestBid": "0.00000000",
        "percentChange": "0.00",
        "baseVolume": "0.00000000",
        "quoteVolume": "0.00000000"
    }
]
```

### [Specific Ticker]

**Description**

Return a specific ticker

**URL**
```
GET /api/v1/ticker/:market_id
```

**Example Request**
```
GET /api/v1/ticker/CRCO_BTC
```

**Example Response**
```json
{
    "id": "CRCO_BTC",
    "quote": "CRCO",
    "base": "BTC",
    "latest": "0.00000000",
    "lowestAsk": "0.00000000",
    "highestBid": "0.00000000",
    "percentChange": "0.00",
    "baseVolume": "0.00000000",
    "quoteVolume": "0.00000000"
}
```

## Questions && Issues

Please use the [issues](https://github.com/cryptrade-project/cryptrade-api-docs/issues) on this github project to ask questions and report bugs.

## Contact

Any other problems or feedbacks, please contact Cryptrade Dev Team via Email: [support@cryptrade.io](mailto:support@cryptrade.io)
