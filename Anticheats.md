#Project Zomboid Official AntiCheats
Name | Description | Parameters
--- | --- | ---
AntiCheatProtectionType1 | checkPVP(), if player hit a "protected" victims (not in PVP Zone, Safehouse etc..) | true/false
AntiCheatProtectionType2 | checkSpeed(), speedhack anticheat (vehicle = speedlimit set in server options. players, limit is 10) | true/false (Threshold Multiplier min: 1, max; 10, default: 3)
AntiCheatProtectionType3 | checkLongDistance()/checkShortDistance(), check if player hit a target from too close or too far | true/false (Threshold Multiplier min: 1, max; 10, default: 1)
AntiCheatProtectionType4 | checkDamage(), check if player do to much damage (damage max: 101.0 * Threshold Multiplier) | true/false (Threshold Multiplier min: 1, max; 10, default: 1)
AntiCheatProtectionType5 | checkOwner(), check "owner" of Zombie to prevent packet spoofing (each client send to server only Z owned by himself) | true/false
AntiCheatProtectionType6 | checkTarget(), check if Zombie target is not spoofed (each client send to server hiw own Z targetting his character) | true/false
AntiCheatProtectionType7 | checkSafehouseAuth(), check if player in safehouse have proper authorisation or access | true/false
AntiCheatProtectionType8 | PacketAuthorization, check if player send a valid packet based on his access level (prevent access to serverside informations, stats etc..) | true/false
AntiCheatProtectionType9 | Check XP Growth Rate (> 1000.0 * * Threshold Multiplier) | true/false (Threshold Multiplier min: 1, max; 10, default: 1)
AntiCheatProtectionType10 | Check if packet sended by client is valid or unknow | true/False
AntiCheatProtectionType11 | *unused* | true/false
AntiCheatProtectionType12 | Check player access level to prevent debug access | true/false
AntiCheatProtectionType13 | Check if packet type sended by client is valid | true/false
AntiCheatProtectionType14 | Check if player give xp to another player without proper access-level | true/false
AntiCheatProtectionType15 | Check AddXP limit, if a player try to add too much xp in a single time (> 1000.0 * * Threshold Multiplier) | true/false (Threshold Multiplier min: 1, max; 10, default: 1)
AntiCheatProtectionType16 | Check if player send a packet to start a fire when fire is disabled, prevent packet spoofing | true/false
AntiCheatProtectionType17 | Check if player send a packet to ignite a tile nonflammable (set in tile definition) | true/false 
AntiCheatProtectionType18 | Check if player send a packet to ignite a tile who can't have smoke on it (set in tile definition) | true/false 
AntiCheatProtectionType19 | Check if packet related to create safehouse sended by client is valid and player have safehouse | true/false
AntiCheatProtectionType20 | Check if player have right access-level to create a safehouse, also check if safehouse created is bigger than Threshold | true/false (Threshold Multiplier min: 1, max; 10, default: 1) 
AntiCheatProtectionType21 | failChecksum(), check if packet checksum is valid or not (not related to files/mods checksum)| true/false
AntiCheatProtectionType22 | Check if client answer to packet checksum control in time | true/false
AntiCheatProtectionType23 | Check if Client use same Time as Server (prevent Clientside time control) | true/false
AntiCheatProtectionType24 | Check if client answer to packet Time control in time | true/false

#Note that a lot of controls are client side, and can be bypassed easily
