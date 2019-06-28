# Hotbar Swapper

This mod lets you set up multiple hotbar loadouts and swap between them with a simple shortcut! This is super useful if you like to build a lot, but also want to carry around a lot of tools and get tired of opening your inventory to move things around on your hotbar all the time. For instance, you could be in the middle of building a base with a full hotbar of structures when you suddenly get attacked. Normally this would be a problem, but not with Hotbar Swapper! Just swap to your weapons loadout, and you are ready to defend yourself!

## Setting up your keyboard shortcuts

This mod lets you configure your own keyboard shortcuts, because nobody likes being locked in to what the modder decided, right? **Your shortcuts will need to be set up before using the mod**, but this is really easy to do:

1. Find your Input.ini file, located by default at:
```
C:\Program Files (x86)\Steam\steamapps\common\ARK\ShooterGame\Saved\Config\WindowsNoEditor\Input.ini
```

2. Paste the following four lines at the bottom of the file, under the other `ActionMappings` lines (in the `[/Script/Engine.InputSettings]` section):
```
ActionMappings=(ActionName="HotbarSwapper_NewLoadout",Key=N,bShift=False,bCtrl=True,bAlt=False,bCmd=False)
ActionMappings=(ActionName="HotbarSwapper_DeleteLoadout",Key=X,bShift=False,bCtrl=True,bAlt=False,bCmd=False)
ActionMappings=(ActionName="HotbarSwapper_NextLoadout",Key=MouseScrollDown,bShift=False,bCtrl=True,bAlt=False,bCmd=False)
ActionMappings=(ActionName="HotbarSwapper_PreviousLoadout",Key=MouseScrollUp,bShift=False,bCtrl=True,bAlt=False,bCmd=False)
```

Modify these shortcuts to whatever you'd like, or leave them as-is!

## Creating a new loadout

To create a new hotbar loadout, use the `HotbarSwapper_NewLoadout` shortcut. Your hotbar will be cleared and ready for you to add items!

To switch to the previous loadout, use the `HotbarSwapper_PreviousLoadout` shortcut. To switch to the next loadout, use the `HotbarSwapper_NextLoadout` shortcut.

To delete a loadout, use the `HotbarSwapper_DeleteLoadout` shortcut.

That's it!

## Known issues

- If you have a loadout that contains consumable items and you eat or use them all after adding them to the loadout _before_ you have switched to another loadout and back, those items won't save their spots on the hotbar when you switch back. If you add them to the hotbar and switch loadouts and come back, then you can safely eat or use all of the items and switch loadouts and there will still be placeholders for them when you switch back.

**tl;dr: It's a good idea to swap loadouts at least once after adding items before using them if they are consumable (e.g. food and structures)!**

- Occasionally items might appear on hotbars they were not saved on. I'm still tracking down this issue which is likely a minor network replication issue.

- In single player, a message about items being added to your inventory will show when switching to a loadout that has consumable/structure items that have already all been used.

## Future plans

This mod is meant to be pretty simple, but I'm considering ways to expand it, possibly with multiple visible hotbars if possible. I'd also like to add keyboard shortcuts to activate items on various loadouts without having to switch to them first.

If you have questions or suggestions, please leave them in the comments! Please note that due to the often overwhelming nature of Steam comments, I won't be likely to answer questions that are not directly related to this mod (such as server management questions, like installation and updating, etc...).