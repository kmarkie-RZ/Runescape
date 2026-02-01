**Client -> Server Packets**

---

## **Client -> Server Packets**

### **1. Opcode 0: Idle**
- **Type**: FIXED
- **Length**: 0 bytes
- **Description**: Sent when there are no actions being performed by the player for this cycle. This is used to keep the connection alive.

---

### **2. Opcode 3: Focus Change**
- **Type**: FIXED
- **Length**: 1 byte
- **Description**: Sent when the game client window goes in and out of focus. This is used to pause or resume the game.

---

### **3. Opcode 4: Chat**
- **Type**: VARIABLE_BYTE
- **Length**: N/A
- **Description**: Sent when the player enters a chat message. This is used for public chat communication.

---

### **4. Opcode 14: Item on Player**
- **Type**: FIXED
- **Length**: 8 bytes
- **Description**: Sent when a player uses an item on another player. This is used for interactions like trading or healing.

---

### **5. Opcode 16: Alternate Item Option 2**
- **Type**: FIXED
- **Length**: 1 byte
- **Description**: Sent when a player uses an item. This is an alternate item option, such as "Use" or "Drop."

---

### **6. Opcode 17: NPC Action 2**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sent when a player clicks the second option of an NPC (e.g., "Attack" or "Trade").

---

### **7. Opcode 18: NPC Action 4**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sent when a player clicks the fourth option of an NPC (e.g., "Pickpocket" or "Follow").

---

### **8. Opcode 21: NPC Action 3**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sent when a player clicks the third option of an NPC (e.g., "Talk-to" or "Pickpocket").

---

### **9. Opcode 25: Item on Floor**
- **Type**: FIXED
- **Length**: 10 bytes
- **Description**: Sent when a player uses an item on another item on the floor. This is used for combining items or special actions.

---

### **10. Opcode 35: Magic on Object**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Sent when a player uses magic on an object. This is used for spells like Alchemy or Telekinesis.

---

### **11. Opcode 36: Anti-Cheat (Walking)**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Sent to validate walking. This is used to prevent cheating or botting.

---

### **12. Opcode 39: Follow**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sent when a player clicks the follow option on another player. This is used to follow another player in the game.

---

### **13. Opcode 40: Dialogue**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sent when a player continues a dialogue. This is used to progress through NPC conversations.

---

### **14. Opcode 41: Equip Item**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when a player equips an item. This updates the player's equipment interface.

---

### **15. Opcode 43: Bank 10 Items**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when a player banks 10 of a certain item. This is used for quick banking actions.

---

### **16. Opcode 45: Flagged Account**
- **Type**: FIXED
- **Length**: 1 byte
- **Description**: Sent when a player's account is flagged. This is used for anti-cheat or moderation purposes.

---

### **17. Opcode 53: Item on Item**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Sent when a player uses an item with another item. This is used for combining items or crafting.

---

### **18. Opcode 57: Item on NPC**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Sent when a player uses an item on an NPC. This is used for interactions like feeding or enchanting.

---

### **19. Opcode 60: Typing onto Interface**
- **Type**: FIXED
- **Length**: 1 byte
- **Description**: Sent while typing onto an interface. This is used for text input fields.

---

### **20. Opcode 70: Object Action 3**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when the player clicks the third action available for an object (e.g., "Climb" or "Search").

---

### **21. Opcode 72: Attack (NPC)**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sent when a player attacks an NPC. This initiates combat with the NPC.

---

### **22. Opcode 73: Attack (Player)**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sent when a player selects the attack option on another player. This initiates PvP combat.

---

### **23. Opcode 74: Remove Ignore**
- **Type**: FIXED
- **Length**: 8 bytes
- **Description**: Sent when a player removes a player from their ignore list. This allows communication with the previously ignored player.

---

### **24. Opcode 75: Item Action 3**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when a player clicks the third option of an item (e.g., "Use" or "Destroy").

---

### **25. Opcode 79: Light Item**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when a player attempts to light logs on fire. This is used for firemaking actions.

---

### **26. Opcode 85: Anti-Cheat (NPC Option 4)**
- **Type**: FIXED
- **Length**: 1 byte
- **Description**: Sent to validate NPC option 4. This is used to prevent cheating or botting.

---

### **27. Opcode 86: Camera Movement**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Sent when the player moves the camera. This is used to synchronize the camera position with the server.

---

### **28. Opcode 87: Drop Item**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when a player wants to drop an item onto the ground. This removes the item from the player's inventory.

---

### **29. Opcode 95: Privacy Options**
- **Type**: FIXED
- **Length**: 3 bytes
- **Description**: Sent when a player changes their privacy options (e.g., public chat, private chat, or trade settings).

---

### **30. Opcode 98: Walk on Command**
- **Type**: VARIABLE_BYTE
- **Length**: N/A
- **Description**: Sent when the player walks somewhere according to a certain action performed, such as clicking an object.

---

### **31. Opcode 101: Design Screen**
- **Type**: FIXED
- **Length**: 13 bytes
- **Description**: Sent when a player is choosing their character design options. This is used during character creation.

---

### **32. Opcode 103: Player Command**
- **Type**: VARIABLE_BYTE
- **Length**: N/A
- **Description**: Sent when the player enters a command in the chat box (e.g., "::command"). This is used for custom commands.

---

### **33. Opcode 117: Bank 5 Items**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when a player banks 5 of a certain item. This is used for quick banking actions.

---

### **34. Opcode 121: Loading Finished**
- **Type**: FIXED
- **Length**: 0 bytes
- **Description**: Sent when the client finishes loading a map region. This is used to synchronize the player's position with the server.

---

### **35. Opcode 122: Item Action 1**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when the player clicks the first option of an item (e.g., "Bury" for bones).

---

### **36. Opcode 126: Private Message**
- **Type**: VARIABLE_BYTE
- **Length**: N/A
- **Description**: Sent when a player sends a private message to another player. This is used for private communication.

---
Continuing with the **Client -> Server Packets**, here is the detailed breakdown of the remaining packets in order:

---

### **37. Opcode 128: Accept Challenge**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sent when a player accepts another player's duel request. This initiates a duel between the two players.

---

### **38. Opcode 129: Bank All Items**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when a player banks all of a certain item that they have in their inventory. This is used for quick banking actions.

---

### **39. Opcode 130: Close Window**
- **Type**: FIXED
- **Length**: 0 bytes
- **Description**: Sent when a player presses the close, exit, or cancel button on an interface. This closes the interface.

---

### **40. Opcode 131: Magic on NPC**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Sent when a player uses magic on an NPC. This is used for spells like Enchant or Teleport.

---

### **41. Opcode 132: Object Action 1**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when the player clicks the first option of an object (e.g., "Cut" for trees or "Open" for doors).

---

### **42. Opcode 133: Add Ignore**
- **Type**: FIXED
- **Length**: 8 bytes
- **Description**: Sent when a player adds a player to their ignore list. This prevents communication with the ignored player.

---

### **43. Opcode 135: Bank X Items Part-1**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when a player requests to bank an X amount of items. This is the first part of the banking process.

---

### **44. Opcode 136: Anti-Cheat (Player Option 1)**
- **Type**: FIXED
- **Length**: 0 bytes
- **Description**: Sent to validate player option 1. This is used to prevent cheating or botting.

---

### **45. Opcode 139: Trade Request**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sent when a player requests a trade from another player (e.g., "Sending Trade Request...").

---

### **46. Opcode 145: Unequip Item**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when a player unequips an item. This removes the item from the player's equipment interface.

---

### **47. Opcode 152: Anti-Cheat (NPC Option 3)**
- **Type**: FIXED
- **Length**: 1 byte
- **Description**: Sent to validate NPC option 3. This is used to prevent cheating or botting.

---

### **48. Opcode 153: Player Option 2 (Report Abuse)**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sent when a moderator or administrator selects the second option of a player (e.g., "Report Abuse").

---

### **49. Opcode 155: NPC Action 1**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sent when a player clicks the first option of an NPC (e.g., "Talk-to" or "Attack").

---

### **50. Opcode 164: Regular Walk**
- **Type**: VARIABLE_BYTE
- **Length**: N/A
- **Description**: Sent when the player walks regularly. This is used to synchronize the player's movement with the server.

---

### **51. Opcode 181: Magic on Ground Item**
- **Type**: FIXED
- **Length**: 8 bytes
- **Description**: Sent when a player uses a spell on a ground item. This is used for spells like High-Level Alchemy.

---

### **52. Opcode 183: Anti-Cheat (Object Option 4)**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Sent to validate clicking object option 4. This is used to prevent cheating or botting.

---

### **53. Opcode 185: Button Click**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sent when a player clicks an in-game button. This is used for interface interactions.

---

### **54. Opcode 188: Add Friend**
- **Type**: FIXED
- **Length**: 8 bytes
- **Description**: Sent when a player adds a friend to their friend list. This allows communication with the added friend.

---

### **55. Opcode 189: Anti-Cheat (Player Option 2)**
- **Type**: FIXED
- **Length**: 1 byte
- **Description**: Sent to validate player option 2. This is used to prevent cheating or botting.

---

### **56. Opcode 192: Item on Object**
- **Type**: FIXED
- **Length**: 12 bytes
- **Description**: Sent when a player uses an item on an object (e.g., using a knife on a log to fletch).

---

### **57. Opcode 200: Anti-Cheat (Banking Options)**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sent to validate banking options. This is used to prevent cheating or botting.

---

### **58. Opcode 202: Idle Logout**
- **Type**: FIXED
- **Length**: 0 bytes
- **Description**: Sent when the player has become idle and should be logged out. This is used to free up server resources.

---

### **59. Opcode 208: Bank X Items Part-2**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Sent when a player enters an X amount of items they want to bank. This is the second part of the banking process.

---

### **60. Opcode 210: Region Change**
- **Type**: FIXED
- **Length**: 0 bytes
- **Description**: Sent when a player enters a new map region. This is used to load the new region.

---

### **61. Opcode 214: Move Item**
- **Type**: FIXED
- **Length**: 7 bytes
- **Description**: Sent when a player moves an item from one slot to another in their inventory or bank.

---

### **62. Opcode 215: Remove Friend**
- **Type**: FIXED
- **Length**: 8 bytes
- **Description**: Sent when a player removes a friend from their friend list. This prevents communication with the removed friend.

---

### **63. Opcode 218: Report Player**
- **Type**: FIXED
- **Length**: 8 bytes
- **Description**: Sent when a player reports another player. This is used for moderation purposes.

---

### **64. Opcode 228: Object Option 4**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when a player uses the 4th option of an object (e.g., "Examine" or "Use").

---

### **65. Opcode 230: Anti-Cheat (NPC Option 2)**
- **Type**: FIXED
- **Length**: 1 byte
- **Description**: Sent to validate NPC option 2. This is used to prevent cheating or botting.

---

### **66. Opcode 234: Object Option 2**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when a player uses the 2nd option of an object (e.g., "Chop" for trees or "Mine" for rocks).

---

### **67. Opcode 236: Pickup Ground Item**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when the player picks up an item from the ground. This adds the item to the player's inventory.

---

### **68. Opcode 237: Magic on Items**
- **Type**: FIXED
- **Length**: 8 bytes
- **Description**: Sent when a player casts magic on the items in their inventory (e.g., High-Level Alchemy).

---

### **69. Opcode 241: Mouse Click**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Sent when the player clicks somewhere on the game screen. This is used for general interactions.

---

### **70. Opcode 246: Anti-Cheat**
- **Type**: FIXED
- **Length**: 15 bytes
- **Description**: Likely related to anti-cheat measures. The exact functionality is unknown.

---

### **71. Opcode 248: Map Walk**
- **Type**: VARIABLE_BYTE
- **Length**: N/A
- **Description**: Sent when the player walks using the map. This includes additional anti-cheat bytes.

---

### **72. Opcode 249: Magic on Player**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Sent when a player attempts to cast magic on another player (e.g., Teleport or Heal).

---

### **73. Opcode 252: Object Action 2**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when the player clicks the second option available for an object (e.g., "Climb" or "Search").

---

### **74. Opcode 253: Ground Item Action**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sent when the player clicks the first option for a ground item (e.g., "Take" or "Light Logs").

---

This completes the **Client -> Server Packets**.
