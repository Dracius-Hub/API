# QuestService
A wrapper Service for the QuestManagerClass. 
Handles giving quests and cancelling quests.

---
## Public Methods
---

### LoadPlayer
Creates a ```QuestManager``` Object for the ```Player``` passed.
```
QuestService:LoadPlayer(inst Player)
```

### EndSession
Destroys the ```QuestManager``` Object for the ```Player``` passed.
```
QuestService:EndSession(inst Player)
```

### GiveQuest
Gives a new quest to the ```Player``` based on the ```questInfo``` passed.
```
QuestService:GiveQuest(inst Player, table questInfo)
```

### RemoveQuest
Removes a specified quest from the ```Player``` 
```
QuestService:RemoveQuest(inst player, int id)
```