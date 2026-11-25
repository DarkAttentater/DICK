# DICK - Dark's Icon & Category Kit: changelog

Versioning: MAJOR.MINOR.PATCH. 0.9.x = test builds before the first public release; each tested change set gets a new patch number
and its own zip in `releases\` (older zips are kept for rollback; on 2026-11-09 the 0.9.3 to 0.9.12 zips were moved to `releases\_archive` and the numbering restarted at 0.9.3). 1.0.0 is the first build that passes the in-game checklist with
AIT, THICC and BOOBIES removed and the borrowed icons replaced. Add one entry per build, newest first.

## 0.12.0

Everything from the 0.11.1 and 0.12.0 test builds (the betas below) in one release:

- Extra columns for the crafting menus: Forge and Grindstone (weapon stats), Forge and Workbench (armor stats), Smelter and Tanning Rack (FROM: what an item is broken down into), Enchanting Table (damage and armor on the Item tab, Effect on the Disenchant tab, soul size on the Soul Gem tab), Alchemy Lab (known effects, Green Pact) and Cooking Pot and Oven (CC Survival and SunHelm food columns).
- Active Effects Type column in the Magic menu (on by default; every other extra column is off by default).
- Reverse sorting: the arrow up of a column uses your sort order, the arrow down uses the same rules each reversed.
- Soul Gem sorting by gem size and soul size.
- Enchantment icons on the Enchanting Table (work in progress, off by default).
- MCM: every Columns and Sorting page starts with an Info section with its reset switch; the Icons page holds the weapon, Active Effects and Enchantment icon settings; System Settings starts with the DICK version; related sections are grouped, headers and labels are Title Case.
- FOMOD installer: the survival mods are check boxes (ticked when the mod is active). The Skyrim SE 1.5.97 DLL is included again.
- Plugin version 0.12.0.

## 0.12.0-beta7 (test build)

- MCM: every Columns and Sorting page starts with an Info section named after the page (for example "Inventory Sorting Info"), with a short line (full text in the description box) and the reset switch at the end of the section. The old "Extra Columns Added by DICK" and "Reset to Defaults" sections are gone.
- Inventory Sorting and Magic Sorting: the sections are spread over both panels to remove the large blank space.

## 0.12.0-beta6 (test build)

- Magic Sorting: the section headers are now Magic Menu: Spells, Powers, Shouts and Active Effects, like the Magic Columns page, and the sections are spread over both panels (no more empty right panel).
- Icons page: the first section is headed "Icons Info" (the game shows a header called just "Info" in lower case), and the switch is now called "Active Effects Icons".

## 0.12.0-beta5 (test build)

- Magic Sorting: the Active Effects section is now headed "Active Effects List". A header that matches an in-game menu heading exactly is shown in capitals by the game; the new text does not match.

## 0.12.0-beta4 (test build)

- Capitalization: options and column labels are Title Case too (as the section headers already are), for example "Base Damage Column", "Sort Order", "Equipped Items First".

## 0.12.0-beta3 (test build)

- Icons page: new Info section (with Reset this page). The Magic Effects page is merged into it: "Icons in Active Effects" is now an on / off switch, and "Icon type" (Source icons or Effect icons) and "Copy type and keywords" are only available while it is on. New "Enchantment Icons" section with a switch "Enchantment icons (work in progress)", off by default.
- Settings: bActiveEffectIcons and iActiveEffectIconType replace iActiveEffectIcons; bEnchantIcons is new (default off).
- System Settings: the About section is first (top left) and starts with the DICK version; both reset switches are in it. The log and settings notes show their text in the description box at the bottom.
- Capitalization: section headers are Title Case, options and column labels sentence case.

## 0.12.0-beta2 (test build)

- Enchanting Table, Enchantment tab (work in progress): DICK works out an icon label for each enchantment from its first effect (fire/frost/shock damage, absorb, paralyze, soul trap, resistances, skills, fortify and regen of health/magicka/stamina, and more) and writes it on the row. New icon rules file 22_Dark-Enchant-Effects.json turns the labels into icons. Some effects share a placeholder icon until their own is drawn (damage by element, soul trap, banish, fear). The log lists the first 12 enchantment rows with their label.

## 0.12.0-beta1 (test build)

- Version bumped to the 0.12.0 line.
- MCM pages: the sections of the Inventory and Magic pages may now go in either panel, so the two panels are as even as possible (Food and Ingredients on the left, Weapons and Armor on the right on the Inventory Columns page). The Info section stays on the left.

## 0.11.1-beta31 (test build)

- MCM pages: sections that belong together are grouped with no empty line between them and always stay in the same panel: smithing (Weapons, Armor, Smelter & Tanning Rack, Other Crafting), enchanting (Disenchanting, Items, Soul Gems, Enchanting Table), alchemy and cooking, and on the other pages weapons with armor, the consumables, and spells with powers and shouts. A single empty line separates the groups.
- Crafting Sorting page: sections now run in station order (smithing, enchanting, alchemy) instead of alphabetical.
- Icons page: "Reset this page" is the last line of its main section instead of a separate section.
- FOMOD installer: the survival mods (Creation Club Survival Mode, Frostfall, SunHelm Survival) are now check boxes in one list. A box is ticked for you when that mod's plugin is active.

## 0.11.1-beta30 (test build)

- Reverse sorting on every list that has a sort order (inventory tabs, Magic menu lists, all crafting menus): clicking the sort arrow now flips the sort. Arrow up = your chosen order (preset or custom). Arrow down = the same rules in the same order, each one reversed (for example Type A-Z, Sub-type A-Z, Name A-Z becomes Type Z-A, Sub-type Z-A, Name Z-A). It follows the custom levels as well; before, the down arrow always used a fixed order.
- Equipped-first stays on top in both directions when you have it switched on.
- Pages without an Info section (the Sorting pages, Icons, Magic Effects, System Settings) now have "Reset to defaults" as their own section at the top; the column pages keep "Reset this page" inside their Info section.

## 0.11.1-beta29 (test build)

- MCM pages: the two panels now fill independently, so section headers no longer have to line up and there is much less blank space. One empty line separates sections. Sections are grouped by kind on the Crafting Columns page (smithing on the left; enchanting, alchemy and cooking on the right).
- "Reset this page" is now the last line of each page's first section (the Info section on the column pages) instead of its own section. The System Settings page keeps its separate Reset section with "Reset all DICK settings".
- Sort order lists: the Soul size choices no longer carry "(Soul Gem tab)".
- Soul Gem tab: the Soul column's sort arrow now points down for high to low and up for low to high, the same as SkyUI's Value column (it was the other way round).

## 0.11.1-beta28 (test build)

- Crafting Columns page reorganised by station, in this order: Forge & Grindstone: Weapons, Forge & Workbench: Armor, Smelter & Tanning Rack, Enchanting Table, Alchemy Lab, Cooking Pot & Oven, then a short "Alchemy, Cooking Pot, & Oven" group that holds Green Pact. Reset sits under the shorter side.
- Enchanting Table: new switches for Effect (Disenchant tab, on by default, SkyUI's own column), Damage and Armor (Item tab, new, off by default) and Soul size (Soul Gem tab, on by default). The Item tab now uses its own Damage and Armor columns.
- Enchanting Table sorting: the Item and Soul Gem tabs now use the sort settings of "Enchanting: Items" and "Enchanting: Soul Gems" (before, they used the Other Crafting order). The Soul Gem tab defaults to gem size, then soul size, small to large; sorting by Soul size high to low gives Grand, Greater, Common, Lesser, Petty, then empty.
- Alchemy Lab: more space between the Green Pact, Known and the number columns. Green Pact is 0.08 wide in all lists.
- Not done in this build: per-tab sort memory at the Cooking Pot and Oven, and enchantment icons on the Enchantment tab.

## 0.11.1-beta27 (test build)

- Alchemy Lab: Value column filled (the list had no value field); optional Green Pact column between Name and Value; optional "Known effects" column (None, 1/4, 2/4, 3/4, All) computed from the ingredient. The PNGII progress ring cannot be drawn from DICK: PNGII only adds its status icons on the inventory-style menus, so that would have to be done in PNGII.
- Cooking Pot and Oven: own view with the inventory's food columns (Green Pact, CC Survival, SunHelm), optional. Their data comes from other mods and is only present on inventory rows, so DICK remembers it per item while the inventory is open: items you do not own yet may show blank.
- Enchanting table: Item tab shows current Damage and Armor; Soul Gem tab shows the soul size of each gem (Empty, Petty, ..., Grand), filled from the gem. The plugin now picks the view by the menu kind and tab, and logs the layout it found ("crafting layout ...") for each tab.
- Crafting menus: improve lists (Grindstone, Workbench) are recognised by the menu kind instead of by row type, so the Enchanting table no longer gets the smithing views.

## 0.11.1-beta26 (test build)

- Smelter, Tanning rack, Workbench: the view is now checked on every pass (SkyUI's current view flag against the wanted one) and re-switched whenever SkyUI has reset it, so FROM shows on first opening and the Workbench keeps its armor columns. Before, it switched once per tab and SkyUI's own reset undid it. The log keeps up to 60 "crafting view" lines.

## 0.11.1-beta25 (test build)

- Workbench and Smelter / Tanning rack: the view switch now uses SkyUI's flag numbers (read from SkyUI's own Flash code; they could not be looked up at run time): armor view (flag 4) at the Workbench, weapon view (flag 1) at the Grindstone, FROM view at the Smelter and the Tanning rack. The Workbench and the Grindstone report the same tab flag (1) to SkyUI, which is why the Workbench got weapon columns.
- FROM column text is right-aligned like SkyUI's own columns.

## 0.11.1-beta24 (test build)

- Forge: FROM column fixed. SkyUI uses the last view of a layout as its fallback, and the FROM view had become the last one; the plain view is last again, so no forge tab shows FROM. Side effect: the Smelter and Tanning rack lose FROM until the plugin can switch views (see below).
- Crafting lists: narrower Type column (0.27 to 0.14) and fixed widths for Value, Weight and Value/Weight, so item names no longer run into the next column; the FROM view keeps at least a third of the list for the name.
- Diagnostics: DICK.log now lists the tab (category) flag numbers of the crafting lists and of the Magic menu. They are needed to tell SkyUI which view to use at the Workbench (armor) and at the Smelter and Tanning rack (FROM). The first attempt failed because the flag constants could not be read from the Flash movie ("no flag").

## 0.11.1-beta23 (test build)

- Workbench (armor improve): the plugin now asks SkyUI's layout for the armor view (and the weapon view at the Grindstone), because SkyUI gave both improve lists the weapon columns. What the layout accepted is written to DICK.log ("crafting view ...").
- Smelter and Tanning rack: the FROM column now has its own view, shown only at those two stations, directly after the item name (before Type). The forge (all tabs) never shows it.
- Fixes in the build scripts only otherwise.

## 0.11.1-beta22 (test build)

- Grindstone and Workbench: the improved Damage / Armor now goes on the right row. The row is found by name from the item card's data, not by the list's selection index (that index did not match the rows and made values jump between rows). The lists now use the same weapon and armor columns as the forge (Damage, Base Damage and the other weapon columns on the Grindstone; Armor, Base Armor and the other armor columns on the Workbench), so no unrelated columns.
- The separate Damage / Armor columns of beta21 are gone (the normal DAM and ARM columns show the improved value instead).
- Smelter and Tanning rack: only the "Breaks down" column is added (wider than before). Forge: unchanged (no Breaks down column).

## 0.11.1-beta21 (test build)

- All extra columns are off by default now, except the Active Effects Type column (on by default).
- Grindstone and Armor Workbench: new optional columns Damage and Armor (the current value; the selected item shows the improved value from the item card), plus Base Damage and Base Armor. The improved value is read from the item card; what the card gives is written to DICK.log ("crafting card data") to check it.
- Smelter and Tanning rack: new optional column "Breaks down" (the item that is used up, read from the recipe).
- The splash image is not re-rendered for test builds; it is refreshed for the next final build only.

## 0.11.1-beta20 (test build)

- Forge, Ammo tab: Base Damage now shows the arrow's damage (arrows have no Speed, Reach or Stagger, so those stay empty).
- More logging in DICK.log for the crafting menus (first row of each kind of list and the members of the menu and its item card) to find the improved Damage and Armor values for the Grindstone and Workbench.

## 0.11.1-beta19 (test build)

- Forge and other crafting menus: found SkyUI's crafting list (`_root.Menu.InventoryLists.itemList`), so the extra columns should now be filled. The first rows are logged to DICK.log to find the fields for the improved Damage/Armor at the Grindstone and Workbench.

## 0.11.1-beta18 (test build)

- Diagnostics only: if the forge list cannot be found, the structure of the Crafting Menu is written to DICK.log so the right list path can be set. No visible change.

## 0.11.1-beta17 (test build)

- Forge and other crafting menus: the extra columns were blank because DICK only filled in the data for the inventory-style menus. It now also fills the Crafting Menu rows (Base Damage, Speed, Reach, Stagger, Base Armor, Slot, warmth). SkyUI's crafting list is not documented, so several list paths are tried and the first crafting rows seen are written to DICK.log ("crafting menu list: ...") to confirm.
- Crafting menus no longer have Total Value or Total Weight columns (forge, enchanting, alchemy); the "Smithing: Totals" group and the two Alchemy total toggles are gone from the Crafting Columns page.

## 0.11.1-beta16 (test build)

- Crafting Columns page: new groups "Smithing: Weapons" (Base Damage, Speed, Reach, Stagger), "Smithing: Armor" (Base Armor, Slot and the CC Survival, Frostfall and SunHelm warmth columns) and "Smithing: Totals" (Total Value, Total Weight). They are the same settings as on the Inventory Columns page, so the forge lists get the same extra columns as the inventory tabs; switching one on in either place switches it on in both.

## 0.11.1-beta15 (test build)

- Wording: the "gear menu" is now called the SkyUI menu (the gear icon above the list) on the column pages and in the README. The column page note is now "Available in the SkyUI menu" and "Maximum of 12 columns", and every column toggle has a clearer help text.
- Proofread the other MCM help texts (Icons, Reset, Active Effects icons, strict rule files, log and reload options).

## 0.11.1-beta14 (test build)

- (CC Survival) Warmth confirmed in game: Nightingale and Shrouded pieces show the values from the Survival Mode table (head 29/18, body 27, hands and feet 13), and the column sorts.
- Removed the per-item warmth lines that beta12 and beta13 wrote to DICK.log (about 115,000 lines in one session) and the WarmthRating line (it always read 0).
- Total Value and Total Weight: every list except All now has its own copy of these two columns, so ticking one in a tab (Apparel, Potions, Food and so on) no longer changes the other tabs. Copies start ticked when they fit in the 12 columns and unticked when they do not.
- Column pages: the long note is now two short lines with the details in the mouse-over help at the bottom.

## 0.11.1-beta13 (test build)

- (CC Survival) Warmth: checked against an xEdit export of the load order. An item now counts once by its main slot (body, then head, then hands, then feet) instead of adding every slot it covers, because Survival Mode has a separate keyword (Survival_BodyAndHead, used on hooded robes) for items that give body and head. Worn pieces and the player's WarmthRating are still logged to verify the numbers.

## 0.11.1-beta12 (test build)

- (CC Survival) Warmth on armor now has data. Survival Mode gives head, body, hands and feet pieces 8/18/29, 17/27/54 and 7/13/24 points (cold/normal/warm item), from UESP Skyrim:Cold; the tier comes from the Survival_ArmorCold and Survival_ArmorWarm keywords (none = normal). Slots 30/31 count as head, 32 body, 33 hands, 37 feet. Not verified against the game yet: DICK.log now lists each worn piece with its computed warmth and the player's WarmthRating when the inventory opens, so the numbers can be checked.

## 0.11.1-beta11 (test build)

- Apparel: with several extra columns on, the last column (Value/Weight) was ticked but drawn blank, because the column count skipped it (SkyUI's config hides it, yet the game draws it). It is now counted, so the surplus Total column is cut and gets its own copy like on Weapons. Weapon Equip is not counted (it starts unticked in the gear menu).

## 0.11.1-beta10 (test build)

- Column pages: the note now explains the 12-column limit: name and icon use 2 of the 12, equip uses 1 more on tabs where you can equip things (gear, spells), and extras past 12 start unticked.
- No other change from beta9. SkyUI appears to remember gear-menu ticks per column, so test the gear menu defaults on a save that has never seen these builds.

## 0.11.1-beta9 (test build)

- Source icons, Mara, Beastblood and racial abilities: the icon pack has an effect rule for the effect form of these rows and it wins over a label whatever the priority. New rule option `iconLabelOnly`: the row stops matching form rules so the label icon decides. Used by Agent of Mara, Beastblood (also no longer needs the ability kind) and the racial emblems.
- The old `29_Dark-DAEDRA-Labels.json` was still shipped next to `20a_Dark-DAEDRA-Labels.json` (the base zip brings it back at every build and the rename step had been broken); it is now removed.
- Gear menu: a column SkyUI cannot show because the view already has 12 is listed in the gear menu but starts unticked. SkyUI keeps the ticked state once per column, not per view, so a column that fits in one view but not in another (Total Value, Total Weight, Main Effect, Mod) now has a copy (`<column>_ov`) in the views where it does not fit; ticking it there does not change the other views. Extras are cut from the end first, then SkyUI's own end columns, so no column is left blank.
- Magic and inventory page note shortened to "Max 12 columns: extras start unticked."

## 0.11.1-beta8 (test build)

- Source icons: the label icons (Agent of Mara, Beastblood, blessings, Mephala and so on) lost to the icon pack's effect rules because PNG Icon Injector ranks matching rules by priority, not by file order. Every rule in `20a_Dark-DAEDRA-Labels.json` now has priority 60.
- Racial abilities (Resist Fire and other racial passives) show the emblem of your race: new DAEDRA rule `dick.racial.any` (new `source.racial` match) plus `fx_racial_<race>` icons for the ten base races.
- Gear menu: a column that fits in one view but is over the 12-column limit in another (Total Weight, Main Effect, Mod and so on) could not be unticked, because SkyUI keeps that flag per column, not per view. It is now left out of the views where it does not fit and stays in the gear menu of the views where it does.
- Reset page and Reset all options set every column back to unticked; the installer's survival choices only decide the starting values.
- Inventory Columns page: the mod tag now comes first: "(CC Survival) Hunger column", "(Frostfall) Warmth column", "(SunHelm) Thirst column".
- Icons in Active Effects: the Effect icons option is marked as work in progress.

## 0.11.1-beta7 (test build)

- Source icons: back to keeping the icon pack's effect-type icons installed (they carry the fallback icons and the skill-perk and racial icons), and the beta6 catch-all rule that gave abilities a generic power icon is gone. Instead the label icons (Agent of Mara, Beastblood, blessings and so on) now live in `20a_Dark-DAEDRA-Labels.json`, which PNG Icon Injector reads before `21_Dark-Effect-Types.json`; the first matching rule wins, so the label should now beat the effect rule.
- Active Effects rows are redrawn once more after the icons are set, to cut down the generic icons that only turned correct after a mouse-over or scroll.
- Gear menu: every column you enable in the MCM now stays in the gear menu. SkyUI draws at most 12 columns per list, so extras beyond the first 12 shown columns start unticked there and you choose which to tick. Narrowing only applies to the columns actually shown.
- Inventory Columns page: "(CC)" is now "(CC Survival)" and "(Survival)" is now "(SunHelm)".
- Installer choices: DICK checks that the values were really written before it marks the install as done, instead of trusting the call; the stamp is kept in Data/SKSE/Plugins/DICK/cache/install-stamp.txt.

## 0.11.1-beta6 (test build)

- Source icons now win over the icon pack's effect-type icons: those rules are only installed in "Effect icons" mode (a restart applies the change). Any ability, spell or power that has no rule of its own shows the icon of its source instead of falling back to the effect icon.
- Potions, poisons and ingredients: DICK now also learns the icon label of those items from the Inventory menu (visit the Potions and Ingredients tabs once), so a potion in Active Effects shows a potion icon instead of a generic one.
- Off now says what it does: DICK's generic magic effect icon on every row.
- Column layout: SkyUI draws at most 12 columns per list and leaves the rest blank, so extra columns beyond 12 are now left out (from the end) instead of showing blank. Column narrowing only happens on lists that show extra columns, so the default lists look as before.
- Inventory Columns page: the Reset group sits in the right pane next to Food and Ingredients.
- Beta packages carry only the AE DLL (1.6.x / 1.7.x); the 1.5.97 option is greyed out until the final build.

## 0.11.1-beta5 (test build)

- FOMOD: the survival column choices now take effect for existing installs too. The installer saves its choices in Data/SKSE/Plugins/DICK/install-defaults.json and DICK applies them once, at the next game load, through MCM Helper (an existing settings file kept the old values before). The version page lists the newest game version first. The "PNG Icon Injector is missing" and Address Library warning pages are gone (a mod manager cannot detect those files reliably); the requirements are listed on the version page instead.
- Type column: a spell found in any race's ability list now counts as Racial (Resist Fire and other abilities of your ancestry). An ability that only shares a perk's name now ranks below the label rules, so Beastblood says Curse again while Ordinator's script-granted abilities still say Skill Perk.
- Column layout: when the switched-on columns of a list add up to more than about three quarters of its width, they are narrowed together so the Name column keeps room and nothing overlaps it. Mod and Main Effect text is cut at 12 characters.
- New choice on the Magic Effects page: Icons in Active Effects = Source icons (each row shows what causes the effect), Effect icons (each row shows the icon of the effect itself, from the icon pack) or Off (the plain icons SkyUI draws). It replaces the old on/off switch "Source icons in Active Effects"; it starts on Source icons. Restart the game after changing it.
- Source icons: potions, food, poisons and eaten ingredients now show the item's own icon (bowl, bottle, ingredient) instead of the icon of the effect.
- Not done: Warmth (CC) on armor stays empty (the value is not in the data SkyUI receives); postponed.

## 0.11.1-beta4 (test build)

- Type column: now sits between Time Left and Source. Abilities that mods hand out by script now count as perk abilities when they carry the name of a perk you have (Ordinator's Expert, Meric and Exotic Smithing now say Skill Perk), and a sub-ability that shares the name of a racial ability now says Racial too (Fire Captured). The player's own record and the race's armor parent race are searched for racial abilities as well.
- The new Magic columns no longer show a "$" before their headings, and every Magic column is narrower (SkyUI's own too: Type, Class, School, Level, Magnitude, Duration, Cost, the three Shout words, Time Left, Source) so more fit next to the name. Mod and Main Effect text is cut with ".." when it would spill into the next column.
- Includes the beta3 FOMOD installer (not yet tested in a mod manager).

## 0.11.1-beta3 (test build)

- FOMOD installer (new package "DICK ... (FOMOD).zip"). Pages: Skyrim version (SE 1.5.97, or AE 1.6.x / 1.7.x: each gets its own DLL built for that game family); Survival columns (Creation Club Survival Mode, Frostfall, SunHelm: each On or Off, On by default when that mod's plugin is active; the choice also sets what "Reset to defaults" restores); and warnings when SkyUI, MCM Helper, PNG Icon Injector or the 1.5.97 Address Library is missing.
- No change to the DLL code since beta2.

## 0.11.1-beta2 (test build)

- New Magic menu columns, all on the Magic Columns page and off by default (the data is read from the game when the list opens):
  - Spells: Delivery (Self, Touch, Aimed, Target, Location), Cast Type (Instant, Hold, Constant), Casts (how many you can cast with your current magicka, or the seconds you can hold a concentration spell; sortable), Main Effect (the spell's costliest effect), Mod (the plugin the spell comes from).
  - Powers: Delivery, Main Effect, Mod (these three columns are shared with Spells; switch them on under Spells).
  - Shouts: Cooldown (the recharge time of word 1, 1+2 and 1+2+3, for example 15/20/30s), Mod.

## 0.11.1-beta1 (test build)

- New Active Effects column: Type (Magic Columns page, off by default). Every active effect is labelled from its source, with no per-mod rules needed: Skill Perk and Unique Perk (an ability granted by one of your perks, depending on whether the perk is in a skill tree), Racial (your race's own abilities), Blessing, Faith (Wintersun), Standing Stone, Curse, Creation Club, Enchantment, Gear, Potion, Poison, Food, Ingredient, Scroll, Spell, Power, Shout, Disease, Staff, Cast by other, and Ability for anything else. A rule's new `typeText` setting overrides it for one effect, and Data/SKSE/Plugins/DICK/effect-types.json adds more labels for a mod (see the README).
- The Type data is filled in even when "Source icons in Active Effects" is off.

## 0.11.0

First release of the merged DICK (item categories, sort columns and the former DAEDRA Active Effects icons in one DLL, one MCM menu and one log). Final build of the 0.11.0-beta series below. Not yet tested in game: the crafting-menu sort orders and the survival-mod columns (planned for 0.11.1).

## 0.11.0-beta14 (test build)

- Reset switches: the 5 second countdown of beta13 never ran (the plugin only looked at the settings file when it changed) and its messages cannot show while the MCM is open. Now ticking a reset switch arms it, the reset runs when you close the menus, and unticking before closing cancels it. The tick clears itself after the reset.

## 0.11.0-beta13 (test build)

- Reset switches now have a 5 second countdown: ticking shows a message, unticking within 5 seconds cancels the reset, otherwise it runs and the tick clears itself.
- System Settings: the About section is now first.
- "Source icons in Active Effects" help now says Off leaves the plain generic white magic-effect icon and that the game must be restarted after switching it either way (switching mid-session can look patchy).

## 0.11.0-beta12 (test build)

- "Source icons in Active Effects" off now also switches off the icon pack's effect-type icons: the four rule files 21_Dark-Effect-Types, 26_Dark-ActiveEffects, 28_Dark-Skill-Perk-Effects and 30_Dark-Effects-Remaining in SKSE/Plugins/PNGIconInjector are renamed to *.json.off (back when switched on). PNG Icon Injector reads them at game start, so the change shows after the next game start. These rules are keyed by effect, so effect icons may also change outside the Active Effects tab.

## 0.11.0-beta11 (test build)

- Reset switches now work as tick boxes: ticking one resets (a page, or everything on System Settings), the plugin then unticks it again by itself, and unticking does nothing. A switch found ticked at game start is only unticked.
- Icons, Magic Effects and System Settings now use both panels (groups go left, right, left, right).
- Main page thumbnail: larger (640x320), bolder text, lossless image so it is less blurry, and the version at the bottom is rendered for each build.
- Magic Effects: the help text now says the switch only controls the source icons; the effect-type icons of the icon pack (armor, health, resist...) are always on.

## 0.11.0-beta10 (test build)

- New last page "System Settings": "Reset all DICK settings" (the other pages keep only "Reset this page"), Strict rule files, the rule reload hotkey and switch, and the troubleshooting options (log level, log every rule hit, dump on menu open, dump hotkey), plus where the logs are. Magic Effects now only has the source-icon options.

- Reset to defaults: every page of the DICK menu now ends with two switches, "Reset this page" and "Reset all DICK settings". Flipping one (either direction) makes the plugin ask MCM Helper to set the listed settings back to their defaults (the same calls other mods use for their reset buttons; DICK does not write the ini itself). Reopen the DICK menu afterwards to see the new values. The setting lists are in SKSE/Plugins/DICK/reset.json; the log line is "[reset] ...".

## 0.11.0-beta8 (test build)

- MCM main page: new thumbnail (title in the DarksSkyrimFont, colored icons, a row of column headers with sort arrows, version), centred on the page.
- DICK.log from the previous game session is kept as DICK.previous.log; the "Magic menu opened" line now reports whether source icons are ON or OFF.

## 0.11.0-beta7 (test build)

- Total Value and Total Weight columns now have data (value or weight times the stack count), and sorting by them works. Filled in by the plugin on the Inventory, Container, Barter and Gift menus (not yet on the crafting menus).
- Base Damage, Speed, Reach, Stagger, Base Armor and Slot columns now have data (read from the weapon or armor record). Warmth, hunger and similar survival columns still depend on the survival mods supplying that data.
- MCM: on pages with several groups, groups now go across then down (left, right, left, right). Shorter intro text on the Columns pages. The DICK main page is now a splash image (title, version, icons) like other MCM menus.
- Active Effects source icons switch: no code fault found; needs a log from a session where the Magic menu is opened after the switch is turned off (see the beta7 notes).

## 0.11.0-beta6 (2026-11-23, beta; becomes 0.11.0 when final)
- Credits: the URW (Urwy) line in OPEN_ICON_CREDITS.txt no longer says the author was notified; it now states his terms (free to use with credit, files not re-uploaded). No other change.
- Page order: Icons first, then the other pages alphabetically (Crafting Columns, Crafting Sorting, Inventory Columns, Inventory Sorting, Magic Columns, Magic Effects, Magic Sorting).
- New pages "Crafting Columns" and "Crafting Sorting". Crafting menus now sort separately: Smithing: Weapons, Smithing: Armor, Other Crafting (the generic crafting list), Disenchanting, Enchanting: Items, Enchanting: Soul Gems and Alchemy (each with its own order, equipped-first switch and five custom levels). Smithing no longer shares the Weapons and Armor settings, and "Crafting" is gone from Magic Sorting. The Alchemy extra columns (Total Value, Total Weight) moved to Crafting Columns.
- Pages renamed: "Item Columns" is now "Inventory Columns" and "Item Sorting" is now "Inventory Sorting". Magic Columns is reserved for Magic menu columns (it has none yet); the crafting (Alchemy) columns moved to Inventory Columns.
- Inventory Columns / Magic Columns now only list the extra columns DICK adds (Total Value, Total Weight, Base Damage, Speed, Reach, Stagger, Base Armor, Slot and the warmth and food columns of the survival mods; checked against the original SkyUI 5.2 config, which already has Material, Value/Weight, Class, School and the Power columns). SkyUI's own columns are no longer in the MCM: use the gear menu above the list. A switched-off extra column is removed from the views, so it does not appear in the gear menu at all; switched on, it is listed there and shown (untick it in the gear menu to hide it). All extras are off by default.

## 0.11.0-beta5 (2026-11-21, beta; becomes 0.11.0 when final)
- Fix: "Equipped items first" did nothing in the Magic menu (Spells, Powers, Shouts, Active Effects, Crafting). Those rows may not carry the item property the sort used, so the Magic tabs now sort by both `isEquipped` and `equipState`. Item tabs are unchanged.
- Inventory Columns / Magic Columns / Inventory Sorting / Magic Sorting: each panel now gets whole groups, split to equal height, instead of pairing groups row by row (that left the right panel empty on Inventory Columns).
- Log: "[effects] source icons in Active Effects: ON/OFF" whenever the switch changes, and a line when the Magic menu opens with it off (to diagnose the switch).
- Known: settings saved by the empty dropdowns of earlier betas (value 4294967295) show as blank levels; press R (Default) on those rows or delete the lines from `Data/MCM/Settings/DICK.ini`.

## 0.11.0-beta4 (2026-11-21, beta; becomes 0.11.0 when final)
- Fix: the custom sort-level dropdowns opened empty. In-game tests showed MCM Helper breaks any dropdown that contains an entry literally named "None"; the entry is now called "Off". The temporary Test Dropdowns page is removed.
- Inventory Sorting, Magic Sorting, Inventory Columns and Magic Columns now use both MCM panels (two categories side by side), so the pages are about half as long.
- Column toggles are named "<name> column" and the sort dropdown "Sort order" so the game does not translate the labels.
- DAEDRA is merged into DICK. `DICK.dll` now contains the sort menu and the Active Effects rule engine; there is no separate DAEDRA plugin to install and the effect-source rules are built in (no "needs DAEDRA 0.1.0 r22" requirement any more). One SKSE entry point, one log (`DICK.log`, effects lines start with `[effects]`), one MCM menu.
- Rules moved to `Data/SKSE/Plugins/DICK/Effects/` (file `effects-dick.json`; was `SKSE/Plugins/DAEDRA/DICK.json`). The label cache moved to `Data/SKSE/Plugins/DICK/cache/item-icon-labels.json`. Your own rule files go next to `effects-dick.json`.
- New MCM page "Active Effects" replaces `DAEDRA.ini`: show source icons, copy type and keywords, strict rule files, log level, log every rule hit, dump on Magic menu open, dump hotkey, reload hotkey and a "Reload rules now" switch. Defaults equal the old DAEDRA.ini defaults (unit-tested). Settings are read thread-safely and never written by the plugin.
- Fix: the Active Effects list is now re-applied after tab switches and filters even when no hotkey is bound (it was skipped unless a dump or reload key was set).
- Removed with the merge: DAEDRA's public API (`DAEDRA_API.h`, the 'DAER' broadcast, RegisterRulesJson). Nothing used it.
- Plugin: CommonLibSSE-NG is now a copy in `plugin/extern` (no longer shared with the DAEDRA folder); tests: `daedra_tests` (rule engine) and `dick_tests` (sort menu, settings, reload trigger). Docs carried over to `plugin/docs`, schema to `plugin/schema`. GPLv3 (the DAEDRA licence) applies to the DLL; see the licence files at release time.
- In-game sort menu (planned for 0.10.1, now part of 0.11.0; MCM Helper menu "DICK", plugin `DICK.dll`, no ESP or Papyrus): weapon order (type + damage, type + name, type + value, type + weight, damage first), potion order (type + effect + magnitude, type + magnitude, strongest first, name), order of the other tabs (by type, or name only), equipped items first, and show/hide switches for the Type, Value, Weight, Total Value, Total Weight, Value/Weight, Material and weapon Base Damage, Speed, Reach and Stagger columns. The plugin watches `Data/MCM/Settings/DICK.ini` and rewrites the sort lines of `Interface/skyui/config.txt` (rendered from `SKSE/Plugins/DICK/config.base.txt` and `profiles.json`); SkyUI reads it when an item menu opens. The defaults reproduce the shipped config exactly (unit-tested). Data generated by `tools/build_mcm_0101.py`.
- Weapon icon option in the menu: Standard or Bold (long weapons drawn 33% thicker, compact ones +3 px), made from the final 0.10.1 icons. The plugin copies `Interface/PNGIconInjector/DICK_variants/<standard|bold>` into `base/`; PNGII shows the change after the next game start.
- README: new "IN-GAME SORT MENU" section and MCM Helper as an optional requirement (`tools/patch_readme_0101.py`). Build: `tools/apply_0110.py` (the old 0.10.1 chain: 0.10.0 chain, thickness picks, MCM data, Active Effects page, README); `build_release.py` adds `plugin/build/plugin/Release/DICK.dll` to the zip when it exists.
- To confirm in game: SkyUI re-reads config.txt when the menu opens; MCM Helper writes the settings ini at once; Vortex tolerates the plugin rewriting config.txt and the SVGs.
- MCM fix: MCM Helper only lists a mod whose plugin has a quest running its `MCM_ConfigBase` script, so `DICK.esp` now holds exactly one record, a Start Game Enabled quest `DICK_MCM_Quest` (light plugin form 0x800) with `MCM_ConfigBase` (ModName "DICK") and a `SKI_PlayerLoadGameAlias` player alias, same layout as TrueHUD. Generated by `tools/make_esp_0110.py`. Without it the menu never appeared (MCMHelper.log had no line for DICK).
- Staging: `tools/patch_effects_0110.py` (run by `apply_0110.py`) moves the rules to `SKSE/Plugins/DICK/Effects/effects-dick.json`, replaces the "optional DAEDRA" README wording with "built into DICK.dll", and adds `DICK_plugin_LICENSE.txt` and `DICK_plugin_NOTICE.txt` (GPLv3) with a source-availability line. Source: the `plugin/` folder; include it or link to it on the mod page.
- MCM redesign (from the first in-game test): main page with version, page list and log location; pages in alphabetical order: Icons, Inventory Columns, Inventory Sorting, Magic Columns, Magic Effects (the former "Active Effects" page); short labels and option names (details in the help text) so text no longer overlaps. Inventory Sorting has Weapons / Potions / Other Items blocks, each with Order (the old presets plus a last choice "Custom"), "Equipped items first" per tab (the single global switch is gone) and five Custom levels (None, Type, Sub-type, Name A-Z/Z-A, Value, Weight, Value/Weight, plus Damage for weapons, Effect group/Strength/Duration for potions, Armor rating for other tabs). Default levels reproduce the first preset exactly (unit-tested); SkyUI's time-remaining/detrimental/school prefix and the name tie-breakers always stay. Inventory Columns and Magic Columns have a toggle for every column that has a hidden flag in config.txt (58), grouped by inventory/magic/crafting category: SkyUI columns default to on, columns DICK adds default to off. Generated by `tools/build_mcm_0110.py` (run by `apply_0110.py`); settings keys changed (new `Sort/u<Tab>Level1..5`, `Sort/b<Tab>EquippedFirst`; `Sort/bEquippedFirst` removed). Unverified: that MCM Helper shows the root-level info page and that SkyUI lists DICK alphabetically.
- Sorting groups: SkyUI shares one sort column between many tabs, so DICK now gives every category its own copy (`armorIconColumn`, `scrollIconColumn`, `foodIconColumn`, `ingredientIconColumn`, `bookIconColumn`, `miscIconColumn` (also Keys), `spellIconColumn`, `powerIconColumn`, `shoutIconColumn`, `effectIconColumn`, `craftIconColumn`; weapons and potions already had theirs) and points that category's views at it. The copies start identical to `iconColumn`, so nothing changes until you pick an order. Inventory Sorting has Weapons, Armor, Potions, Scrolls, Food, Ingredients, Books and Misc/Keys; the new page Magic Sorting has Spells, Powers, Shouts, Active Effects and Crafting. Every group has Order (presets + Custom), Equipped items first and five Custom levels; the level choices are taken from the sort attributes of the columns that category shows (each numeric or text column gives a high-low/low-high or A-Z/Z-A pair), plus Type, Sub-type and Name. Settings keys: `Sort/u<Group>Sort`, `Sort/u<Group>Level1..5`, `Sort/b<Group>EquippedFirst` (the old `uOtherSort` is gone). To test in game: whether a criterion whose column is switched off (for example Value/Weight, Total Value) still sorts.
- beta2 (from the beta1 test in game): sort-level dropdowns opened empty and then cleared their value (cause not yet known; beta2 adds a temporary page "Test Dropdowns" with dropdowns of different lengths to find it, to be removed again). Labels that equal a game translation key were shown translated (type, value, weight, order, DAMAGE, ARMOR RATING ...): column toggles are now named "<Name> column" and "Order" is "Sort order".

## 0.10.1 (2026-11-21)
Icon-only release: weapon icon thickness. The in-game sort menu that was planned for this build moved to 0.11.0 (no DICK.dll has been compiled yet).
- Many long weapons were too thin to read at inventory size. All weapon rows (no ammo) were reviewed in the Icon Picker with width options that keep every shape detail; the 28 picks below changed, everything else keeps its 0.10.0 icon. Generated by `tools/thicken_0101.py` from the 0.10.0 icons (`tools/icons_0100_base`); picks are in `tools/picker_build/picker_exports_0101.txt` and applied by `tools/resolve_thick_0101.py`.
  - +25% wider, whole icon: bow, quarterstaff, rapier, shiv, trident, twinblade, wakizashi, woodaxe, woodsword.
  - +25% wider, blade/shaft only: greatsword, lance, sword.
  - +25% grown evenly all round (outline grown by a percentage of the body width instead of stretched along one axis): hammer, katana, nodachi.
  - +25% shaft only (the head, blade and guard stay as drawn): battleaxe, halberd, javelin, pike, scythe (the neck from the blade head down is included), spear, staff, staff_blank.
  - Outline: crescent, crossbow and whip +3 px; pickaxe and saw +6 px on the thin parts.
- Fixed in the base icons: the glaive handle (jagged steps replaced by one straight band) and the javelin shaft (kink removed). The glaive keeps its size otherwise.
- Build: `tools/apply_0101.py` extracts the 0.10.0 release as the base, applies the thickness picks (`resolve_thick_0101.py`, `patch_weapons_0100.py`) and stops; the 0.10.0 rules, labels and sort are untouched. `tools/build_release.py` leaves out changelog entries for versions newer than the one being built.
- Not tested in game. To check: the changed weapon icons at 24 and 32 px in the inventory, QuickLoot and Recent Loot.

## 0.10.0 (2026-11-21)
Version note: this build was planned as 0.9.7. It is numbered 0.10.0 because it changes the design of the weapon and ammo icons from single-colour silhouettes to detailed multi-colour icons (up to four colours per icon, taken from each in-game model's textures), a decision that applies to future icon work.
- Recent Loot (TrueHUD) weapon icons now match the inventory and QuickLoot: the Nordic War Pick showed a war axe in the feed but a pickaxe elsewhere, because the feed only follows PNGII rules and PNGII's own WeapTypeWarAxe rule beat DICK's Inventory Injector label (OCF_WeapTypeWarpick). New `37_Dark-Loot-Weapons-0100.json` (priority 50) mirrors all 94 keyword-based weapon label rules from DICK.json in the same order (later rule wins, as in Inventory Injector), then adds explicit form rules for the weapons of the official game plugins (32 rules, 93 forms), so it is the same in every load order. Generated by `tools/patch_loot_weapons_0100.py`. Ammo, armor and the other item types are untouched (the arrow icon beside the HUD ammo count is the equipped-ammo display, not a loot card).
- Weapons and ammunition now sort by damage inside each type: Weapon > weapon type (alphabetical) > damage high to low > name, and Ammo > ammo type (Arrow, Bolt, ...; alphabetical) > damage high to low > name. The group order (weapons, tools, ammo) and every other tab are unchanged. Done with a weapon-only copy of the icon column (`weaponIconColumn`, sort chain plus `infoDamage` descending after the type) used by the Weapons, All, Favorites and weapon crafting views (`tools/patch_sort_0100.py`).
- README sort section updated. Build: `tools/apply_0100.py` runs the 0.9.6 chain, then the weapon sort and the loot weapon rules.
- New weapon icons: every weapon type SkyUI can list now has its own icon. New labels (Inventory Injector rules in DICK.json, PNGII label rules in `38_Dark-Weapon-Labels-0100.json`, Recent Loot mirror regenerated): `weapon_warpick` (war picks were pickaxe), `weapon_hammer1h` (Ebony Hammer was the tool hammer), `weapon_club` (was mace), `weapon_greatclub` (was warhammer), `weapon_scimitar` (was saber; `weapon_saber` now shows the same artwork), `weapon_glaive` (was halberd), `weapon_shiv`, `weapon_crescent` (was the native sword/war axe/greatsword icon), `weapon_staff_blank` (unenchanted staves and wands; enchanted staves keep `weapon_staff`, whose head is now soul-gem coloured).
- Weapon and ammo icons redrawn as multi-colour icons (up to 4 colours; colours taken from each model's texture) with silhouettes traced from the in-game meshes: 55 icons (`tools/icons_0100`, resolved from the approved picker choices by `tools/resolve_icons_0100.py`). Japanese swords (katana, nodachi, wakizashi) are thicker with filled hilt diamonds. Bow, crossbow, bullet, gun, pistol, arrow, bolt, chakram and the rest of the ranged set all changed.
- Credits: Urwy (URW - Useless Resources - Weapons: Steel War Pick, Ebony Hammer, Trident Blade, Daedric Crescent) and 747823 (Weapons of the Third Era: Iron Club, Silver Tanto) added to OPEN_ICON_CREDITS.txt. Urwy asks to be notified when his assets are used.
- Build: `tools/apply_0100.py` now also runs `tools/patch_weapons_0100.py` before the loot weapon rules.
- Not tested in game. To check: the multi-colour weapon icons in the inventory, QuickLoot and Recent Loot, the new weapon-type labels, and that ammo should list highest damage first inside each ammo type (this assumes SkyUI exposes damage for ammo as it does for weapons).

## 0.9.6 (2026-11-18)
- Fixed wrong icons in TrueHUD's Recent Loot feed: food, drinks, ingredients and misc items showed the generic apple, mushroom or default icon (Leg of Goat, Tomato, Eidar Cheese, Eidar Cheese Sliced and similar). PNGII draws the loot feed icons from its own rules only, so DICK's Inventory Injector keyword and form rules never reached it. New `35_Dark-Loot-096.json` (331 rules, priority 50, generated from the Inventory Injector rules by `tools/patch_loot_096.py`) mirrors them for food and drink, ingredients, misc items and lights. The feed resolves a PNGII label rule (default_food, default_ingredient, misc_clutter) as well as the item's form rules, and rules without an explicit priority outrank low numbers, so the generated rules use priority 50 and the explicit misc form rules in `27_Dark-Misc-Forms.json` are raised to 60 (priority 1 to 9 did not win; confirmed in game 2026-11-18). Weapons, armor, books, scrolls, soul gems and potions already resolved through TrueHUD's own labels and are untouched.
- Fallback `36_Dark-Loot-Forms-096.json` (105 rules, priority 50) for the official game plugins only (Skyrim, Update, Dawnguard, HearthFires, Dragonborn), so it is the same in every load order: the Inventory Injector rules evaluated per vanilla item (`tools/patch_loot_forms_096.py`, using a plugin scan and a Keyword Item Distributor emulation that also understands model-path rules) and written as explicit form rules, so vanilla items get their icon even if PNGII cannot resolve the OCF_* keyword names. Items from mods use the generic keyword rules in file 35. Salt Pile (both forms) gets the soup bowl icon (`food_stew`, from KID's OCF_VesselBowl model rule) like Inventory and QuickLoot.
- Generated loot rules never include potion or scroll icons (default_potion, potion_*, default_scroll, scroll_*): at priority 50 they overrode PNGII's per-effect potion icons in the inventory and feed.
- Potion sort now has an effect layer: Type > Effect > Magnitude. Inside Health, Magicka and Stamina: Restore, then Fortify (timed buffs), then regeneration-rate potions. The Fortify group (other attributes) is alphabetical by skill (Alchemy, Alteration, Archery, Block, Conjuration, Destruction, Enchanting, Heavy Armor, Illusion, Light Armor, Lockpicking, One-Handed, Pickpocket, Restoration, Smithing, Sneak, Speech, Two-Handed), then Carry Weight and the rest. 40 Inventory Injector rules assign `itemSort` (already part of the Potions column sort); applied by `tools/patch_potion_sort_096.py`. Skill rules match both the actor value (plain and `...Mod` names, since Fortify skill potions store the Mod value) and the vanilla effect keyword `MagicAlchFortify<Skill>`; only the keyword rules took effect in game for the Fortify skill potions. Confirmed in game.
- Scroll icons (default_scroll, scroll_spider) use the note parchment colour #efe4c0 instead of white.
- `19_Dark-Rings.json`: the ClothingRing rule used a `keywords` key that PNGII does not support (logged as a warning); it now uses `keywordsAny`.
- README: Object Categorization Framework (OCF) and Keyword Item Distributor (KID) are now listed as requirements; 1,230 of DICK's 1,617 Inventory Injector rules match OCF_* keywords (`tools/patch_readme_096.py`).
- Build: `tools/apply_096.py` runs the 0.9.5 chain and then the loot patch.
- Tested in game 2026-11-18: loot feed icons for food, cheese, meat, fish, fruit, plates, tankards and baskets; potion and scroll icons and colours; potion effect sort. PNGII rules use priority 50 (files 35/36) and 60 (file 27) because lower numbers lose to the generic label icon. Zip built 2026-11-18 with `bLogMatches = 0`.

## 0.9.5 (2026-11-16)
- Alembic recoloured (purple liquid #6241be/#896ed4, grey body #67757f). All tabs approved; zip built 2026-11-17.
- Misc round 2: Tolfdir's Alembic and the Beafarmer Alembic have their own `misc_alembic` label; the alembic uses the Twemoji alembic (approved); torch has an orange flame and a wood-coloured handle; suggested colours for inkwell (dark brown), lantern (copper), mortar (stone grey) and metal cup. Applied by `tools/patch_misc3_095.py`.
- Races and Deities: suggested colours applied (awaiting approval), one per race and per Divine, with no reds that could be mistaken for the Daedric (Wintersun Daedric deities) icon; Auriel deity uses the Auriel item lemon. Other, Skills, Effects, Races and Deities tabs approved.
- Misc: Aetherium Crest has its own label and icon (the crest from the Aetherial staff, enlarged, teal); the 35 Hearthfire BYOH house items (planter crops and ingredients, house mead, plus the Resource Pack and Goblins aloe/mushroom copies) use the house-part icon; the Auriel deity icon is now the Auriel sun crest from the Auriel bow (white like the other deities). Applied by `tools/patch_crest_095.py`. Magic and Food tabs approved.
- Food tab approved. Items that fell back to the default food icon now use proper icons: Salmon Steak (meat), Courtesy Ale and Courtesy Honningbrew Mead (beer), Home made Firebrand Wine (wine), Goodberry (default potion); Poisoned Red and Green Apple (Curios) get new labels with the poison skull cut out of the apple. Applied by `tools/patch_food4_095.py`. Books and Keys tabs approved.
- Gourd: new own drawing (thin striped gourd with stem, rotated 45, shaped like the in-game gourd); papaya, chitin and thorax approved.
- Food/Misc round 4 (picks from Icon Picker): carrot, tomato, mango, melon, pineapple (flipped) use Twemoji; leek, banana, kiwi use game-icons recoloured; papaya is the Twemoji mango with an orange body; gourd traced from the in-game image (colour #c9c46a); chitin is game-icons fish-scales rotated 45 and cropped to a few scales; thorax rotated 45 with the head notch filled and rib marks kept; green apple approved. Applied by `tools/patch_picks3_095.py`.
- Food/Misc round 3: Thorax icon is now a trace of the in-game reference image (earlier drawn version kept for the picker); green apple and the six Wintersun sacred fruits (banana, kiwi, mango, melon, papaya, pineapple) have their own labels (provisional recoloured apple icons until chosen in Icon Picker); carrot, gourd, leek, tomato and chitin icons are open for open-licence alternatives; cheese wheel, potato and antennae approved.
- Food round: the cheese wheel is now whole (no slice removed); vegetables split into own icons and labels (potato/yam: Potato, Baked Potatoes, Ash Yam; carrot; gourd: Gourd, Wild Gourd; leek: Leek, Grilled Leeks; tomato) with Cabbage staying on the vegetable icon; Skooma potion and drug icons use a lighter lavender purple (#9b84e8) that stays distinct from the poison magenta; dragonstone grey, strips #756000, spigot metal; goblet, jug and lute colours suggested. Apples (default_food labels) now show on the Food tab of the picker.
- Misc review round (picker): Mudcrab Chitin, Nordic Barnacle and Juvenile Mudcrab use the crab icon (unused hex-copy crab dropped); new cheese wheel icon for the two cheese wheels; Chitin is a fish-scale icon; Chaurus Hunter Antennae and both thoraxes have their own icons; butterflies and moths each have a coloured variant (default butterfly stays white); Dartwings are blue and orange; Bone Meal uses the bowl/soup icon and Beehive Husk the honeycomb; drum and the three flutes use their own labels; ore, stone ore and rock share the ore shape in different colours; Skull of Corruption is a weapon; Ayleid soul gem crystals flipped (point up on the right). Colours: egg #dddddd, cloth #EDDA87, bones one pale tone, tusk ivory, drug skooma purple, plus about 50 suggested colours awaiting approval.
- Potions tab: health, magicka, stamina, cures, resists, other, fortify and poisons keep their groups; inside each group the highest magnitude now comes first, then name. Done with a Potions-only copy of the icon column, so scrolls, spells and every other tab sort as in 0.9.4.
- Active Effects: new `30_Dark-Effects-Remaining.json` gives an icon to the 170 named lasting effects that had none (a scan of 753 plugins now finds 0). Hearthfire house parts use the house-part icon, Survival Mode exhaustion, hunger and affliction effects the camp, food and disease icons, Ordinator Tome of Many Pages and the Mage Guild ritual effects their skill icons, and DLC quest and creature effects the deity, bat, soul gem, detect-life and similar icons or the default effect icon. Existing icons only.
- Fixed the Dragon Priest mask icons showing black: the PNGII artwork had lost its fill colour in the recolour step. Base is white; light, heavy and cloth variants use the family colours of the other armor icons.
- Build: 266 icons that differ only in colour (weight variants, hex copies, aliases) now come from 82 master shapes and one colour table (`tools\label_colours.json`), so a colour is changed in one place and rebuilt. The shipped icons are identical to 0.9.4 apart from the Dragon Priest masks. Tested in game: PNGII ignores the I4 `iconColor` rule for its SVG icons, so colours stay baked into the files.
- Karstaag's Skull now uses its own pale frost blue copy of the PNGII troll skull; the plain troll skull stays white.
- Colour pass from the Icon Picker: armlets, bandolier, bra, choker, facemask, panties, piercing, scarf, stockings and tattoo variants use the light, heavy and cloth family colours; clothing crown cloth gold; Sunder, Blackbow, Keening, Wraithguard, Dwarven scrap, Dwemer core and Dwemer cube share one Dwemer gold (#c8a22c), and the Auriel items moved to a paler lemon (#ffe566) to stay distinct; the Aetherial items stay teal. Wraithguard has no weight variants, so its light, heavy and cloth rules and files were removed.
- Poison potion, Damage and Poison Resist icons: the old poison skull is replaced by the one used on Namira's Ring.
- Credits: PNGII icons are used and recoloured under the author's (rijosan) published permissions, with credit; the wording "not for paid mods" was corrected.
- DAEDRA (rebuild 2026-11-17, same 0.9.5 zip): the 18 skill rules are merged at priority -12 (below the worn-gear rule, so worn gear keeps its own icon) and a new `dick.quickshot` rule gives Quick Shot the Archery icon; 42 rules, 33 labels checked. Actor-value names verified against the F7 dump of 2026-11-17 (OneHandedMod, MarksmanMod, SneakMod, SpeechcraftMod, IllusionMod, DestructionPowerMod, RestorationSkillAdvance, Enchanting). Applied by `tools/patch_daedra_095.py`; `daedra_check_rules.py` now evaluates effect.actorValue.
- Not tested in game.

## 0.9.4 (2026-11-13)
Icon review pass: every icon row was reviewed in the Icon Picker and the approved picks are applied.
- About 270 icon labels changed or recoloured: weapons thickened with uniform unique-weapon glyphs, new misc, food, book, key and potion colours, effect icons (stamina, ward, resists, night eye, noise and others), apparel picks (scarf, eyepatch, cloak, Wraithguard, Clavicus Vile mask, rings, spellbreaker and more), flipped soul gems, brooms and pitchforks.
- Skill icons: all 18 skills have new badge icons (shield for combat, pinwheel for stealth, sparkle star for magic) with the skill glyph inside. Combat red, magic blue and stealth green. 12 skills also have `fx_skill_*` labels for DAEDRA.
- Deity icons: all nine are new drawings made from the in-game shrines.
- Race icons stay IAmNotSimon's (credited, see LICENSE_EXCEPTIONS.txt); Dunmer is now white.
- Fastened Shield of the Crusader now uses the shield icon and the Tribunal masks the mask icon; face masks, default armor and backpacks reuse the mask, body and backpack icons.
- DAEDRA: one rule now gives every Daedric Prince effect (Azura, Boethiah, Mephala and the rest, including Wintersun and similar mods) the red Daedric rune. Rule count is 23. The proposed skill rules are held back until their actor-value names are checked with a DAEDRA dump.
- Credits: Twemoji (CC BY 4.0), the race-icon exception and all new sources added to OPEN_ICON_CREDITS.txt and the README. game-icons.net author names are still missing for some new icons and must be added before 1.0.0.
- Not tested in game.

## 0.9.3 (2026-11-09)
Rebaselined release: this build replaces the earlier 0.9.3 to 0.9.12 test builds (2026-11-03 to 2026-11-06), which are archived and folded into it. Everything listed under "Folded-in builds" below is included.
- New, optional DAEDRA support: `SKSE/Plugins/DAEDRA/DICK.json` (23 rules) tells apart Active Effects rows that share one effect but come from different sources. Icons come from the new `29_Dark-DAEDRA-Labels.json`. Needs DAEDRA 0.1.0 r22 or newer; nothing changes if it is not installed.
- Rules cover shrine blessings and Agent of Mara (deity icons), Beastblood (paw), Follower/Devotee of Mephala, Aetherial Crown, Relics of the Crusader, Azura's Star, Summermyst "Unified Ab" abilities, any disease, the five school master-quest trackers (Apocalypse and ODIN), and a low-priority rule that gives effects from worn gear the gear item's icon.
- Rules were written from DAEDRA.log dumps of one load order; not yet tested in game.
- Dodo power icons are replaced (18 of 18), including the tombstone, hands, fists, drops and emblems. Dodo skills are not yet.
- Stone, QuickLoot enchantment-status and other icon replacements from the 2026-11-06 sessions are included.
- Fixed QuickLoot IE item names overlapping their icons (Mammoth Tusk, Cast Iron Pot and other DICK-labelled rows): `Interface/DICK/icons.swf` is now a valid SWF with an invisible 128x128 clip instead of an empty stub, so QuickLoot indents the text. Confirmed in game.

### Folded-in builds (archived in `releases\_archive`)
### 0.9.12 (2026-11-06, archived)
- Every icon that came from AIT, THICC (KIT), BOOBIES, SkyUI or I4 is replaced with openly licensed or self-made art: 140 icons from AIT, THICC, BOOBIES and SkyUI plus 26 I4 icons, traced from the game's own meshes or drawn from basic shapes. Unique-weapon emblems (Miraak mask, Eye of Magnus star) added.
- PNGII icons used by the mod are bundled under its asset-use permission and credited. README rewritten.
- Release candidate: 1.0.0 follows the in-game checklist.

### 0.9.11 (2026-11-03, archived)
- Trident with long handle, chalice with cross, tankard narrowed at the bottom.
- New book family (plain, manual with hammer, Hermaeus Mora stand-in, five spell schools), scroll family (note, missive with gold bag, Atronach Forge stand-in) and rolled scroll, built from basic shapes plus open symbols.

### 0.9.10 (2026-11-03, archived)
- Cheese and musket balls reverted to the original open icons (cheese wedge, bullets).

### 0.9.9 (2026-11-03, archived)
- Cheese is a wheel missing a slice (cut face visible); musket balls are a close diagonal stack of four.

### 0.9.8 (2026-11-03, archived)
- Wings tilted back, crotch raised on trousers, original bread icon widened and rounded, cheese wheel without inner gap and slice barely pulled out, 3D stack of four musket balls.

### 0.9.7 (2026-11-03, archived)
- Wings angled inward, longer trouser legs, solid bread loaf with thin cuts, more realistic cheese wheel (rind, holes in wheel and slice), thicker sun/snowflake with a thin gap, pile of musket balls.

### 0.9.6 (2026-11-03, archived)
- Wings (side by side), full-length trousers without ruffles, bread cuts filled, 3D cheese wheel with slice, larger sun ring with 4-arm snowflake, three separate musket balls. Boxer briefs and honeycomb reverted to the earlier open icons.

### 0.9.5 (2026-11-03, archived)
- Revisions after review: cuisses (thigh plates), rounded pouch/satchel, trousers without ruffles, boxer briefs, straightened crown, mirrored heels and scalpel, crab mouth removed, rounder bread, cheese wheel, tilted fish, simpler honeycomb with drips, closer antlers and claws, fork and knife only, smaller sandwich with motion lines, detailed sun/snowflake, instincts eye recentred, waterskins at 1/3 and 2/3, musket balls, longer kunai handle.

### 0.9.4 (2026-11-03, archived)
- Open-licence icons, second pass: 24 direct picks (rotated/mirrored where needed) and 14 icons derived from open ones (horns, antlers, bones, pelvis, claws, tusk, pistol, kunai, card, inkwell, bandana, inverted eyepatch, sun/snowflake, chat bubble). 38 more icons; 127 of the original 286 replaced so far.
- Weapons use the shared grey where requested; credits updated.

### 0.9.3 (2026-11-03, archived)
- First open-licence icon pass: 89 icons (and their light/heavy/cloth and colour variants, 138 files) swapped from AIT/THICC/BOOBIES artwork to game-icons.net (CC BY 3.0) and Material Design Icons (Apache 2.0). Credits in OPEN_ICON_CREDITS.txt.
- About 197 borrowed icons are still to be replaced before 1.0.0.

## 0.9.2 (2026-11-03)
- Active Effects: icon for every lasting effect by type (stats, regen, resists, skills, cloaks, summons, shouts, ...) from all plugins; about 5,900 effects. Gear enchantments and abilities included.
- Light and Slow Time effect icons replaced (the PNGII ones were hearts).
- Renamed to DICK - Dark's Icon & Category Kit.

## 0.9.1 (2026-11-03)
- Every Ordinator perk effect uses its skill icon.
- Real dragon claws gold, replicas white; backpack icon restored (pouch rules were overriding it).
- Tool weapons (pickaxe, wood axe, fishing rod, tool knife) sort at the bottom of Weapons; sickles, scythes and hammers stay weapons.
- Pickaxe uses the SkyUI icon again.
- Stub icon file `Interface/DICK/icons.swf` so the inventory injector applies icon labels without the old packs.

## 0.9.0 (2026-11-02)
- Standalone: sorting and icon rules of AIT, THICC and BOOBIES folded in (`DICK.json`, `DICK.esp`, `DICK_english.txt`, SkyUI config), so those mods can be removed.
- Deity, skill-badge and Active Effects icons added.
