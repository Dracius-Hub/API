# __PlayerDataService__
This service manages player profiles and interactions with individual player data.

## __Public Methods__

### ChangeStat
Changes the ```Player``` passed ```stat``` to ```val```.
```
PlayerDataService:ChangeStat(inst Player, str statName, int val)
```

### AssignQuest
Assigns a quest to the ```Player``` passed.
```
PlayerDataService:AssignQuest(inst Player, quest Quest, str questId)
```

### GetProfile
Returns the active profile for the ```Player``` passed
```
PlayerDataService:GetProfile(inst Player) -> profile
```

### GetSignals
Returns the active signals or the ```Player``` passed
```
PlayerDataService:GetSignals(inst Player) -> Dictionary<signalName, signal>
```

### GetStat
Returns the ```stat``` value of the passed ```Player```.
```
PlayerDataService:GetStat(inst Player, str statName) -> any
```

### GetActiveQuests
Returns a list of active quests for the ```Player``` passed.
```
PlayerDataService:GetActiveQuests(inst Player) -> Dictionary<questId, quest>
```

### GetMode
Returns the ```Player```'s current selected mode based on the ```modeType``` passed.
```
PlayerDataService:GetMode(inst Player, str modeType) -> str 
```

## GetEnergyColor
Returns EnergyColor of the ```Player```
```
PlayerDataService:GetEnergyColor(inst Player) -> Color3
```

## __Private Methods__

### _loadProfile
Loads the profile of the ```Player``` passed.
```
PlayerDataService:_loadProfile(inst Player)
```

### _releaseProfile
Destroys the profile of the ```Player``` passed.
```
PlayerDataService:_releaseProfile(inst Player)
```

### _createSignals
Creates signal objects for the ```Player``` passed.
```
PlayerDataService:_createSignals(inst Player)
```

---
## Profile Template
---
```
local ProfileTemplate = {
	Stats = {
		Endurance = 0;
		KiControl = 0;
		Strength = 0;
		Speed = 0;
	};

	Character = {
		EnergyColor = "0,170,255";
	};

	Mode = {
		Mode = "SSJ";
		Stack = "Kaioken";
	};

	Settings = {
		GraphicsLevel = 3;
		PowerOutput = 100;
	};

	Inventory = {};

	Skills = {};
}
```