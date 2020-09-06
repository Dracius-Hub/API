# ModeService
This service is used to handle all modes that players use, aswell as activating their draining systems, boost systems, etc.

---
## Public Methods
---

### Ascend
Transforms the ```Player``` into to the mode they have selected, based on the ```modeType``` passed.
```
ModeService:Ascend(inst Player, str modeType)
```

### Descend
Reverts the ```Player``` into base form, based on the ```modeType``` passed
If the passed ```modeType``` is "Mode" then the player will return to base state.
```
ModeService:Descend(inst Player, str modeType, bool doNotShowEffects)
```

### TransformPlayer
Decides whether to ascend or descend the ```Player```, based on the ```modeType``` passed.
```
ModeService:TransformPlayer(inst Player, str modeType)
```

### GetPlayerModeNames
Returns an array ```activeModes``` that contains all modes the ```Player``` has active
```
ModeService:GetPlayerModeNames(inst Player) -> Dictionary<modeName, modeType>
```

### GetModesByType
Returns a dictionary that contains all modes the ```Player``` has active
```
ModeService:GetModesByType(inst Player) -> Dictionary<modeType, modeName>
```

---
## Private Methods
---

###resetPlayer
Destroys all ```Mode``` Objects that the ```Player``` has active
```
ModeService:_resetPlayer(inst Player)
```

###handleCharacter
Whenever a new character is added from the ```Player```, then destroy the modes
```
ModeService:_handleCharacter(inst Player)
```