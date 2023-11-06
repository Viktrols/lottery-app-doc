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

<h2> Lotto regular </h2> <br>
POST with params:

```           
f_game_type: "lotto",
f_game_version: "lotto_regular",
f_is_double: "1" if true, else "0",
f_is_extra: "1" if true, else "0",

f_games_count:  "1",  -- always "1"
f_total_sum: "31.20",  -- total sum
f_pay_method: "credit_card"/"balance"/"bit"/"applepay",
f_is_subscription: "1" if user want to subscribe, else "0",
f_subscription_days: if subscription, count of days STR, 2/3/etc, "infinity" if each next game
f_subscription_automatic:  "1" if true, else "0"

IF NOT DOUBLE:

nums_regular_line_1: "21;28;30;33;34;35;" - selected numbers in first string with separator ';' (from 01 to 37)
nums_regular_line_2: "01;28;30;33;34;35;" - selected numbers in second string
nums_regular_line_3: "01;28;30;33;34;35;" 
nums_regular_line_4: "01;28;30;33;34;35;" 
nums_regular_line_5: "01;28;30;33;34;35;"
nums_regular_line_6: "01;28;30;33;34;35;"
nums_regular_line_7: "01;28;30;33;34;35;"
nums_regular_line_8: "01;28;30;33;34;35;"
nums_regular_line_9: "01;28;30;33;34;35;"
nums_regular_line_10: "01;28;30;33;34;35;"
nums_regular_line_11: "01;28;30;33;34;35;"
nums_regular_line_12: "01;28;30;33;34;35;"
nums_regular_line_13: ""
nums_regular_line_14: ""

nums_regular_strong_1: "1" -- selected strong number in first line (1/2/3/4/5/6/7)
nums_regular_strong_2: "3" -- selected strong number in second line (1/2/3/4/5/6/7)
nums_regular_strong_3: ""
nums_regular_strong_4: ""
nums_regular_strong_5: ""
nums_regular_strong_6: ""
nums_regular_strong_7: ""
nums_regular_strong_8: ""
nums_regular_strong_9: ""
nums_regular_strong_10: ""
nums_regular_strong_11: ""
nums_regular_strong_12: ""
nums_regular_strong_13: ""
nums_regular_strong_14: ""


IF DOUBLE:

nums_double_line_1: "02;28;30;33;34;35;" - selected numbers in first string with separator ';' (from 01 to 37)
nums_double_line_2: ""
nums_double_line_3: ""
nums_double_line_4: ""
nums_double_line_5: ""
nums_double_line_6: ""
nums_double_line_7: ""
nums_double_line_8: ""
nums_double_line_9: ""
nums_double_line_10: ""

nums_double_strong_1: "7" -- selected strong number in first line (1/2/3/4/5/6/7)
nums_double_strong_2: "1"
nums_double_strong_3: ""
nums_double_strong_4: ""
nums_double_strong_5: ""
nums_double_strong_6: ""
nums_double_strong_7: ""
nums_double_strong_8: ""
nums_double_strong_9: ""
nums_double_strong_10: ""
```

<h2> Lotto systematic / strong </h2> <br>
POST with params:

```           
f_game_type: "lotto",
f_game_version: "lotto_systematic" / "lotto_strong",
f_is_double: "1" if true, else "0",
f_is_extra: "1" if true, else "0",

f_games_count:  "1",  -- always "1"
f_total_sum: "31.20",  -- total sum
f_pay_method: "credit_card"/"balance"/"bit"/"applepay",
f_is_subscription: "1" if user want to subscribe, else "0",
f_subscription_days: if subscription, count of days STR, 2/3/etc, "infinity" if each next game
f_subscription_automatic:  "1" if true, else "0"

f_form_type: "8", STR (8/5/9/10/11/12 - if systematic, 4/5/6/7 - if strong)
f_nums_line: "01;03;07;09;12;18;21;22;27;33;" - selected numbers with separator ';' (from 01 to 37),
f_nums_strong: "1;3;4;7;" selected strong numbers with separator ';'(1/2/3/4/5/6/7),

```


<h1>url: 'calc_game_lotto_sum/'</h1>

<h2> 123 game</h2> <br>
POST with params:

```
ticket_type:  "game123_regular",
form_type: count of selected lines, STR, 1/2/3/4/5,
price: selected price, STR, 1/2/3/5/10/25,

is_subscription: "1" if user want to subscribe, else "0",
subscription_days: if subscription, count of days STR, 2/3/etc, "infinity" if each next game
```

<h2> 777 game</h2> <br>
POST with params:

```
ticket_type: "game777_regular"/"game777_col8"/"game777_col9",
form_type:  count of selected lines, STR, 1/2/3, -- always "1" if "game777_col8" or "game777_col9",

is_subscription: "1" if user want to subscribe, else "0",
subscription_days: if subscription, count of days STR, 2/3/etc, "infinity" if each next game
```

<h2> Chance </h2> <br>
POST with params:

```
ticket_type: 'chance_regular'/'chance_multi'/'chance_systematic',
price: selected price, STR, 5/10/25/50/70/100/250,
card_hearts: "A", selected card heart, STR, 7/8/9/10/J/Q/K/A if 'chance_regular'/'chance_multi' "78QA", selected cards heart in one string, STR, 7/8/9/T/J/Q/K/A, ('10' = 'T') if 'chance_systematic',
card_spades: '' -- same as card_hearts,
card_diamonds: '' -- same as card_hearts,
card_clubs: '' -- same as card_hearts,

is_subscription: "1" if user want to subscribe, else "0",
subscription_days: if subscription, count of days STR, 2/3/etc, "infinity" if each next game
```

<h2> Lotto regular </h2> <br>
POST with params:

```
ticket_type: "lotto_regular",
count_lines: '4', number of completely filled lines,
is_double: "1" if true, else "0",
is_extra: "1" if true, else "0",

is_subscription: "1" if user want to subscribe, else "0",
subscription_days: if subscription, count of days STR, 2/3/etc, "infinity" if each next game
```

<h2> Lotto</h2> <br>
POST with params:

```
ticket_type: "lotto_regular"/"lotto_systematic"/"lotto_strong"

count_lines: '4', number of completely filled lines,  --- only if "lotto_regular"
form_type: "8", STR (8/5/9/10/11/12 - if systematic, 4/5/6/7 - if strong)  --- only if "lotto_systematic"/"lotto_strong",

is_double: "1" if true, else "0",
is_extra: "1" if true, else "0",

is_subscription: "1" if user want to subscribe, else "0",
subscription_days: if subscription, count of days STR, 2/3/etc, "infinity" if each next game
```

