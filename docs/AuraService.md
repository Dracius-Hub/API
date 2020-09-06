# __AuraService__
Wraps AuraManagers and creates one for each player

---
### __GetAuraManager__
---
```
AuraService[Player] -> indexs the AuraManager
```


---
## __Public Methods__
---

### GiveAura
Gives the ```Player``` the specified ```Aura```

```
AuraService:GiveAura(inst Player, str aura)
```

### RemoveAura
Removes the ```Aura``` specified from the ```Player```

```
AuraService:RemoveAura(inst Player, str aura)
```

---
## __Private Methods__
---

### _createManager
Creates an AuraManager for ```Player```

```
AuraService:_createManager(inst Player)
```

### _destroyManager
Destroys the AuraManager for ```Player```

```
AuraService:_destroyManager(inst Player)
```
