<h1>url: 'cab-game-lotto-save/'</h1>
<h2> 123 game</h2> <br>
POST with params:
  
```
f_game_type: "123", 
f_game_version: "game123_regular",
f_form_type: count of selected lines, STR, 1/2/3/4/5, 
f_block1: selected numbers in block 1 in one string, STR, example: "456",
f_block2: "126",
f_block3: "567",
f_block4: "",
f_block5: "",
f_price: selected price, STR, 1/2/3/5/10/25,
f_games_count: "1",  -- always "1"
f_total_sum: "60",  -- total sum
f_pay_method: "credit_card"/"balance"/"bit"/"applepay",
f_is_subscription: "1" if user want to subscribe, else "0",
f_subscription_days: if subscription, count of days STR, 2/3/etc, "infinity" if each next game
f_subscription_automatic:  "1" if true, else "0"
```

<h2> 777 game</h2> <br>
POST with params:

```
f_game_type: "777",
f_game_version: "game777_regular"/"game777_col8"/"game777_col9",
f_form_type: count of selected lines, STR, 1/2/3, -- always "1" if "game777_col8" or "game777_col9"
f_line_1: selected numbers in one string, STR, example: "04;22;27;45;48;57;70;",
f_line_2: "",
f_line_3: "",
f_games_count:  "1",  -- always "1"
f_total_sum: "60",  -- total sum
f_pay_method: "credit_card"/"balance"/"bit"/"applepay",
f_is_subscription: "1" if user want to subscribe, else "0",
f_subscription_days: if subscription, count of days STR, 2/3/etc, "infinity" if each next game
f_subscription_automatic:  "1" if true, else "0"
```

<h2> Chance game Regular and Multi</h2> <br>
POST with params:

```           
f_game_type: "chance",
f_game_version: "chance_regular"/"chance_multi",
f_form_type: count of selected card suits, STR, 1/2/3/4,
f_card_hearts: "A", selected card heart, STR, 7/8/9/10/J/Q/K/A,
f_card_spades: "",selected card spade, STR, 7/8/9/10/J/Q/K/A,
f_card_diamonds: "", selected card diamond, STR, 7/8/9/10/J/Q/K/A,
f_card_clubs: "", selected card club, STR, 7/8/9/10/J/Q/K/A,
f_price: selected price, STR, 5/10/25/50/70/100/250,
f_games_count:  "1",  -- always "1"
f_total_sum: "60",  -- total sum
f_pay_method: "credit_card"/"balance"/"bit"/"applepay",
f_is_subscription: "1" if user want to subscribe, else "0",
f_subscription_days: if subscription, count of days STR, 2/3/etc, "infinity" if each next game
f_subscription_automatic:  "1" if true, else "0"
```

<h2> Chance game Systematic</h2> <br>
POST with params:

```           
f_game_type: "chance",
f_game_version: "chance_systematic",
f_form_type: count of selected card suits, STR, 1/2/3/4,
f_card_hearts: "78QA", selected cards heart in one string, STR, 7/8/9/T/J/Q/K/A, ('10' = 'T')  
f_card_spades: "9J",selected cards spade in one string, STR, 7/8/9/T/J/Q/K/A, ('10' = 'T')  
f_card_diamonds: "KA", selected cards diamond in one string, STR, 7/8/9/T/J/Q/K/A, ('10' = 'T')  
f_card_clubs: "789T", selected cards club in one string, STR, 7/8/9/T/J/Q/K/A, ('10' = 'T')  
f_price: selected price, STR, 5/10/25/50/70/100/250,
f_games_count:  "1",  -- always "1"
f_total_sum: "60",  -- total sum
f_pay_method: "credit_card"/"balance"/"bit"/"applepay",
f_is_subscription: "1" if user want to subscribe, else "0",
f_subscription_days: if subscription, count of days STR, 2/3/etc, "infinity" if each next game
f_subscription_automatic:  "1" if true, else "0"
```

