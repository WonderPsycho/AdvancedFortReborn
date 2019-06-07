This is the readme document for the Spellcrafts mod, by Eric Blank.

Credits:
Eric Blank - I did lots of typing and copy/pasting. At least some of the ideas I generated of my own accord, even if they aren't entirely original.
Putnam - I like his solutions to problems so much I implement them occasionally if I hit a roadblock.
Gizogin - who posted the ice spike spell that I used to help me understand other parts of the interaction system, and is still included.
With ideas shamelessly stolen from; everyone who dares to post on the bay12forums, popular culture, and mythology.
Help catching bugs and such from: gnome, Nahere and hertggf

Short summary:
This mod adds various night creatures, secrets, and ways to learn "magic" through interactions, reactions and syndromes in Dwarf Fortress. The player can learn magic in both fortress and adventure modes, through multiple means. The mod is intended to be compatible with vanilla DF and other lightweight mods which dont change many of the basic game's files. As such it is intended to run off of the vanilla DF files and does not modify them.


Installation:

Extract the contents of the zip file directly into the game's raw/objects folder. If you have an unmodified, vanilla entity_default.txt, you can simply copy the entity_default.txt in the same folder as this readme into the objects folder to override the base game and allow dwarves and humans to develop magic. If you do not have a vanilla entity_default.txt, you can copy/paste the following into the entity definitions for MOUNTAIN and PLAINS:





	[PERMITTED_JOB:ALCHEMIST]
	[PERMITTED_BUILDING:SPELL_MAGIC_STUDY]
	[PERMITTED_BUILDING:SPELL_CONJURE_CIRCLE]
	[PERMITTED_BUILDING:SPELL_HOLY_ALTAR]
	[PERMITTED_REACTION:SPELL_HOLY_ALTAR_PRAY_NO_SACRIFICE]
	[PERMITTED_REACTION:SPELL_HOLY_ALTAR_SACRIFICE_FOOD]
	[PERMITTED_REACTION:SPELL_HOLY_ALTAR_SACRIFICE_GOLD]

	[PERMITTED_REACTION:SPELL_INSCRIBE_SLATE_SIMPLE_FORT]
	[PERMITTED_REACTION:SPELL_LEARN_MAGIC_GENERAL_ALL_FORT]
	[PERMITTED_REACTION:SPELL_LEARN_MAGIC_AETHERIAL_FORT]
	[PERMITTED_REACTION:SPELL_LEARN_MAGIC_HYAZITH_FORT]
	[PERMITTED_REACTION:SPELL_LEARN_MAGIC_POLYBESTIA_FORT]
	[PERMITTED_REACTION:SPELL_LEARN_MAGIC_MEDISEPHOS_FORT]

	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_WOOD_GEM_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_COAL_GEM_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_COAL_METAL_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_WOOD_BARS_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_BONE_BARS_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_WOOD_BONE_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_BONE_GEM_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_BLOOD_GEM_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_VERMIN_PET_GEM_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_VERMIN_WILD_GEM_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_VERMIN_DEAD_GEM_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_FISH_GEM_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_FISH_RAW_GEM_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_CORPSE_GEM_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_PLANT_GEM_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_FRUIT_GEM_FORT]
	[PERMITTED_REACTION:SPELL_MAKE_AETHER_SALT_SEED_GEM_FORT]

	[PERMITTED_REACTION:SPELL_CONJURE_CREATURES_MISC]
	[PERMITTED_REACTION:SPELL_CONJURE_EXCHANGE_AETHER]
	[PERMITTED_REACTION:SPELL_CREATE_WOOD]
	[PERMITTED_REACTION:SPELL_CREATE_OBSIDIAN]
	[PERMITTED_REACTION:SPELL_CREATE_LIMESTONE]
	[PERMITTED_REACTION:SPELL_CREATE_MAGIC_CHEESE]
	[PERMITTED_REACTION:SPELL_CREATE_MAGIC_MEAT]
	[PERMITTED_REACTION:SPELL_CREATE_MAGIC_MEAD]
	[PERMITTED_REACTION:SPELL_CREATE_MAGIC_LEATHER]
	[PERMITTED_REACTION:SPELL_CREATE_MAGIC_THREAD]
	[PERMITTED_REACTION:SPELL_CREATE_MAGIC_CLOTH]
	[PERMITTED_REACTION:SPELL_CREATE_MAGIC_SAND]
	[PERMITTED_REACTION:SPELL_CREATE_MAGIC_BARS]

	[TOOL:ITEM_TOOL_BOOK_MAGIC]
	[TOOL:ITEM_TOOL_ATHAME_HYAZITH]
	[ARMOR:ITEM_ARMOR_BEAST_RUNE:COMMON]
	[ARMOR:ITEM_ARMOR_AETHER_FOCUS:COMMON]
	[ARMOR:ITEM_ARMOR_AMULET_MEDISEPHOS:COMMON]
	[PERMITTED_REACTION:SPELL_ENCHANTED_IRON_MAKING]
	[PERMITTED_REACTION:SPELL_CREATE_RESIDUE]
	[PERMITTED_REACTION:SPELL_REDUCE_RESIDUE]



This will make the magic studying mechanic available in fortress mode, and allow spellbooks to appear in bags of junk in adventure mode. You can also paste that in the definitions of any modded entities you have. Even without doing that, the magic effects will be available to a clan of dwarvish wizards that will appear in your world and can be played as a fortress or adventurer. Their noble positions are different from the mountain dwarves but should be playable. Keep in mind that these changes don't take effect until you generate a new world.


Directions on how to get started in adventure mode:
You'll first want to find or make a slate. There is a reaction to produce one under the spellcrafts - items menu.
You will then want to make aether salts. There is a menu for these that includes many different reactions depending on what components you have available.
There is also a reaction to produce rough gems which are one of the common components in making aether salt.
Once you have both aether salts and a slate, you can perform the "study magic in general" reaction under the same category. This will consume the aether salts, not the slate, and has a fair chance to produce one or more of the essences of spells.
Eat the essences to gain their respective spells.
In the process of producing these essences though there is a much smaller chance of generating a "magic aura" which will vaporize instantly upon performing any action. If you're quick, you can throw these away from you and they will vaporize where they land. If not, there is a chance you will inhale their vapors and be afflicted by their syndromes. These should not be fatal, but they can be a nuissence. If you have high disease resistance, your chances of being affected are greatly reduced.
There is also a spell specifically for increasing your disease resistance attribute. This should help protect you further. If you search in piles of loot or warehouses you can also find an aether focuser, which is used to study aetherial magic, the first school available.
Other schools will exist and ritual items for them also must be acquired.

Fortress mode is much the same:
Your dwarves can produce a slate tool from any hard material such as stone or wood, and build a magician's studio
in the magicians studio you have access to more or less all the same reactions you do in adventure mode.
Only dwarves with the alchemy labor enabled will perform these reactions.
The essences produced can be stored in food stockpiles under the "plant cheese" category.
Essences dont rot, but can be eaten by vermin, so it is advised that whatever stockpile they're to be stored in is protected by at least one cat (or other vermin-hunting critter)
Any dwarves could end up eating your essences. If this is a problem, you can store them in a locked room and drop them onto the stockpile from above by dumping 
them or something. Then only allow dwarves you want to be able to perform these spells in. The essence being a food item also allows you to control which essences dwarves are allowed to eat. You can forbid or dispose of any that you dont want dwarves consuming, for instance restricting any fire spells.

In either mode, you also have the choice to conjure items by using an aether salt component. These include basic materials and food products.

If you have questions, comments, or bugs to report, post in the bay12forums thread and I'll get back to you as soon as possible:
http://www.bay12forums.com/smf/index.php?topic=149426.0