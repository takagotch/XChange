### xchange
---
https://github.com/knowm/XChange

```java
Exchange bitstamp = ExchangeFactory.INSTANCE.createExchange(BitstampExchange.class.getName);
MarketDataService marketDataService = bitstamp.getMarketDataService();
Ticker ticker = marketDataService.getTicker(CurrencyPair.BTC_USD);
System.out.println(ticker.toString());


ExchangeSpecification exSpec = new BitstampExchange().getDefaultExchangeSpecification();
exSpec.setUserName("34387");
exSpec.setApiKey("xxx");
exSpec.setSecretKey("xxx");
Exchange bitstamp = ExchangeFactory.INSTANCE.createExchange(exSpec);

AccountService accountService = bitstamp.getAccountService();
AccountInfo
```

```
```

```
```


