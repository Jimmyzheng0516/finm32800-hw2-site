# Dataframe: `hw2:crsp_treasury_consolidated` - CRSP Treasury Consolidated

Consolidated CRSP US Treasury database combining daily pricing data (prices, yields, durations) with issue-level characteristics (coupon, maturity, issue date). Sourced from WRDS.


## DataFrame Glimpse

```
Rows: 2530592
Columns: 20
$ kytreasno                  <f64> 200636.0
$ kycrspid                   <str> '19700215.104000'
$ tcusip                     <str> '912810AE'
$ caldt             <datetime[ns]> 1970-01-02 00:00:00
$ tdatdt            <datetime[ns]> 1965-01-15 00:00:00
$ tmatdt            <datetime[ns]> 1970-02-15 00:00:00
$ tfcaldt                    <i64> 0
$ tdbid                      <f64> 99.5
$ tdask                      <f64> 99.5625
$ tdaccint                   <f64> 1.5217391304348
$ tdyld                      <f64> 0.00021199520830037
$ price                      <f64> 101.0529891304348
$ tcouprt                    <f64> 4.0
$ itype                      <f64> 1.0
$ original_maturity          <f64> 5.0
$ years_to_maturity          <f64> 0.0
$ tdduratn                   <f64> 44.0
$ tdretnua                   <f64> 0.00083430893652524
$ days_to_maturity           <i64> 44
$ callable                  <bool> False


```

## Dataframe Manifest

| Dataframe Name                 | CRSP Treasury Consolidated                                                          |
|--------------------------------|--------------------------------------------------------------------------------------|
| Dataframe ID                   | [crsp_treasury_consolidated](../dataframes/hw2/crsp_treasury_consolidated.md)                                       |
| Sources                        | CRSP                                          |
| Providers                      | WRDS                                        |
| Provider Links                 | https://wrds-www.wharton.upenn.edu/                                   |
| Tags                           | Treasury, Fixed Income, Yield Curve                                             |
| Access Types                   |                                       |
| How is data pulled?            | WRDS via Python                                                   |
| Data available up to (min)     | N/A (large file)                                                             |
| Data available up to (max)     | N/A (large file)                                                             |
| Dataframe Path                 | /sessions/rcw-011twcneuvo2vkpuyg5ufzvx/hw2/_data/TFZ_consolidated.parquet                                             |


**Linked Charts:**

- None


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

