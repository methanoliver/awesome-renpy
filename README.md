# Awesome RenPy [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome goodies for [RenPy](https://renpy.org/) visual novel engine. Originally this started as me dumping my bookmark folder, but since this accrued some interest, I decided to make this more of a thing.

Who am I kidding, this will languish in obscurity like every other attempt to produce an index of these things...

## Contents

+ [Tutorials](#tutorials)
+ [Frameworks](#frameworks)
+ [Assets](#assets)

## Tutorials

RenPy's own documentation is somewhat scattered, at times incomplete, and often, insufficiently detailed.

+ [Lezcave](https://www.lezcave.com/renpy-tutorials/) - A set of basic tutorials
+ [Feniks Development](https://feniksdev.com/navigation/) - In-depth explanations of basic programming notions as they relate to RenPy.

## Frameworks

Pieces of code big enough to be called full-blown libraries.

+ [Lezinventory](https://www.lezcave.com/lezinventory-framework/) - General purpose inventory system.
+ [Pink Engine](https://pink-productions.itch.io/pink-engine) - Tiled map framework.
+ [RPG Battle Engine](https://github.com/Habitacle/battle-engine) - What it says on the tin.
+ [Static chessboard displayable](https://github.com/RuolinZheng08/renpy-static-chessboard) - What it says on the tin. Can be used to produce a [full AI-run chess game](https://github.com/RuolinZheng08/renpy-chess).
+ [RADC](https://github.com/CharlieFuu69/RenPy_Asset_Download_Complement) - A framework to enable a RenPy project to download its own DLC. Documentation in Spanish only.
+ [DynamicSpriteManager](https://github.com/alexkrob/dynamicsprites/) - A high-level system for easily defining and compiling the RenPy native LayeredImage. Given a directory of images, it will automatically scan and categorize those images for use in a mix-and-match style sprite declaration language based on filenames. Documentation inline with code.
+ [Speech Bubbles](https://github.com/RenpyRemix/speech-bubbles) - A unique look presenting novel text as speech bubbles.
+ [Console](https://github.com/abduelhamit/renpy-ingame-console/) - An in-game console for the player to use (i.e. distinct from the built-in developer console). Not well documented at all.
+ [AliceOS](https://github.com/ProjectAliceDev/aliceos) - What is this I don't even.
+ [Messenger Emulator](https://github.com/sDextra/messenger-emulator) - An advanced library for imitating Telegram Messenger in-game. Requires work to adapt to more modern versions of RenPy.

## Tools

### Developer tools

These are meant to be built into the game at least during development, and thus are a cross between libraries and standalone tools.

+ [Ren'Edit](https://minute.itch.io/renedit) - A beta-tester support tool to easily acquire corrections and comments.
+ [ActionEditor](https://github.com/kyouryuukunn/renpy-ActionEditor3) - A powerful director tool for manipulating [camera](https://www.renpy.org/doc/html/model.html) and viewing the results.
+ [MouseFinderTool](https://github.com/CharlieFuu69/RenPy_MouseFinderTool) - A set of developer tools to pinpoint mouse position of things. Documentation in Spanish only.

### Standalone developer tools

These are software unto themselves.

+ [renpy2linux](https://github.com/Shizmob/renpy2linux) - A script to convert Ren'Py releases to Windows, OSX and Linux-compatible ones, when the only thing you have is one of the three. Requires Linux or OSX to work.
+ [renpy-graphviz](https://github.com/EwenQuim/renpy-graphviz) - Draws a flowchart of a RenPy project based on jumps, calls and labels. Has an online version.
+ [renkit](https://github.com/kobaltcore/renkit) - A toolkit for managing Ren'Py instances via the command line, intended for build automation and continuous integration.
+ [renpydeskgen](https://github.com/Polymehr/renpydeskgen) - Shell script to generate Linux `*.desktop` files for RenPy games.
+ [unrpyc](https://github.com/CensoredUsername/unrpyc) - The `*.rpyc` file decompiler.
+ [unrpa](https://github.com/Lattyware/unrpa) - The most famous RPA archive extractor.
+ [rpatool](https://github.com/Shizmob/rpatool) - The less famous RPA archive extractor.

### End-user tools

These tools are made for end-users, rather than developers.

+ [Translator3000](https://github.com/NyashniyVladya/Translator3000) - Runs RenPy games through automated translation. Trial version.

## Assets

No visual novel is complete without artwork and sound. Beware and carefully observe the license terms!

### Asset libraries

+ [Itch.io](https://itch.io/game-assets/genre-visual-novel) - Visual novel specific assets available on Itch.io.
+ [Pixabay](https://pixabay.com/) - a variety of Creative Commons images, videos, music and sound effects.
+ [Free Music Archive](https://freemusicarchive.org/) - Royalty-free and CC music.
+ [OpenGameArt](https://opengameart.org/) - assets for a variety of game types, many useful for visual novels.
+ [FreeSound](https://freesound.org/) - major source of free sounds of every description.
+ [Incompetech](https://incompetech.com/music/royalty-free/music.html) - Kevin MacLeod's music. *Everyone* has heard it.
+ [SoundBible](https://soundbible.com/) - A collection of sound effects.
+ [Soundimage](https://soundimage.org/) - Specially aimed at game developers.
+ [FreePD](https://freepd.com/) - Music
+ [FontSquirrel](https://www.fontsquirrel.com/) - Free TTF/OTF fonts.

### Asset generators

#### Sound generators

+ [ChipTone](https://sfbgames.itch.io/chiptone) - online generator.
+ [FxTone](https://raylibtech.itch.io/rfxgen) - online generator.
+ [LabChirp](https://labbed.itch.io/labchirp)

#### Character sprite generators

+ [Sutemo's Character Creator](https://emily2.itch.io/sutemo)
+ [Mannequin](https://ar14.itch.io/mannequin) - free and paid versions

#### Other generators

+ [TextureLab](https://njbrown.itch.io/texturelab) - Procedural texture generator.
+ [Procgen Arcana](https://watabou.github.io/) - A collection of generators intended primarily for tabletop roleplaying which produce useful maps.

#### AI-powered generators

Most of these are only useful to produce background images, as getting the detail and specificity required of anything else out of them is impossible. But free backgrounds are free backgrounds.

+ [ArtBreeder](https://www.artbreeder.com/)
+ [DreamStutio](https://beta.dreamstudio.ai/)

### Asset editing tools

+ [Krita](https://krita.org/) - The best open source paint program.
  + [Generate Ren'Py Scripting](https://github.com/SeanHRN/generate-renpy-scripting) - A plugin for Krita, outputs a block of Ren'Py script to display the images of the active Krita document as they appear on the canvas, working in tandem with the [krita-batch-exporter](https://github.com/GDQuest/krita-batch-exporter).
+ [GIMP](https://www.gimp.org/) - The more arcane and ancient, but likewise powerful open source paint program.
+ [Audacity](https://www.audacityteam.org/) - Open source audio editor.
+ [Ocenaudio](https://www.ocenaudio.com/en/) - Less powerful, but more convenient, free (as in beer) audio editor.
+ [FFMpeg](https://ffmpeg.org/) - the Swiss army knife of video and audio format conversion and filtering.
+ [IMGOnline.com.ua](https://www.imgonline.com.ua/eng/) - a collection of online texture processing tools.
+ [Waifu2X](https://waifu2x.booru.pics/) - AI-based image upscaler.
+ [FotoSkether](https://fotosketcher.com/) - The better way of making photos look like painting. Windows-only, runs under Wine.

## Other Awesome Lists

Other amazingly awesome lists can be found in [awesome](https://github.com/sindresorhus/awesome), [awesome-awesome](https://github.com/emijrp/awesome-awesome) and [awesome-awesomeness](https://github.com/bayandin/awesome-awesomeness). Of particular note for RenPy users should be [awesome-python](https://github.com/vinta/awesome-python) and [awesome-glsl](https://github.com/vanrez-nez/awesome-glsl).
