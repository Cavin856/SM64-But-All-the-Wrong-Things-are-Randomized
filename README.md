This is Super Mario 64 - But All the Wrong Things are Randomized
AKA Cursed SM64 Randomizer
Made by Cavin856



I know this is a wall of text, but please read it anyway, or at the very least, everything from the asterisks down.



Originally made in 2024, released for April Fool's 2025, I had planned to do more with this, but lost interest after taking about an 8 month break.
Part of the reason for losing interest was that I started working on other projects,
but also, the code for this project, as it become increasingly clear, was not organized in an effecient way.
It had started to become function spaghetti that I didn't want to re-learn months later after forgetting how I laid everything out.
Additionally, I had since learned much better ways to organize my code, and did not want to work under my old, ineffecient, system, nor painfully update it.

How this rando works is: every time you re-enter a course, it re-randomizes all randomizes relating to that course.
There is no "logic" because this rando doesn't shuffle items around like traditional metroidvania randomizes etc.
It just applies silly and sometimes interesting effects to the levels.
More of an experiment anyway, I learned a lot about SM64 while making this, and also about MIPS Assembly.
If a star is impossible (which on rare cases may be), just keep reloading the level until it's doable, hopefully.
Hopefully past-me was diligent enough to ensure that every star can eventually be doable, as I have not bothered to check now, in 2025.

Additionally, a buddy of mine ended up spreading word about this hack back when I was developing it and generating a fairly surprising amount of hype for it.
To everyone who may have been waiting for something far grander than this for about a year now, I'm sorry.
I'm sorry that this wasn't as elaborate as you, or even I, may have envisioned.
Sometimes this happens with game development, projects get scrapped or modified or remade or delayed,
which is why I don't like sharing anything about my hacks publically, especially so easrly in development.
Unfortunately, my buddy did not realize this, and shared information about it anyway.
I don't blame him though, and I ask that if you heard about it through him, that you don't blame him either.
The fault is on me for sharing in-progress videos of some of the cooler randos.
I was so hyped that I wanted to share it and didn't consider the possible consequences.



************** READ THIS AT THE VERY LEAST **************

That being said, this was still unfinished, as mentioned above, but I don't feel like "finishing" it though, as this was a meme hack anyway.
Most every main course as a special rando.
Some are unique to that course, whereas others are generic enough that they can be applied to any course in the config file.
Originally, I wanted to have multiple presets for different skill-levels of SM64,
but since this hack never got completely finished and I just want to release it, I've turned up all the settings to a somewhat advanced level.
You can also adjust the config file and then apply it using Armips to customize what you do and do not want enabled.
Do not re-order any of the lines in the config file that you apply, otherwise it will break.
The config file just writes hard-coded variables into the rom itself, and so changing the order of those variables will break things.

Regarding the randomizes themselves, I think it's best experienced yourself, blind.
It should be noted, however, that the following areas do not have unique randomizers:

SSL Pyramid, the Castle, and all Side Courses.
(Additonally, LLL did not have it's own rando, so I gave it the same generic rando that WF had)

I had wanted to add randomizers to those areas too, but never got around to it.
Additionally, not every randomizer is great, or even super noticable.
Some randos you may actively hate instead (DDD was a terrible idea).
My favourite by far is BBH's rando.

Thank you for trying out this test hack of mine,
- Cavin856



~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
(Technical stuff below, you can skip this if you don't care about the coding side of this)

This was done in an un-extended romfile, and indeed you can theoretically download all the code files yourself and make the patch yourself if you wanted.
The code files can be found on my github here:

https://github.com/Cavin856?tab=repositories

This was done entirely with MIPS Assembly using the SM64 Decomp as reference only.

The code isn't organized great, and back then I fell into the bad habbit of sorting code by code type, rather than topic.
This results in all of the hardcoded hooks and edits being segregated to their own file, which is a terrible mistake.
Several closely related functions are in different code files, and some files contain several completely unrelated functions.
Additionally, my label prefixes weren't great back then, and I didn't use enough comments to explain how functions worked.
This all caused the code to be very annoying to follow. Not as bad as some earlier scrapped projects, but still not great.
There were several shortcuts and better ways to code some of these functions for clarity too.
All in all, this was an excellent learning experience, but compared to what I know now, this was kind of brute-forcey and primative.

Feel free to use any of this code in your own hack projects.
Just be sure to add me to the credits if you do.
