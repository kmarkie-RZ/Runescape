## **Server -> Client Packets **

| **Opcode** | **Name**                          | **Description**                                                                 |
|------------|-----------------------------------|---------------------------------------------------------------------------------|
| 1          | Animation Reset                  | Resets all animations in the area.                                              |
| 4          | Display Stationary Animation     | Shows a stationary animation.                                                   |
| 24         | Flash Sidebar                    | Flashes a sidebar icon.                                                         |
| 34         | Update Single Item               | Updates a single item in the inventory.                                         |
| 35         | Camera Shake                     | Shakes the player's camera.                                                     |
| 36         | Send Config                      | Sends configuration settings (e.g., duel rules).                                |
| 44         | Display Ground Item              | Displays an item on the ground.                                                 |
| 50         | Send Add Friend                  | Adds a friend to the friend list.                                               |
| 53         | Set Stack Size                   | Sets the stack size of an item.                                                 |
| 60         | Send Regional Packet             | Sends a regional update.                                                        |
| 64         | Remove Ground Item               | Removes an item from the ground.                                                |
| 65         | NPC Updating                     | Updates NPCs in the area.                                                       |
| 68         | Reset Button State               | Resets all button states.                                                       |
| 70         | Interface Offset                 | Sets the offset for drawing an interface.                                       |
| 71         | Send Sidebar Interface           | Assigns an interface to a sidebar tab.                                          |
| 72         | Clear Inventory                  | Clears an interface's inventory.                                                |
| 73         | Load Map Region                  | Loads a new map region.                                                         |
| 74         | Send Song                        | Plays a background song.                                                        |
| 78         | Clear Minimap Flag               | Clears the minimap flag.                                                        |
| 79         | Scroll Position                  | Sets the scrollbar position of an interface.                                    |
| 81         | Player Updating                  | Updates the local player.                                                       |
| 84         | Update Ground Item Amount        | Updates the amount of a ground item.                                            |
| 85         | Update Local Player              | Updates the player's local coordinates.                                         |
| 87         | Toggle Interface Button          | Toggles an interface button.                                                    |
| 97         | Show Interface                   | Displays a normal interface.                                                    |
| 99         | Minimap State                    | Sets the minimap's state.                                                       |
| 101        | Remove Object                    | Removes a regional object.                                                      |
| 104        | Display Player Option            | Displays a player right-click option.                                           |
| 105        | Play Sound in Location           | Plays a sound effect at a location.                                             |
| 106        | Force Tab                        | Forces a sidebar interface.                                                     |
| 107        | Reset Camera                     | Resets the camera position.                                                     |
| 109        | Logout                           | Disconnects the client.                                                         |
| 110        | Run Energy                       | Sends the player's run energy level.                                            |
| 114        | System Update                    | Sends a system update countdown.                                                |
| 117        | Display Projectile               | Displays a projectile.                                                          |
| 121        | Queue Song                       | Queues a song to play next.                                                     |
| 122        | Interface Color                  | Changes the color of an interface.                                              |
| 126        | Send Text                        | Attaches text to an interface.                                                  |
| 134        | Update Skill                     | Updates a player's skill level and experience.                                  |
| 135        | Skill Level                      | Sends a skill level to the client.                                              |
| 147        | Transform Player Into Game Object| Transforms a player into a game object.                                         |
| 151        | Add Object                       | Adds a regional object to the game world.                                       |
| 156        | Remove Ground Item               | Removes an item on the ground.                                                  |
| 160        | Animate Object                   | Animates a game object.                                                         |
| 164        | Chat Interface                   | Shows an interface in the chat box.                                             |
| 166        | Spin Camera                      | Spins the player's camera.                                                      |
| 171        | Send Hidden Interface            | Hides an interface until hovered over.                                          |
| 174        | Send Sound                       | Plays a sound effect.                                                           |
| 176        | Open Welcome Screen              | Displays the welcome screen.                                                    |
| 177        | Gradually Turn Camera            | Gradually turns the camera to a location.                                       |
| 185        | Display Player Head Model        | Displays a player's head model on an interface.                                 |
| 196        | Send Private Message             | Sends a private message to another player.                                      |
| 200        | Interface Animation              | Sets an interface's model animation.                                            |
| 206        | Chat Settings                    | Sends chat privacy settings.                                                    |
| 208        | Walkable Interface               | Displays an interface in walkable mode.                                         |
| 214        | Send Add Ignore                  | Adds a player to the ignore list.                                               |
| 215        | UNKNOWN (Ground Items)           | Likely related to ground items.                                                 |
| 219        | Clear Screen                     | Clears the screen of all interfaces.                                            |
| 221        | Friends List Status              | Indicates the friends list load status.                                         |
| 230        | Interface Model Rotation         | Sets an interface's model rotation and zoom.                                    |
| 240        | Weight                           | Sends the player's weight amount.                                               |
| 241        | Construct Map Region             | Constructs a dynamic map region.                                                |
| 246        | Interface Item                   | Displays an item model inside an interface.                                     |
| 248        | Inventory Overlay                | Displays an interface over the sidebar area.                                    |
| 249        | Initialize Player                | Sends the player's membership status and server index.                          |
| 253        | Send Message                     | Sends a server message or trade/duel request.                                   |
| 254        | Display Mob Hint Icon            | Displays a hint icon over a mob.                                                |

---

## **Client -> Server Packets **

| **Opcode** | **Name**                          | **Description**                                                                 |
|------------|-----------------------------------|---------------------------------------------------------------------------------|
| 0          | Idle                              | Sent when no actions are performed.                                             |
| 3          | Focus Change                      | Sent when the game window gains or loses focus.                                 |
| 4          | Chat                              | Sent when the player enters a chat message.                                     |
| 14         | Item on Player                    | Sent when a player uses an item on another player.                              |
| 16         | Alternate Item Option 2           | Sent when a player uses an item (alternate option).                             |
| 17         | NPC Action 2                      | Sent when a player clicks the second option of an NPC.                          |
| 18         | NPC Action 4                      | Sent when a player clicks the fourth option of an NPC.                          |
| 21         | NPC Action 3                      | Sent when a player clicks the third option of an NPC.                           |
| 25         | Item on Floor                     | Sent when a player uses an item on another item on the floor.                   |
| 35         | Magic on Object                   | Sent when a player uses magic on an object.                                     |
| 36         | Anti-Cheat (Walking)              | Validates walking actions.                                                      |
| 39         | Follow                            | Sent when a player follows another player.                                      |
| 40         | Dialogue                          | Sent when a player continues a dialogue.                                        |
| 41         | Equip Item                        | Sent when a player equips an item.                                              |
| 43         | Bank 10 Items                     | Sent when a player banks 10 of a certain item.                                  |
| 45         | Flagged Account                   | Sent when a player's account is flagged.                                        |
| 53         | Item on Item                      | Sent when a player uses an item with another item.                              |
| 57         | Item on NPC                       | Sent when a player uses an item on an NPC.                                      |
| 60         | Typing onto Interface             | Sent while typing into an interface.                                            |
| 70         | Object Action 3                   | Sent when the player clicks the third option of an object.                      |
| 72         | Attack (NPC)                      | Sent when a player attacks an NPC.                                              |
| 73         | Attack (Player)                   | Sent when a player attacks another player.                                      |
| 74         | Remove Ignore                     | Sent when a player removes a player from their ignore list.                     |
| 75         | Item Action 3                     | Sent when a player clicks the third option of an item.                          |
| 79         | Light Item                        | Sent when a player attempts to light logs on fire.                              |
| 85         | Anti-Cheat (NPC Option 4)         | Validates NPC option 4.                                                         |
| 86         | Camera Movement                   | Sent when the player moves the camera.                                          |
| 87         | Drop Item                         | Sent when a player drops an item.                                               |
| 95         | Privacy Options                   | Sent when a player changes their privacy settings.                              |
| 98         | Walk on Command                   | Sent when the player walks according to an action.                              |
| 101        | Design Screen                     | Sent during character creation.                                                 |
| 103        | Player Command                    | Sent when the player enters a command (e.g., "::command").                      |
| 117        | Bank 5 Items                      | Sent when a player banks 5 of a certain item.                                   |
| 121        | Loading Finished                  | Sent when the client finishes loading a map region.                             |
| 122        | Item Action 1                     | Sent when the player clicks the first option of an item.                        |
| 126        | Private Message                   | Sent when a player sends a private message.                                     |
| 128        | Accept Challenge                  | Sent when a player accepts a duel request.                                      |
| 129        | Bank All Items                    | Sent when a player banks all of a certain item.                                 |
| 130        | Close Window                      | Sent when a player closes an interface.                                         |
| 131        | Magic on NPC                      | Sent when a player uses magic on an NPC.                                        |
| 132        | Object Action 1                   | Sent when the player clicks the first option of an object.                      |
| 133        | Add Ignore                        | Sent when a player adds a player to their ignore list.                          |
| 135        | Bank X Items Part-1               | Sent when a player requests to bank an X amount of items.                       |
| 136        | Anti-Cheat (Player Option 1)      | Validates player option 1.                                                      |
| 139        | Trade Request                     | Sent when a player requests a trade.                                            |
| 145        | Unequip Item                      | Sent when a player unequips an item.                                            |
| 152        | Anti-Cheat (NPC Option 3)         | Validates NPC option 3.                                                         |
| 153        | Player Option 2 (Report Abuse)    | Sent when a moderator reports abuse.                                            |
| 155        | NPC Action 1                      | Sent when a player clicks the first option of an NPC.                           |
| 164        | Regular Walk                      | Sent when the player walks regularly.                                           |
| 181        | Magic on Ground Item              | Sent when a player uses magic on a ground item.                                 |
| 183        | Anti-Cheat (Object Option 4)      | Validates object option 4.                                                      |
| 185        | Button Click                      | Sent when a player clicks an in-game button.                                    |
| 188        | Add Friend                        | Sent when a player adds a friend.                                               |
| 189        | Anti-Cheat (Player Option 2)      | Validates player option 2.                                                      |
| 192        | Item on Object                    | Sent when a player uses an item on an object.                                   |
| 200        | Anti-Cheat (Banking Options)      | Validates banking options.                                                      |
| 202        | Idle Logout                       | Sent when the player is idle and should be logged out.                          |
| 208        | Bank X Items Part-2               | Sent when a player enters an X amount of items to bank.                         |
| 210        | Region Change                     | Sent when a player enters a new map region.                                     |
| 214        | Move Item                         | Sent when a player moves an item in their inventory or bank.                   |
| 215        | Remove Friend                     | Sent when a player removes a friend.                                           |
| 218        | Report Player                     | Sent when a player reports another player.                                      |
| 228        | Object Option 4                   | Sent when a player uses the 4th option of an object.                            |
| 230        | Anti-Cheat (NPC Option 2)         | Validates NPC option 2.                                                         |
| 234        | Object Option 2                   | Sent when a player uses the 2nd option of an object.                            |
| 236        | Pickup Ground Item                | Sent when a player picks up an item from the ground.                            |
| 237        | Magic on Items                    | Sent when a player casts magic on items in their inventory.                     |
| 241        | Mouse Click                       | Sent when the player clicks somewhere on the screen.                            |
| 246        | Anti-Cheat                        | Likely related to anti-cheat measures.                                          |
| 248        | Map Walk                          | Sent when the player walks using the map.                                       |
| 249        | Magic on Player                   | Sent when a player casts magic on another player.                               |
| 252        | Object Action 2                   | Sent when the player clicks the second option of an object.                     |
| 253        | Ground Item Action                | Sent when the player clicks the first option for a ground item.                 |

---
