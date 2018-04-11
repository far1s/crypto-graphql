## Getting started
```shell
npm start
````
Go to `localhost:4000/graphql`

## Fetching documents
Fetch all currencies
```graphql
{
    coins {
      	rank,
      	symbol,
        percent_change_24h,
        price_usd,
    }
}

```

Fetch a specific coin by coin id (String)
```graphql
{
  coins(id: "bitcoin") {
    id,
    name,
    symbol,
    rank,
    price_usd,
    price_btc,
    h24_volume_usd,
    market_cap_usd,
    available_supply,
    total_supply,
    percent_change_1h,
    percent_change_24h,
    percent_change_7d
  }
}
```
