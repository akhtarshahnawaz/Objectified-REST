# Objectified REST is a wrapper for ORM style access to REST APIs

This package allows to call REST endpoints the way we access objects and object properties. You can also pass parameters to refine the result and authenticate to access private data.

To install

```python
pip install objectifiedrest
```

Then to use the package

```python
from objectifiedrest import ORest

c = ORest(url = 'https://www.deribit.com/api/v2', client_id = 'xxxx',client_secret='xxxx')
c.private_get_positions(currency = "ETH",kind = "option").raw()
c.get_instruments(currency='BTC',kind='future',expired='false').raw()
```
