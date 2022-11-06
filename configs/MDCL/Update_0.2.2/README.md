Update Scalp Harmony Search NEAT 0.2.2 | Take Profit 0.5% MAX | Opti settings | Lower EMA's  | AU Enabled

Idea behind the strategie :

- Increased grid a little bit on long side
- Increased grid on short side
- Increased entries and standard max long only
- Keep initial_qty_pct to 0.01
- Increased QTT from entries, standard distance between them, 1.0 | 3.0.
- Keep price action to a minimum. 
- Full passive - Auto Unstuck On with new threshold from enarjord remark 0.1 Max.

Tried the 0.05 on threshold, seems to work fine. Max hours stuck is higher but the losses from AU are lower, for this new bulk opti i'll increase a bit to 0.1, trying to reduce max hours stuck. 
Remark from dotcom87, force auto_unstuck_ema_dist to min 0.001

Long min Grid = 25% | Long max Grid = 40%
Short min Grid = 35% | Short max Grid = 50%
adg_PAD_std = 0.015
adg_realized_PAD_mean = 0.015 
 
  adg_PAD_std:
  adg / max(max_pa_dist_std, mean([max(max_pa_dist_std, PAD_std) for PAD_std in results]))
  maximum_pa_distance_std_long: 0.015
  maximum_pa_distance_std_short: 0.015

  adg_realized_PAD_mean:
  adg_realized / max(max_pa_dist_mean, mean([max(max_pa_dist_mean, PAD_mean) for PAD_mean in results]))
  
  maximum_pa_distance_mean_long: 0.015
  maximum_pa_distance_mean_short: 0.015

    long:

      grid_span: [0.25, 0.4]
      ema_span_0: [10, 2000]
      ema_span_1: [10, 5000]
      wallet_exposure_limit: [0.1, 0.1]
      max_n_entry_orders: [7, 20]
      initial_qty_pct: [0.01, 0.01]
      initial_eprice_ema_dist: [-0.1, 0.0]
      eqty_exp_base: [1.5, 3.0]
      eprice_exp_base: [1.0, 3.0]
      min_markup: [0.002, 0.002]
      markup_range: [0.000, 0.003]
      n_close_orders: [5, 20]
      auto_unstuck_wallet_exposure_threshold: [0.0, 0.1]
      auto_unstuck_ema_dist: [0.0001, 0.1]

    short:

      grid_span: [0.35, 0.5]
      ema_span_0: [10, 4000]
      ema_span_1: [10, 8000]
      wallet_exposure_limit: [0.1, 0.1]
      max_n_entry_orders: [7, 20]
      initial_qty_pct: [0.01, 0.01]
      initial_eprice_ema_dist: [-0.1, 0.0]
      eqty_exp_base: [1.5, 3.0]
      eprice_exp_base: [1.0, 3.0]
      min_markup: [0.002, 0.002]
      markup_range: [0.000, 0.003]
      n_close_orders: [5, 20]
      auto_unstuck_wallet_exposure_threshold: [0.0, 0.1]
      auto_unstuck_ema_dist: [0.0001, 0.1]
