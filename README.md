# PBOS - PassivBotOnlyStrategy

PBOS is a group of person working in Passivbot strategies.

**Discord Members :**
- MDCL : https://github.com/Skanouch/passivbot
- DotCom : https://github.com/raftheunis87/pb-configs
- Flyingtoaster : https://github.com/donewiththedollar/passivbot_v5.7.0
- Tedy : https://github.com/tedyptedto/passivbot
- enarjord : https://github.com/enarjord/passivbot/
- krishna_nx : N/C
- rygreen93 : N/C
- Miguelito : N/C

## PassivBot Strategies

Startegies :
- [Sorted by categ and long adg](https://github.com/tedyptedto/pbos/blob/main/strategy_sorted_by_categ_and_long_adg.csv)
- [Sorted by coin and long adg](https://github.com/tedyptedto/pbos/blob/main/strategy_sorted_by_coin_and_long_adg.csv)
- [Sorted by long adg](https://github.com/tedyptedto/pbos/blob/main/strategy_sorted_by_long_adg.csv)
- [Sorted by stars and long adg](https://github.com/tedyptedto/pbos/blob/main/strategy_sorted_by_stars_and_long_adg.csv)

## PassivBot Strategies backtested with same parameters
The goal is to backtest all strategies with the same backtest parameters :
- **1 second candles** very occurate
- coin list (XRPUSDT, LTCUSDT, ADAUSDT, DOTUSDT, UNIUSDT, DOGEUSDT, MATICUSDT, BNBUSDT, SOLUSDT, TRXUSDT, AVAXUSDT)
- From 2020-01-01 to 2022-07-23
- starting_balance : 1000 $
- wallet exposure : 1 (we is auto adjusted to 1 for the sum of long and short wallet exposure)

Results :
- [All backtest](https://github.com/tedyptedto/pbos/blob/main/bt_2020-01-01_2022-07-23_1000_1_XRPUSDT_LTCUSDT_ADAUSDT_DOTUSDT_UNIUSDT_DOGEUSDT_MATICUSDT_BNBUSDT_SOLUSDT_TRXUSDT_AVAXUSDT_USDCUSDT.csv)
- [Strategies having this requirements](https://github.com/tedyptedto/pbos/blob/main/best_bt_2020-01-01_2022-07-23_1000_1_XRPUSDT_LTCUSDT_ADAUSDT_DOTUSDT_UNIUSDT_DOGEUSDT_MATICUSDT_BNBUSDT_SOLUSDT_TRXUSDT_AVAXUSDT_USDCUSDT.csv) :
  "-min-eqbal_ratio_min_long", "0.8", "-max-stuck-avg", "2", "-min-gridspan", "19", "-min-gain", "100", "-max-pa_distance_mean_long", "0.02", "-max-loss_sum_long","500"

### Legend

- bt_* = Informations relative to backtesting
- l_* = Informations on the strategy for Long side
- s_* = Informations on the strategy for Short side
- "uid" : Unique Id for the config.json,
- "info" : Link to the config.json and bulk config,
- "categ" : name of the bulk,
- "bt_balance" : starting_balance,
- "bt_coin" : Symbol backtested,
- "bt_days" : No. days,
- "bt_l_adg" : Long ADG realized per exposure,
- "bt_s_adg" : Short ADG realized per exposure,
- "long" : Long enabled,
- 'l_AU' : Long AutoUnstuck enabled,
- "l_gspan" : Long grid_span (height of the grid),
- "l_TP"  : Long TP distance / TP zone height /,
- "short" : Short enabled,
- 's_AU' : Short AutoUnstuck enabled,
- "s_gspan" : Short grid_span (height of the grid),
- "s_TP"  : Long TP distance / TP zone height /,

