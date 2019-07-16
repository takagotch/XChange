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
AccountInfo accountInfo = accountService.getAccountInfo();
System.out.println(accountInfo.toString);
```

```
<dependency>
  <groupId>org.knowm.xchange</groupId>
  <artifactId>xchange-core</artifactId>
  <version>4.3.20</version>
</dependency>
<dependency>
  <groupId>org.knowm.xchange</groupId>
  <artifactId>xchange-XYZ</artifactId>
  <version>4.3.20</version>
</dependency>

<repository>
  <id>sonatype-oss-snapshot</id>
  <snapshots/>
  <url>https://oss.sonatype.org/content/repositories/snapshots</url>
</repository>
```

```
```


