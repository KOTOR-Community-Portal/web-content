# General Questions

## FAQs for New Players

### What's different between KOTOR and KOTOR 2?

KotOR and KotOR 2 are very similar. With respect to mechanics, KotOR 2 introduced an influence system, a slightly advanced crafting system, some new feats and Force powers, and lightsaber & Force forms. In regards to plot, KotOR 2 presents an overall darker story compared to the story of KotOR, which is more reminiscent of a traditional Star Wars movie.

KOTOR 2's influence system causes certain actions and dialogue options to gain or lose influence with certain party members. With a high influence rating, a party member's alignment will more closely match your player character's alignment, while a low influence rating will cause the character to shift to the opposite of your player character's alignment. If the influence value is either high or low enough, party members will share information about their background, and some party members may get bonuses or access to new classes.

The crafting system in KotOR 2 allows you to create parts to upgrade your weapons and armor, rather than relying on finding them throughout the game as was the case with KotOR. The parts you're able to create are based on your own or your party members' skills (e.g., Computer Use, Demolitions, and Repair). You can also break items in your inventory down into generic components that are used to create the aforementioned parts. The variety of parts allows a weapon (and therefore its user) to specialize in various different playstyles—for example, some parts increase the critical threat range while others provide attack bonuses.

There are various new feats and Force powers in KotOR 2. Of particular note are the Cross-Class Skill feats. These feats allow the player to take a skill that normally requires two skill points to level up and convert it to a class skill, which only takes a single skill point to level up. There are also advanced forms of some feat trees when you reach a prestige class later in the game.

The lightsaber and Force forms that your player character can learn allow you to modify your bonuses and penalties as combat situations change. For example, the Ataru lightsaber form gives you a defense bonus against a single target, but lowers your defense against all other targets and makes your more susceptible to blaster fire. The Force Channel form grants you a bonus to Force point regeneration outside of combat, increases the damage of your Force powers, and grants you a bonus to saving throws against Force powers. There are 7 lightsaber forms and 4 Force forms.

KOTOR 2 also effectively lacks a level cap (having a level cap of 50, which is impossible to reach without a modded game or resorting to cheating/savegame editing), whereas the original KOTOR has a hard level cap of 20.

___

### Can I get away with playing KOTOR 2 before I play the original KOTOR?

It's possible, although not recommended. Both games introduce unique characters, weapons and environments, and KotOR II lays out the basics of what happened in the first KotOR game. Despite this, however, the background behind events in the second game is intimately tied to events that are either first discussed in or actually happen in the first game, and while it's easy for a user playing KotOR II first to learn the basics of the galactic situation, there's no way to know the ins-and-outs of it without playing the games in release order. That was very much the way that they were designed to be played.

___

### What's the combat system of the KOTOR games like?

Both KOTOR and KOTOR 2 utilize a d20 rolling system originating in Dungeons & Dragons and used by games like Baldur's Gate, Planescape, and Neverwinter Nights. Essentially, for each action the computer rolls a twenty-sided die, which must hit above a certain number in order to succeed. This roll is modified by various equipment and stat bonuses possessed by both you and your enemy, and are better explained in other sections. These rolls determine anything from successfully hitting an opponent, to unlocking a door, to determining the effectiveness of your force powers. The specific data for each roll can be viewed from the "Message Log" menu.

## Setup Help

### Can my system handle the KOTOR games?

According to Steam the system requirements are as follows:

Hardware|Model/Value
:-:|:-- 
OS|Windows XP and Windows Vista 
Processor| Intel Pentium 3 1Ghz or AMD Athlon 1GHz 
Memory| 256 RAM 
Graphics| 32 MB with Hardware T&L 
DirectX| Directx 9.0b or better 
Hard Drive| 3.5 GB 
Sound| Directx 9.0b compatible 

KotOR is quite an old game, though, an therefore may sometimes have trouble running on modern machines even if your system technically meets the specifications. If you have problems with *crashes specifically*, the four most common culprits are:

* an operating system newer than Windows XP, in which case downloading [this .dll file](https://web.archive.org/web/20160108035406/http://www.gamefront.com/files/9398284/TSL_Windows_Vista_Fix) and placing it in your game directory may help

* an issue with graphics rendering, which can often be solved by disabling grass, soft shadows, or vertex buffer effects

* an issue with playing the game at a resolution smaller than your monitor's native resolution—see [here](/faq/k1.html#My_game_is_crashing_before/shortly_after_the_main_menu,_or_whenever_I_have_a_cutscene!) for how to solve this for KOTOR, and [here](/faq/k2.html#My_game_is_crashing_before/shortly_after_the_main_menu,_or_whenever_I_have_a_cutscene!) for KOTOR 2

* playing on a laptop or other system with an integrated graphics card, which can unfortunately (though not always) result in irreparable problems which no known method can get around; we recommend ensuring the platform you buy your games on has a refund policy if you do choose to try playing on a laptop

This list is meant to help provide a shorthand of things to try for users who purchase the game and experience immediate or near-immediate problems, *not* to be exhaustive; we can probably help even if your issue isn't on here! If you're having other problems, please check the FAQ sections for your specific game ([KOTOR](/faq/k1.html) or [KOTOR 2](/faq/k2.html)) first, but if there's nothing there to address your specific problem please hop into the #tech_support channel of the [KOTOR Discord](https://discord.gg/kotor) and let us know your problem! Nine times out of ten, we can find at least a partial solution for you.

## Mod Support

### How does KOTOR modding work?

There are two basic ways mods will interact with KOTOR: *file addition* and *TSLPatcher installers*.

* File addition is the most basic, and therefore most common, modding system. By creating a folder called "override" in your main game directory, files from mods can be placed directly into the folder, which will instruct the game to utilize these modified files over the basegame files of the same name. This has implications for compatibility, however, since any files of the same name included in other mods will force you to choose one over the other, perhaps with game-breaking consequences. Installing mods in this manner can also rapidly grow out-of-hand—it's difficult to track what files came from where when you have 4,000 in your override folder.

* TSLPatcher installs are not inherently more advanced, but do have the capacity to be. The TSLPatcher is a utility which modders can set up to install their mods for them, and in the case of mods which utilize the TSLPatcher the .exe will come pre-packaged with the mod in question. The TSLPatcher allows for the easy installation of more complex mods which make use of file installations to other directories (such as modules or movies), as well as having the functionality to append changes to files in the override, *de facto* allowing mods which would typically be incompatible with one another to be installed and function normally, since the file isn't being overwritten like it would be with the file addition method. The TSLPatcher isn't a ward against everything going wrong, however, because for it to function properly the modder who set it up must have taken the time to ensure all their edits were made properly and in the most compatible format possible, which isn't always the case. Still, a TSLPatcher install is more likely to be compatible than a file addition 100% of the time, and also has helpful installation feedback built into the .exe, so you can track problems if they do occur.

___

### I want to request/try to create a mod, what do I need to do?

You can sign up on [Deadly Stream](https://deadlystream.com). The forums have a Request section for requesting a mod, and there is a tutorial section with some info to help those aspiring to create a mod of their own. Also, there is a Modding Toolset section in the Downloads.

If you need any help with modding, you can post a thread asking for help, explaining what you have, and trying to explain what you need. Most of the time others will help teach you as best they can, provided you're polite and patient.

___

### This site's mod build has quite a lot of mods. Is there somewhere I can download and install them all at once?

In short, no. As a common courtesy and to comply with our partner site Deadlystream's rules, we strictly require a mod author's permission to have their content included in a mod package. Due to the sheer number of various mod creators whose mods are included in the build, this would be impractical at best, impossible realistically. If you want to use the builds but don't want to take the time to install all of the mods individually, this is why the Category and Tier system are present: to help you find & install the mods you feel are most important to enhancing your experience.
