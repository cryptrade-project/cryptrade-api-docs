# API Docs For Cryptrade DEX

API documents for Cryptrade decentralized exchange.

## Endpoint
The base endpoint is: [https://api.cryptrade.io](https://api.cryptrade.io)

## Request Limits
* The maximum access rate is 200 requests per minute, any clients initiates more requests will be throttled with status code 429.

## Public API

### All tickers

**Description**

Return all available tickers

**URL**
```
GET /api/v1/tickers
```

**Response**
```json
[
    {
        "id": "BTC_BTS",
        "quote": "BTC",
        "base": "BTS",
        "latest": "0.00000000",
        "lowest_ask": "0.00000000",
        "highest_bid": "0.00000000",
        "percent_change": "0.00",
        "base_volume": "0.00000000",
        "quote_volume": "0.00000000"
    },
    {
        "id": "CRCO_BTS",
        "quote": "CRCO",
        "base": "BTS",
        "latest": "0.00000000",
        "lowest_ask": "0.00000000",
        "highest_bid": "0.00000000",
        "percent_change": "0.00",
        "base_volume": "0.00000000",
        "quote_volume": "0.00000000"
    },
    {
        "id": "CRCO_BTC",
        "quote": "CRCO",
        "base": "BTC",
        "latest": "0.00000000",
        "lowest_ask": "0.00000000",
        "highest_bid": "0.00000000",
        "percent_change": "0.00",
        "base_volume": "0.00000000",
        "quote_volume": "0.00000000"
    }
]
```




### Specific ticker
```
GET /api/v1/ticker/:market_id
```
