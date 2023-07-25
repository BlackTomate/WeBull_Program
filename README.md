# Webull Project
APIs for webull, you are free to use, but code not extensively checked and Webull may update the APIs or the endpoints at any time.
https://www.webull.com/

# Install

```
pip install webull

or

python3 -m pip install webull
```

# Run tests

```
pip install pytest requests_mock
python -m pytest -v
```

```
from webull import webull # for paper trading, import 'paper_webull'

wb = webull()
wb.login('test@test.com', 'pa$$w0rd')

```

How to login with your mobile
```
from webull import webull # for paper trading, import 'paper_webull'

wb = webull()
wb.login('+1-1112223333', 'pa$$w0rd') # phone must be in format +[country_code]-[your number]

```

How to order stock
```
from webull import webull
wb = webull()
wb.login('test@test.com', 'pa$$w0rd')

wb.get_trade_token('123456')
wb.place_order(stock='AAPL', price=90.0, qty=2)
```

How to check standing orders
```
from webull import webull
wb = webull()
wb.login('test@test.com', 'pa$$w0rd')

wb.get_trade_token('123456')
orders = wb.get_current_orders()
```

How to cancel standing orders
```
from webull import webull
wb = webull()
wb.login('test@test.com', 'pa$$w0rd')

wb.get_trade_token('123456')
wb.cancel_all_orders()
```

# FAQ
Thank you so much, I have received Emails and messages on reddit from many traders/developers that liked this project. Thanks to many that helped and contributed to this project too! There are quite a few repeated questions on the same topic, so I have utilized the Wiki section for them. If you have troubles regarding *Login/MFA Logins*, *Real Time Quote Data*, *What is Trade PIN/Trade Token*, or *How to buy me a coffee* please take a look at the Wiki pages first.


# Developers
If you are interested to join and help me improve this, feel free to message me.
