# __AuraManager__
This class handles auras for each player

## __Constructors__

### .new
Creates a new AuraManager for the passed ```Player```
```
AuraManager.new(inst Player) -> AuraManager
```

## __Public Methods__

### GiveAura
Gives an Aura to the Player its assigned to manage.
```
AuraManager:GiveAura(inst Aura)
```

### RemoveAura
Removes the specified aura depending on the ```method``` passed.
```
Methods:
	instant
	<any>
```
```
AuraManager:RemoveAura(str auraName, str method)
```

### ToggleAura
Toggles whether the auras are active or not
```
AuraManager:ToggleAura(bool enabled)
```

### ToggleInnerAura
Toggles the glowing inside of the aura. 
Note: Create definition of "InnerAura" for useful links
```
AuraManager:ToggleInnerAura(bool enabled)
```

### GetColors
Returns the colors of all auras (active and inactive).
Note: Finish creating this function
```
AuraManager:GetColors() -> ColorSequence, ColorSequence
```

### GetGlowAuras
Returns the Auras that glow, an example of a glow aura is MUI's.
```
AuraManager:GetGlowAuras(str auraName) -> Array<auras>
```

