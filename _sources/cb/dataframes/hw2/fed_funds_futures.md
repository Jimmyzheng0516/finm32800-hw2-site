# Dataframe: `hw2:fed_funds_futures` - 30-Day Fed Funds Futures (ZQ) Daily Bars

Daily OHLCV bars (schema ohlcv-1d) from the Databento GLBX.MDP3 dataset (CME Globex MDP 3.0), pulled with the parent symbol ZQ.FUT so one request returns every listed ZQ contract. Columns: date (trading date, tz-naive), symbol, open, high, low, close, volume. A contract settles at 100 minus the average daily effective fed funds rate over its month, so 100 minus the close is the market's forecast of that average rate, in percent. Symbols such as ZQU6 are outright monthly contracts (month code plus last digit of the year); symbols such as ZQU6-ZQZ6 are calendar spreads and should be dropped with fedwatch.filter_outright_contracts before computing rates. Thinly traded far months may not have a bar every day. The pull checks the query cost first and refuses to download unless it is $0.00 under the course subscription.


## DataFrame Glimpse

```
Rows: 11653
Columns: 7
$ date   <datetime[ns]> 2026-10-25 00:00:00
$ symbol          <str> 'ZQG7-ZQJ7'
$ open            <f64> 15.5
$ high            <f64> 16.0
$ low             <f64> 15.5
$ close           <f64> 16.0
$ volume          <u64> 333


```

## Dataframe Manifest

| Dataframe Name                 | 30-Day Fed Funds Futures (ZQ) Daily Bars                                                          |
|--------------------------------|--------------------------------------------------------------------------------------|
| Dataframe ID                   | [fed_funds_futures](../dataframes/hw2/fed_funds_futures.md)                                       |
| Sources                        | CME Globex                                          |
| Providers                      | Databento                                        |
| Provider Links                 | https://databento.com/                                   |
| Tags                           | Monetary Policy, Futures, Fed Funds, Fedwatch                                             |
| Access Types                   |                                       |
| How is data pulled?            | Databento API via Python                                                   |
| Data available up to (min)     | 2026-10-25 00:00:00                                                             |
| Data available up to (max)     | 2026-10-25 00:00:00                                                             |
| Dataframe Path                 | /sessions/rcw-011twcneuvo2vkpuyg5ufzvx/hw2/_data/fed_funds_futures.parquet                                             |


**Linked Charts:**


- [hw2:fedwatch_latest_forecast](../../charts/hw2.fedwatch_latest_forecast.md)



## Pipeline Manifest

| Pipeline Name                   | HW 2: The Yield Curve and the Policy Path                       |
|---------------------------------|--------------------------------------------------------|
| Pipeline ID                     | [hw2](../../../index.md)              |
| Maintainer                      | Jeremiah Bejarano               |
| Contributors                    | Jeremiah Bejarano |
| Repository                     | https://github.com/hw-finm-32800/hw2                  |
| Pipeline Web Page               | <a href="file:///sessions/rcw-011twcneuvo2vkpuyg5ufzvx/hw2/docs/index.html">Pipeline Web Page      |
| Date of Last Code Update        | 2026-10-27 07:11:24           |
| OS Compatibility                | Windows, Linux, macOS |
| Linked Dataframes               |  [hw2:crsp_treasury_consolidated](../../dataframes/hw2/crsp_treasury_consolidated.md)<br>  [hw2:fed_yield_curve](../../dataframes/hw2/fed_yield_curve.md)<br>  [hw2:fed_funds_futures](../../dataframes/hw2/fed_funds_futures.md)<br>  |


**Build Commands:**
```
doit

```

