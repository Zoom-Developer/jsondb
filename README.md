<h1>JSON DB</h1>
<h3>Simple python local database</h3>

***Install:***
```
pip install jsondbpy
```

***Quick start:***

```python
from jsondb import Manager

manager = Manager("database.test")
data = manager.get()
if not data.get("nick"): 
    data["nick"] = input("Enter your nickname: ")
    manager.save()
nick = data["nick"]
print("Hello, %s" % nick)
```

    First start
```
>>> Enter your nickname: ZoomDeveloper
Hello, ZoomDeveloper
```
    Restart script
```
Hello, ZoomDeveloper
```
