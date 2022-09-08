# expretoption
Website    : https://autotradevip.com/en/  
Olmyptrade : https://youtu.be/zTZT7zDlmtU  
Binomo     : https://youtu.be/ww9rVMX5TK4  
IQ Option  : https://youtu.be/4i3YUEDRGWY  
Quotex     : https://www.youtube.com/channel/UCCqnm8XHUoc0Ude78RJwmoA  
Expert Option     : https://www.youtube.com/channel/UCCqnm8XHUoc0Ude78RJwmoA
### Import
```python
from expertoptionapi.stable_api import expertoption
```

### Login by ssid
if connect sucess return True,None  

if connect fail return False,None  
```python
from expertoptionapi.stable_api import expertoption
ssid="""{"action":"setContext","message":{"is_demo":1},"token":"ffd62aef2f07c925753cd7dc7854cd5","ns":1}"""
account=expertoption(set_ssid=ssid)
check_connect,message=account.connect()
print(check_connect,message)
```

### Check_win & buy sample

```python
from expertoptionapi.stable_api import expertoption
ssid="""{"action":"setContext","message":{"is_demo":1},"token":"ffd62aef2f07c925753cd7dc7854cd5","ns":1}"""
account=expertoption(set_ssid=ssid)
check_connect,message=account.connect()
if check_connect:
    account.change_balance("PRACTICE")#"REAL"
    check,id = API.buy("topcryptoindex", "1", "put", "60") #True, id_number
    print(API.check_win(id))
```
