# Changelog - Developers

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

##### This change log is only really useful to the developers who use the SnowballAPI to create plugins. If you are a user, please check [[here]]() for the user change log.

## [[1.0.0]](https://github.com/SnowballClient/Installer/raw/master/%23%20Releases/Snowball%20v1.0.0%20Installer.jar) - 12/11/2018
### Added
- CustomBlock Class - This class represents a block that is added to the game
- CustomItem Class - This class represents a item that is added to the game
- SnowballPlayerKeypressEvent - This event is fired when ever a person pushes a key on there keyboard. This only works when the user has Minecraft selected, for obvious reasons
- CustomEnchantment Class - This class represents a enchantment that is added to the game
- EnumCosmetic Class - Cosmetics like a TopHat, to wings etc
- SnowballAPI Class - The Main API for the SnowballClient
  - void addBlock(CustomBlock block)
  - void addItem(CustomItem item)
  - void addEnchantment(CustomEnchantment ench)
  - SnowballPlayer getSnowballPlayer(Player player)
- SnowballPlayer class - This class allows you to manipulate anything you want about the player
  - void getBukkitPlayer() - Returns the bukkit player
  - boolean hasCustomSkin() - Does this player have a custom skin?
  - void sendToast(String title, String desc) - Send them a toast with no Icon
  - void sendToast(String title, String desc, ItemStack icon) - Send them a toast with a icon
  - void removeCustomSkin() - Removes the players custom skin
  - void setCustomSkin(String skinUrl) - Add a custom skin to the player. Keep in mind that this needs to be a 1.12.2 skin. If the picture is not a skin, some intresting things will start to happen.
  - void resetCustomUsername() - Removes the users custom username
  - void setCustomUsername(String name) - Sets the tablist and nametag. Color codes do not work by default but you can use ChatColor.translateAlternateColorCodes or ChatColor.COLOR for coloring the nametag.
  - void addCosmetic(EnumCosmetic... cosmeticIn) - Adds a cosmetic to the player
  - void removeCosmetic(EnumCosmetic... cosmeticIn) - Removes a cosmetic from the player

### Changed
- Nothing so far

### Removed
- Nothing so far
