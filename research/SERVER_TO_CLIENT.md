**Server -> Client Packets**

---

## **Server -> Client Packets**

### **1. Opcode 1: Animation Reset**
- **Type**: FIXED
- **Length**: 0 bytes
- **Description**: Resets all animations in the immediate area. This is often used to clear lingering animations after an event or action.

---

### **2. Opcode 4: Display Stationary Animation**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Displays a stationary animation at a specific location. For example, this could be used to show a spell effect or an emote.

---

### **3. Opcode 24: Flash Sidebar**
- **Type**: FIXED
- **Length**: 1 byte
- **Description**: Causes a sidebar icon to start flashing. This is often used to alert the player of a new notification or event.

---

### **4. Opcode 34: Update Single Item**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Updates a single item in the player’s inventory. This could involve changing the item’s quantity, appearance, or state.

---

### **5. Opcode 35: Camera Shake**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Causes the player’s camera to shake. This is often used for dramatic effects, such as earthquakes or explosions.

---

### **6. Opcode 36: Send Config**
- **Type**: FIXED
- **Length**: 3 bytes
- **Description**: Sends a configuration to the client. For example, this could be used to set rules for a duel interface.

---

### **7. Opcode 44: Display Ground Item**
- **Type**: FIXED
- **Length**: 5 bytes
- **Description**: Displays an item on the ground at a specified coordinate. This is used to show items that players can pick up.

---

### **8. Opcode 50: Send Add Friend**
- **Type**: FIXED
- **Length**: 9 bytes
- **Description**: Adds a friend to the player’s friend list. This packet sends the friend’s details to the client.

---

### **9. Opcode 53: Set Stack Size**
- **Type**: VARIABLE_SHORT
- **Length**: N/A
- **Description**: Sets the stack size of an item on the inventory interface. This is used for items that can be stacked, such as coins or runes.

---

### **10. Opcode 60: Send Regional Packet**
- **Type**: FIXED
- **Length**: 3 bytes
- **Description**: Sends a regional packet, which is used for updates within a specific region of the game world.

---

### **11. Opcode 64: Remove Ground Item**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Removes a ground item from the game world. This is used when an item is picked up or disappears.

---

### **12. Opcode 65: NPC Updating**
- **Type**: VARIABLE_SHORT
- **Length**: N/A
- **Description**: Updates NPCs in the area, including their movements, actions, and appearance.

---

### **13. Opcode 68: Reset Button State**
- **Type**: FIXED
- **Length**: 0 bytes
- **Description**: Resets the state of all buttons in the game. This is often used to clear any toggled or pressed buttons.

---

### **14. Opcode 70: Interface Offset**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sets the offset for drawing an interface. This is used to position interfaces on the screen.

---

### **15. Opcode 71: Send Sidebar Interface**
- **Type**: FIXED
- **Length**: 3 bytes
- **Description**: Assigns an interface to one of the tabs in the game sidebar. For example, this could set the inventory tab to display the player’s inventory.

---

### **16. Opcode 72: Clear Inventory**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Clears an interface’s inventory. This is used to remove all items from an interface, such as a shop or bank.

---

### **17. Opcode 73: Load Map Region**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Loads a new map region as the player moves. This is used to dynamically load areas of the game world.

---

### **18. Opcode 74: Send Song**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Plays a background song. This is used to set the music for a specific area or event.

---

### **19. Opcode 78: Clear Minimap Flag**
- **Type**: FIXED
- **Length**: 0 bytes
- **Description**: Clears the minimap flag from the minimap. This is used to remove markers or indicators from the minimap.

---

### **20. Opcode 79: Scroll Position**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Sets the scrollbar position of an interface. This is used to control the position of scrollable interfaces.

---

### **21. Opcode 81: Player Updating**
- **Type**: VARIABLE_SHORT
- **Length**: N/A
- **Description**: Updates the local player’s appearance, position, or actions. This is used to synchronize the player’s state with the server.

---

### **22. Opcode 84: UNKNOWN (Ground Items)**
- **Type**: FIXED
- **Length**: 7 bytes
- **Description**: Likely related to updating the amount of a ground item. The exact functionality is unknown.

---

### **23. Opcode 85: Update Local Player**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Updates the player’s localX and localY coordinates. This is used to synchronize the player’s position with the server.

---

### **24. Opcode 87: Toggle Interface Button**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Toggles an interface button. This can have multiple states, such as in the dueling interface.

---

### **25. Opcode 97: Show Interface**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Displays a normal interface, such as a shop or bank.

---
Continuing with the **Server -> Client Packets**, here are the next set of packets in order:

---

### **26. Opcode 99: Minimap State**
- **Type**: FIXED
- **Length**: 1 byte
- **Description**: Sets the mini map's state. This could involve enabling or disabling certain features of the minimap.

---

### **27. Opcode 101: Remove Object**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Removes a regional object from the game world. This is used when an object is destroyed or no longer needed.

---

### **28. Opcode 104: Display Player Option**
- **Type**: VARIABLE_BYTE
- **Length**: N/A
- **Description**: Displays a player right-click option. This is used to add custom options to the right-click menu for players.

---

### **29. Opcode 105: Play Sound in Location**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Plays a sound effect in a specific location. This is used to add ambient or event-specific sounds.

---

### **30. Opcode 106: Force Tab**
- **Type**: FIXED
- **Length**: 1 byte
- **Description**: Force sets a player's current sidebar interface. This overrides the player's current tab.

---

### **31. Opcode 107: Reset Camera**
- **Type**: FIXED
- **Length**: 0 bytes
- **Description**: Resets the camera position to its default state. This is often used after a cinematic or special camera movement.

---

### **32. Opcode 109: Logout**
- **Type**: FIXED
- **Length**: 0 bytes
- **Description**: Disconnects the client from the server. This is used when the player logs out or is forcibly disconnected.

---

### **33. Opcode 110: Run Energy**
- **Type**: FIXED
- **Length**: 1 byte
- **Description**: Sends the player's run energy level. This updates the run energy bar on the client.

---

### **34. Opcode 114: System Update**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sends a countdown until a system update (e.g., server maintenance). This is displayed as a warning to players.

---

### **35. Opcode 117: Display Projectile**
- **Type**: FIXED
- **Length**: 15 bytes
- **Description**: Displays a projectile, such as an arrow or spell, flying from one location to another.

---

### **36. Opcode 121: Queue Song**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Queues a song to be played next. This is used to transition between background music tracks.

---

### **37. Opcode 122: Interface Color**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Changes the color of an interface. This is used to dynamically update interface appearances.

---

### **38. Opcode 126: Send Text**
- **Type**: VARIABLE_SHORT
- **Length**: N/A
- **Description**: Attaches text to an interface. This is used to display dynamic text, such as item names or descriptions.

---

### **39. Opcode 134: Update Skill**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Updates a player's skill level and experience. This is used to synchronize skill progress with the client.

---

### **40. Opcode 135: Skill Level**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Sends a skill level to the client. This is used to display the player's current level in a specific skill.

---

### **41. Opcode 147: Transform Player Into Game Object**
- **Type**: FIXED
- **Length**: 10 bytes
- **Description**: Transforms a player into a game object. This is often used for special events or animations.

---

### **42. Opcode 151: Add Object**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Adds a regional object to the game world. This is used to spawn objects dynamically.

---

### **43. Opcode 156: Remove Ground Item**
- **Type**: FIXED
- **Length**: 3 bytes
- **Description**: Removes an item on the ground. This is used when an item is picked up or disappears.

---

### **44. Opcode 160: Animate Object**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Animates a game object. This is used to add movement or effects to objects.

---

### **45. Opcode 164: Chat Interface**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Shows an interface in the chat box. This is used to display interfaces alongside chat messages.

---

### **46. Opcode 166: Spin Camera**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Spins the player's camera to a specific angle. This is used for cinematic effects.

---

### **47. Opcode 171: Send Hidden Interface**
- **Type**: FIXED
- **Length**: 3 bytes
- **Description**: Sets an interface to be hidden until hovered over. This is used for tooltips or hidden menus.

---

### **48. Opcode 174: Send Sound**
- **Type**: FIXED
- **Length**: 5 bytes
- **Description**: Plays a sound effect. This is used for various in-game sounds, such as spells or item interactions.

---

### **49. Opcode 176: Open Welcome Screen**
- **Type**: FIXED
- **Length**: 10 bytes
- **Description**: Displays the welcome screen. This is often shown when a player logs in.

---

### **50. Opcode 177: Gradually Turn Camera**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Gradually turns the camera to a specified location. This is used for smooth camera transitions.

---

### **51. Opcode 185: Display Player Head Model on Interface**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Displays a player's head model on an interface. This is often used for customization or identification.

---

### **52. Opcode 196: Send Private Message**
- **Type**: VARIABLE_BYTE
- **Length**: N/A
- **Description**: Sends a private message to another player. This is used for player-to-player communication.

---

### **53. Opcode 200: Interface Animation**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Sets an interface's model animation. This is used to animate interface elements.

---

### **54. Opcode 206: Chat Settings**
- **Type**: FIXED
- **Length**: 3 bytes
- **Description**: Sends the chat privacy settings. This is used to configure who can send messages to the player.

---

### **55. Opcode 208: Walkable Interface**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Displays an interface in walkable mode. This allows the player to walk while the interface is open.

---

### **56. Opcode 214: Send Add Ignore**
- **Type**: VARIABLE_SHORT
- **Length**: N/A
- **Description**: Adds a player to the ignore list. This prevents the player from receiving messages from the ignored player.

---

### **57. Opcode 215: UNKNOWN (Ground Items)**
- **Type**: FIXED
- **Length**: 7 bytes
- **Description**: Likely related to ground items. The exact functionality is unknown.

---

### **58. Opcode 219: Clear Screen**
- **Type**: FIXED
- **Length**: 0 bytes
- **Description**: Clears the screen of all open interfaces. This is used to reset the player's view.

---

### **59. Opcode 221: Friends List Status**
- **Type**: FIXED
- **Length**: 1 byte
- **Description**: Indicates the friends list load status. This is used to synchronize the friends list with the server.

---

### **60. Opcode 230: Interface Model Rotation**
- **Type**: FIXED
- **Length**: 8 bytes
- **Description**: Sets an interface's model rotation and zoom. This is used to adjust the appearance of interface models.

---

### **61. Opcode 240: Weight**
- **Type**: FIXED
- **Length**: 2 bytes
- **Description**: Sends the player's weight amount. This updates the weight indicator on the client.

---

### **62. Opcode 241: Construct Map Region**
- **Type**: VARIABLE_SHORT
- **Length**: N/A
- **Description**: Constructs a dynamic map region using a palette of 8x8 tiles. This is used to load custom map areas.

---

### **63. Opcode 246: Interface Item**
- **Type**: FIXED
- **Length**: 6 bytes
- **Description**: Displays an item model inside an interface. This is used to show items in interfaces like banks or shops.

---

### **64. Opcode 248: Inventory Overlay**
- **Type**: FIXED
- **Length**: 4 bytes
- **Description**: Displays an interface over the sidebar area. This is used for overlays like the equipment stats interface.

---

### **65. Opcode 249: Initialize Player**
- **Type**: FIXED
- **Length**: 3 bytes
- **Description**: Sends the player's membership status and their current index on the server's player list. This is used during login.

---

### **66. Opcode 253: Send Message**
- **Type**: VARIABLE_BYTE
- **Length**: N/A
- **Description**: Sends a server message (e.g., "Welcome to RuneScape") or trade/duel request. This is used for system notifications.

---

### **67. Opcode 254: Display Mob Hint Icon**
- **Type**: FIXED
- **Length**: 3 bytes
- **Description**: Displays a hint icon over a mob. This is often used for quest-related NPCs.

---

This completes the **Server -> Client Packets**.

