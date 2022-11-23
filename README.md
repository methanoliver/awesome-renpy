# Awesome RenPy [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome goodies for [RenPy](https://renpy.org/) visual novel engine. Originally this started as me dumping my bookmark folder, but since this accrued some interest, I decided to make this more of a thing. Things that were known to be obsolete at the time of writing -- which happens relatively often in the RenPy land -- did not make it into this list unless they were otherwise significant or were the only example of their kind.

Who am I kidding, this will languish in obscurity like every other attempt to produce an index of these things...

## Contents

+ [Documentation](#documentation)
  + [Introductory](#introductory)
  + [Python](#python)
  + [Specific](#specific)
  + [Non-English documentation](#non-english-documentation)
  + [Patreon articles](#patreon-articles)
    + [Internals](#internals)
    + [Features](#features)
      + [Menus](#menus)
    + [Platform support details](#platform-support-details)
    + [Interoperability](#interoperability)
    + [Examples](#examples)
+ [Project templates](#project-templates)
+ [Frameworks](#frameworks)
  + [General](#general)
  + [Network](#network)
  + [Visual novel elements](#visual-novel-elements)
  + [Gameplay elements](#gameplay-elements)
  + [Device imitation](#device-imitation)
  + [Extra content](#extra-content)
+ [Cookbook](#cookbook)
  + [Snippets](#snippets)
    + [Text](#text)
    + [Effects](#effects)
    + [Particles](#particles)
    + [Displayables](#displayables)
    + [User interface](#user-interface)
    + [Other snippets](#other-snippets)
  + [Minigames](#minigames)
  + [Shaders](#shaders)
  + [Code examples](#code-examples)
  + [Other](#other)
+ [Tools](#tools)
  + [In-engine developer tools](#in-engine-developer-tools)
  + [Standalone developer tools](#standalone-developer-tools)
    + [General](#general-1)
    + [Continuous integration](#continuous-integration)
    + [Unpacking and decompilation](#unpacking-and-decompilation)
    + [Conversion](#conversion)
  + [End-user tools](#end-user-tools)
+ [Assets](#assets)
  + [Asset libraries](#asset-libraries)
    + [Fonts](#fonts)
    + [Individual libre artists](#individual-libre-artists)
  + [Asset generators](#asset-generators)
  + [Asset editing tools](#asset-editing-tools)
    + [Graphics](#graphics)
    + [Sound](#sound)
    + [Video](#video)
+ [Support](#support)

## Documentation

[RenPy's own documentation](https://www.renpy.org/doc/html/index.html) is somewhat scattered, at times incomplete, and often, insufficiently detailed.

That is, of course, no excuse not to read it, but if that was not helpful:

### Introductory

+ [Lezcave](https://www.lezcave.com/renpy-tutorials/) - A set of basic tutorials
+ [VNCoder](https://vncoder.dev/) - Another set of basic tutorials.
+ [Working with RenPy](https://videlais.com/2018/06/28/working-with-renpy-part-1-downloading-and-configuring/) - Almost a book, walking through much of the basics.

### Python

+ [Feniks Development](https://feniksdev.com/navigation/) - In-depth explanations of basic programming notions as they relate to RenPy.
+ [Python Tips](https://book.pythontips.com/en/latest/index.html) - While not specifically RenPy related, so a number of sections dealing with the operating environment are not relevant, this book will aid people who already know the very basics of Python.
+ [getting your head around Ren'py: for coders](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=39572#p422964) - Explains the unusual things about RenPy for people with experience of more regular programming languages.
+ [Free Python Books](https://github.com/pamoroso/free-python-books) - A list of Python books in English that are free to read online or download.

### Specific

+ [Ren'Py Tutorial - LayeredImage](https://tofurocks.itch.io/renpytut-layeredimage) - Complexities of `layeredimage` by example.
+ [Reading Screen Language Documentation](https://github.com/jbondguy007/reading-renpy-screens-docs) - A treatise on understanding screen language documentation.
+ [Implementing Translations](https://mysterycorgi.itch.io/renpy-tips/devlog/74300/implementing-translations) - Detailed explanation of how to translate a project into multiple languages.
+ [Ren'Py Visual Novels on Steam Guide](https://docs.google.com/document/d/1La4Pg72Wzpo1cPFFPk_g8Wjkl-MwLG2Qunwu65Ovl5w/edit) - A comprehensive guide with screenshots for getting your Ren’Py based game onto Steam.

### Non-English documentation

+ [RenPy for Dummies](https://renpyfordummies.blogspot.com/) - A Russian-language blog full of cookbook examples.
+ [Энциклопедия Ren'Py](http://ru.renpypedia.shoutwiki.com/) - Russian-language RenPy wiki.

### Patreon articles

These are articles from [PyTom's Patreon](https://patreon.renpy.org/), most of which explain a certain feature in more detail than the manual does and provide example code.

#### Internals

Explain certain obscure, but sometimes critical implementation details.

+ [Under the Hood: Interactions](https://patreon.renpy.org/interaction.html) - the only explanation of what an "interaction" is.
+ [What is a context?](https://patreon.renpy.org/dev-2019-12.html#extra-what-s-a-context) - A more in-depth explanation of what a context is.
+ [Porting your game to Python 3](https://patreon.renpy.org/dev-2021-12.html#porting-your-game-to-python-3) - Some detail on what exactly is different between the 7.5 and 8.0 branches of RenPy and how to switch over.
+ [Under the Hood: .rpyc files](https://patreon.renpy.org/rpyc.html) - Describes the internals of an `.rpyc` file and their use.
+ [Save Compatibility Through Repeated Releases
](https://patreon.renpy.org/dev-2021-02.html#save-compatibility-through-repeated-releases)
+ [Avoiding Framerate Glitches Caused By Image Prediction](https://patreon.renpy.org/framerate-stability.html)

#### Features

Explanations on the use of a particular feature.

+ [Character Customization](https://patreon.renpy.org/character-customization.html) - Using character objects to apply textbox customizations.
+ [Multiple Dialogue Blocks](https://patreon.renpy.org/multiple-dialogue.html)
+ [Save Metadata](https://patreon.renpy.org/save-metadata.html) - How to get your save/load screen to display more in-depth information about a save than it normally can.
+ [Decorators and gui.variant](https://patreon.renpy.org/dev-2021-11.html#decorators-and-gui-variant) - On the proper usage of `renpy.variant`.
+ [Adjust Attribute Example](https://patreon.renpy.org/dev-2021-04.html#adjust-attribute-example) - How to use `config.adjust_attributes` and whether you need to.
+ [Pausing movies](https://patreon.renpy.org/dev-2021-07.html#pausing-movies) - How to pause movies and music.
+ [Save on Quit](https://patreon.renpy.org/save-on-quit.html) - One of the actually numerous ways to automatically save on quit.
+ [Layered Image Conversion](https://patreon.renpy.org/layeredimage-conversion.html) - Converting to use `LayeredImage` from the obsolete technique of using `Composite`/`LiveComposite`.

##### Menus

`menu:` statement has a lot more flexibility than you would think.
 
+ [Timed Choice Menus](https://patreon.renpy.org/timed-choice-menus.html) - How to make a choice menu that can time out.
+ [Shuffling choice menus](https://patreon.renpy.org/shuffle-menu.html) - Shuffling items in the menu.
+ [Menu Arguments Cookbook](https://patreon.renpy.org/menu-arguments.html) - More advanced examples on using menus.
+ [Very Old Features](https://patreon.renpy.org/very-old-features.html) - Three rarely used features - menu labels, menu sets and gameplay timer.
+ [Menu blurring](https://patreon.renpy.org/dev-2020-09.html#menu-blurring) - An example of overriding the built-in menu system to blur the image behind the menu buttons.

#### Platform support details

Details on what you need to do to get your project to run on a particular platform.

+ [Android Adaptive Icons in Ren’Py](https://patreon.renpy.org/android-icons.html)
+ [Notarizing Mac Applications](https://patreon.renpy.org/macos-notarization.html#notarizing-mac-applications) - How to notarize your OSX releases.
+ [Steam Deck Guide](https://github.com/renpy/steam-deck-guide) - How to get your project to pass Steam Deck compatibility review.

#### Interoperability

Interoperability with the rest of the world.

+ [Requests](https://patreon.renpy.org/dev-2020-11.html#requests) - Using the bundled [requests](https://requests.readthedocs.io/en/latest/) Python library to, among other things, save data to a Google Sheet. For the record, the bundled version in 8.0.3 is 2.20.0
+ [News From Your Website](https://patreon.renpy.org/news.html) - Making HTTP requests from RenPy in examples.
+ [Adding Google Analytics to Your Visual Novel](https://patreon.renpy.org/analytics.html) - See also the updated script in a [later Patreon post](https://patreon.renpy.org/dev-2021-03.html#analytics).

#### Examples

Code examples implementing a particular feature.

+ [Automatic speech bubbles](https://patreon.renpy.org/speech-bubbles.html) - A simpler take on speech bubbles than the Speech Bubbles framework.
+ [Three Creator Defined Statements](https://patreon.renpy.org/three-creator-defined-statements.html)
+ [Drop Down Menus](https://patreon.renpy.org/dev-2022-05.html#drop-down-menus) - How to make drop-down menus.
+ [Multi-Key](https://patreon.renpy.org/dev-2022-04.html#multi-key) - Reacting to multiple keys pressed simultaneously.
+ [Marquee](https://patreon.renpy.org/dev-2021-11.html#marquee) - How to make text that scrolls back and forth if it's longer than the area allocated to it.
+ [MultipleCallback](https://patreon.renpy.org/dev-2020-03.html#multiple-callbacks) - Example of how to use configuration variables that only permit one callback function to call multiple functions anyway.
+ [Label log](https://patreon.renpy.org/dev-2020-02.html#label-log) - Example of using `config.label_callback`.
+ [Flashing Messages on the Main Menu](https://patreon.renpy.org/dev-2020-01.html#visual-conference) - Example of how to draw attention to new menu items by making them flash until investigated.
+ [Checking for Changes and Displaying A Message
](https://patreon.renpy.org/check-for-changes.html) - How to automate displaying a message to a player when a variable changes without writing explicit checks.
+ [Python Tricks #1](https://patreon.renpy.org/python-tricks-1.html) - Simplifying long screen action lists, using `__unicode__` to create a string representation of an object for interpolation.
+ [Python Tricks #2](https://patreon.renpy.org/python-tricks-2.html) - On using random number generation and queueing images for display.
+ [Title Screens](https://patreon.renpy.org/title-screens.html)
+ [In-Game Wiki-Like Glossary or Codex](https://patreon.renpy.org/wiki.html)
+ [Custom Preferences](https://patreon.renpy.org/custom-preferences.html) - Adding more things to the Preferences screen and using them.

## Project templates

Templates to start off a new project containing commonly requested features a stock RenPy new project does not offer.

+ [All-in-one GUI Template](https://tofurocks.itch.io/renpy-gui-template)
+ [renpy-awesome-template](https://github.com/RuolinZheng08/renpy-awesome-template) - An advanced starter project template.
+ [renpy-minimal-template](https://github.com/enaielei/renpy-minimal-template) - Actually the complete reverse: A minimal working template, which contains none of the default GUI. Also contains the example of using the scarcely documented explicitly loadable modules feature.

## Frameworks

Pieces of code big enough to be called libraries.

### General

+ [Console](https://github.com/abduelhamit/renpy-ingame-console/) - An in-game console for the player to use (i.e. distinct from the built-in developer console). Not well documented at all.
+ [DynamicSpriteManager](https://github.com/alexkrob/dynamicsprites/) - A high-level system for easily defining and compiling the RenPy native LayeredImage. Given a directory of images, it will automatically scan and categorize those images for use in a mix-and-match style sprite declaration language based on filenames. Documentation inline with code.
+ [Extra Animated Value](https://github.com/RenpyRemix/extra-animated-value) - Extending `AnimatedValue` for bars.

### Network

+ [RADC](https://github.com/CharlieFuu69/RenPy_Asset_Download_Complement) - A framework to enable a RenPy project to download its own DLC. Documentation in Spanish only.
+ [Discord Rich Presence Support for Ren'Py Projects](https://github.com/Lezalith/RenPy_Discord_Presence) - Interact with Discord Rich Presence.
+ [Auto Weather Change](https://github.com/multimokia/Renpy-Weather-Utils) - Access [openweathermap](https://openweathermap.org/) API to acquire weather information from RenPy.

### Visual novel elements

+ [Renpy Auto Highlight](https://wattson.itch.io/renpy-auto-highlight) - A library to automatically highlight the currently speaking character.
+ [Speech Bubbles](https://github.com/RenpyRemix/speech-bubbles) - A unique look presenting novel text as speech bubbles.
+ [FancyText](https://github.com/yukinogatari/Ren-Py-FancyText) - Text that can fade in letter-by-letter, and appear in other interesting ways.
+ [Kinetic Text Tags](https://github.com/SoDaRa/Kinetic-Text-Tags) - Text that shakes, waves, bounces, scatters, etc.
+ [RPY-VNBE](https://github.com/rjscdev/RPY-VNBE) - A set of multiple libraries, including an achievement system and a number of text effects.
+ [Encyclopaedia Framework](https://github.com/jsfehler/renpy-encyclopaedia) - Simplifies creating an encyclopaedia, bestiary, glossary, or similar system.
+ [renpy-rainbowtext](https://github.com/Lezalith/renpy-rainbowtext) - A rainbow text effect.
+ [renpy-word-description](https://github.com/valery-iwanofu/renpy-word-description) -- Text tooltips on hover over words.

### Gameplay elements

+ [Dating Sim Engine](https://github.com/renpy/dse) - The fundamental code for a Tokimeki Memorial style dating simulation strategy planning game.
+ [Dating sim toolkit](https://github.com/DRincs-Productions/DS-toolkit) - A different take on same.
+ [
Navigation Quest Time Routine System](https://github.com/DRincs-Productions/NQTR-toolkit) - A complete system introducing the concepts of location, time and event, producing the framework of a not-quite-point-and-click adventure game.
+ [Lezinventory](https://www.lezcave.com/lezinventory-framework/) - General purpose inventory system.
+ [Pink Engine](https://pink-productions.itch.io/pink-engine) - Tiled map framework capable of using [Tiled](https://www.mapeditor.org/) maps.
+ [RPG Battle Engine](https://github.com/Habitacle/battle-engine) - What it says on the tin.
+ [Sheepstorm Battle Framework](https://circle-cosine.itch.io/sheepstorm-battle-framework) - A different battle engine.
+ [Cardgame Framework](https://github.com/renpy/cardgame) - What it says on the tin. Ancient code, but still works well in current RenPy. Not very suitable for modification, due to relying exclusively on deprecated features.

### Device imitation

+ [Candella](https://github.com/UnscriptedVN/candella) - "Candella is a fork of the AliceOS framework, a Ren'Py framework that provides an operating environment to visual novels. This operating environment includes utilities, classes, and other code that lets developers and players write and use apps designed for the system." To put it less opaquely, this imitates a full window system with "applications" inside RenPy.
+ [Ren'Py Chat Log](https://github.com/JimTheCactus/chatlogging) -- Library for displaying scrolling chat logs.
+ [Messenger Emulator](https://github.com/sDextra/messenger-emulator) - An advanced library for imitating Telegram Messenger in-game. Requires work to adapt to more modern versions of RenPy.
+ [phone message system for renpy](https://nadianova.itch.io/phone-message-system-for-renpy) - Another implementation of a phone, this one works as is.
+ [RenpyPhoneSMS](https://github.com/israelrbb/RenpyPhoneSMS) - And another one.

### Extra content

In a classic Japanese title, these would go into making the contents of an "Extras" menu.

+ [GalleryPlus](https://github.com/cheonbyeol/RenPy-GalleryPlus) - Extends the functionality of RenPy's built-in Gallery class. Allows looping images, pages, navigation buttons.
+ [renpy-gallery-inject](https://github.com/Numerlor/renpy-gallery-inject) - Self contained gallery screen, and code to allow the screen and functionality to be patched into existing games without changing their code in any way.
+ [RPY-VNBE](https://github.com/rjscdev/RPY-VNBE) - A set of multiple libraries, including an achievement system and a number of text effects.
+ [Ren'Py Universal Player](https://github.com/GanstaKingofSA/RenPy-Universal-Player) - An enhanced music room for Ren'Py projects that allows users to play tracks outside the game's story along with sideloaded songs.
+ [renpy-achievement](https://github.com/shawna-p/renpy-achievement) - A screen to display an XBox-like achievement popup. Does not actually interact with any achievement backend, but the builtin one should serve.

## Cookbook

Most useful RenPy code comes in the form of code snippets, examples, and other small pieces, rather than a well-packaged library. As such, many of these links link to Gists, forum posts, and other such locations wherein a given code snippet is presented in context. You can always wade the depths of [Lemmasoft RenPy forums](https://lemmasoft.renai.us/forums/viewforum.php?f=51) yourself for more.

### Snippets

Not all of these are confirmed to work in current versions of RenPy.

#### Text

+ [Experiments in Ren'Py Heresy](https://gist.github.com/kobaltcore/2d2d913e513d25f02f4800e41fbbee8d) - Several undocumented text effects.
+ Three alternate takes on how to give the player a preview of text printed with a certain given CPS: [by Oliver](https://gist.github.com/methanoliver/bbb026b2c6daeb9b7aae508314e30cfd), [by Lezalith](https://gist.github.com/Lezalith/f6ea469f10f10d21f53c2c5f592cd12f), [by Feniks](https://gist.github.com/shawna-p/3a12772369af03b85b25196275412868)
+ [Subscript and superscript text tags](https://gist.github.com/methanoliver/fb2ef18de4c23fadbb23b13fa3d10d48)
+ [Smallcaps text tag](https://gist.github.com/methanoliver/166c18caa224fa15ead6dca95cccbb05)
+ [Pronouns class](https://github.com/Gouvernathor/renpy-PronounsClass) - A class to handle character pronouns.
+ [Window-fixed CTC](https://gist.github.com/methanoliver/7671cbcabe46bcc8a0f757ba195bb1a4) - how to position a CTC relative to a window, rather than fixed on the screen or relative to the last printed line.
+ [Two-column NVL mode](https://gist.github.com/methanoliver/cb6ae08d432d9395cff65975733599ab) - How to have your NVL screen display two columns of text, filling one after the other in a semi-automatic fashion.

#### Effects

+ [X-Ray effect](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=62128) - This turns the mouse pointer into a device to see inside things.
+ [ChromaGlitch](https://github.com/Gouvernathor/renpy-ChromaGlitch) - Glitch effect.
+ [RenPyGlitch](https://github.com/NyashniyVladya/RenPyGlitchs) - A different implementation of a glitch effect. Documentation in Russian.
+ [SWHolo](https://github.com/Gouvernathor/renpy-SWHolo) - Star Wars hologram effect.
+ [Parallax layer](https://gist.github.com/midgethetree/b449be114f21974ed21b3fbf3653433f) - Layer parallax based on mouse position.
+ [Rain effect](https://gist.github.com/methanoliver/98fe9304b63fff1f7d3419120e2c11f5) - not particle, but rather texture based.
+ [Simple rain effect](https://lemmasoft.renai.us/forums/viewtopic.php?f=52&t=37489#p406150) - describes a simpler, but less convincing technique to make rain.
+ [How to do a cloud animation with RenPy](https://traumendes-madchen.com/blog/?p=1395) - A primer on animated backgrounds.
+ [Noir-Style Shadow/Lighting Effects](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=49140#p483366) - fun with AlphaMask.
+ [Gradient()](https://gist.github.com/methanoliver/f265cd68bf13ac1008d7140d07b2e023) - A Gradient() equivalent of Solid() that generates gradients in place using shaders.

#### Particles

+ [RenPyParticles](https://github.com/AgentAlpha81/RenPyParticles) - Custom particle motion classes. Documentation in Russian.
+ [Dust](https://gist.github.com/rurubell/a30752048bbe20de546d737c2476916f) - a particle effect. Documentation in Russian.
+ [Projection starfield](https://github.com/jsfehler/renpy-projection-starfield) - Particle-based starfield.
+ [Ren-Py-Free-to-Use-Falling-Leaves](https://github.com/Thediamondcryst/Ren-Py-Free-to-Use-Falling-Leaves) - Particle-based falling leaves, complete with assets.
+ [Ren-Py-Free-to-Use-Moving-Clouds](https://github.com/Thediamondcryst/Ren-Py-Free-To-Use-Moving-Clouds) - Particle-based moving clouds, complete with assets.

#### Displayables

+ [Static chessboard displayable](https://github.com/RuolinZheng08/renpy-static-chessboard) - What it says on the tin. Can be used to produce a [full AI-run chess game](https://github.com/RuolinZheng08/renpy-chess).
+ [Analog clock](https://github.com/williamd1k0/renpy-analog-clock) - A clock displayable.
+ [Simpo clock](https://badmustard.itch.io/simpo-clock) - Another clock
+ [Radar chart](https://github.com/jsfehler/renpy-radarchart) - Displayable for plotting data onto a radar chart.

#### User interface

+ [Scrollbutton](https://gist.github.com/midgethetree/b210ddadfb07e85873022fde0202f646) - A button to scroll a viewport.
+ [Continue button](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=48154#p477769) - Multiple methods to create a 'Continue' main menu button that would load the most recent save game.
+ [One-screen visual novel](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=37055#p402373) - that is, how to disable the entire game menu and jump straight into the body of the novel.
+ [Main Menu with a Video Background](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=47193#p472755) - This gets asked on average once a week.
+ [Button "PRESSED" state](https://lemmasoft.renai.us/forums/viewtopic.php?f=8&t=57848&sid=95776df5d873ef265bcf05244d317495) - How to detect that an on-screen button is being held down, rather than just clicked.

#### Other snippets

These are useful, but difficult to categorize.

+ [Free-hand draw](https://github.com/jsfehler/renpy-freehand-draw) - Draw on a canvas inside a Ren'Py game.
+ [MyShow](https://gist.github.com/Enerccio/1e24664f2d6705d30d1f4cce2cced902) - An example of overriding the built-in `show` statement to potentially add functionality, does so by directly editing the script in memory after loading.
+ [screen_choice](https://gist.github.com/dossy/cbb7b7ed18a292e4d9c51c8d63a15c69) - How to apply transitions to the current scene behind a Ren'Py choice menu.
+ [afk.rpy](https://gist.github.com/tserber98/b0d177c4dffa38e4719695b13c87e55f) - How to detect that a player didn't attend the game for a certain period.
+ [Differential image loader](https://gist.github.com/methanoliver/2668767d5332aea66a866d2b84692d1c) - Given two different sprites of the same character in the same pose, produce image files which use one of them as a base, store only the pixels that are different from that base for all others, and automatically make a `layeredimage` out of them.
+ [Affection points](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=22817#p287294) An example of implementing the basic notion of affection points.
+ [A timer that would work and after leaving the project](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=47774#p475564) - Example code to account for time that passed while the game wasn't running.
+ [Buns with sound in renpy](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=54324#p507536) - Answers to multiple questions on how to do something with sound in RenPy.
+ [Scroll any background](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=54333#p507598) - by adding a mirrored copy to the side and repeating.
+ [How to add Google Ads(Admob) to Renpy](https://www.youtube.com/watch?v=oUhcXlzc2a4) - What it says on the tin. (YouTube video)
+ [Yandex Mobile ads in RenPy](https://github.com/valery-iwanofu/rapt-yandex-ads) - What it says on the tin, but in Russian.
+ [Expanding Mobile Functionality With Pyobjus/Pyjnius](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=46091#p467178) - Invoking Android API when on Android.
+ [BPM in Ren'Py - Timing animations to your musics tempo](https://sleepyagents.blogspot.com/2016/09/bpm-in-renpy-timing-animations-to-your.html) - Describes the techniques to manually time an animation to music tempo.
+ [Making a Separate Content Patch](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=45448#p463349) - How to make an optional content patch.
+ [Ren'Py Lovense Boilerplate](https://github.com/lolabray/Renpy-lovense-boilerplate) - Code examples for controlling Lovense vibrating devices from RenPy.
+ [Import Json Data Easier](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=65400) - A class decorator you can use to easily populate data storing objects from a JSON file.
+ [RenPy Extension Demo](https://github.com/Ayowel/renpy-extension-demo) - Examples of using the scarcely documented engine extension mechanism.

### Minigames

Self-contained minigames can occasionally be found. Some assembly is usually required.

+ [Simon Says](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=40295#p428028)
+ [Rhythm game](https://github.com/RuolinZheng08/renpy-rhythm) - Dance Dance Revolution style, well documented.
+ [Rock Paper Scissors](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=50068#p486361) - A RPS game meant as a tutorial how to program one.
+ [renpy-go](https://github.com/limniris1/renpy-go) - [Go](https://en.wikipedia.org/wiki/Go_(game)) in RenPy.
+ [Space Invaders](https://github.com/pass-by-reference/renpy-space-invaders)
+ [Renpy-lockpick-minigame](https://github.com/kaodachet/Renpy-lockpick-minigame)
+ [47 minigames](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=47820#p475772) - A forum post collecting links to minigame implementations on Lemmasoft forums, 47 as of last count. How many still work as written remains unknown.

### Shaders

Shaders are the most arcane part of RenPy, because they require branching into [GLSL](https://en.wikipedia.org/wiki/OpenGL_Shading_Language), while accounting for RenPy intricacies. Some of the effects achieved thereby are very useful, however.

+ [RenPy Shader Collection](https://github.com/valery-iwanofu/renpy-shader-collection) - waves, color picker.
+ [Wave shader](https://github.com/SoDaRa/RenpyWaveShader) - A better documented wave shader.
+ [Renpy-GLSL-Test](https://github.com/WatercressStudios/Renpy-GLSL-Test) - Experimental setup, contains a packaged "whirl" transition that originates from [one of PyTom's patreon posts](https://patreon.renpy.org/dev-2020-07.html).
+ [renpy-blend-modes](https://github.com/CrossCouloir/renpy-blend-modes) - Shader-based Photoshop-style blend modes for images. Only soft light is implemented.
+ [RGB Split](https://github.com/AgentAlpha81/RGB-Split) - Chromatic aberration shader.
+ [Outline shader](https://github.com/RenpyRemix/outline-shader) - Adds outlines to arbitrary objects.
+ [Round corners shader](https://gist.github.com/Pseurae/15dc9c6a145161063126c3b4de39a0aa) - Very neat, but why does it only work on `Solid()` for me, I have no idea.
+ [Shader](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=65248) - Several animated image-generating shaders ported from Shadertoy.
+ [Circle crop](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=64534) - A shader way to make a square image circular.
+ [Drunk blur](https://lemmasoft.renai.us/forums/viewtopic.php?f=51&t=62705) - Double vision "drunk" blur.

### Code examples

Occasionally, entire games are published as open source, though not necessarily free. Whenever they contain anything useful as example code, they go in this section.

+ [Cute demon crashers](https://github.com/robotlolita/cute-demon-crashers) - interesting examples of functional programming, well commented, even if dated.
+ [Learn to Code RPG](https://github.com/freeCodeCamp/LearnToCodeRPG) - a complete RenPy title, showcasing some of the more obscure features, with full source and assets.
+ [Decompiled Doki Doki Literature Club](https://github.com/SecondThundeR/DokiDoki-RenPy) - while this is presented only for the purposes of producing mods, this showcases the state of the art of RenPy programming from 6.99 era, and is of historical and educational interest.
+ [DW Klondike Solitaire](https://github.com/YGGDRASIL-STUDIO/DW-Klondike-Solitaire) - A complete Solitaire in RenPy, good as an example of using the Card Game Framework.
+ [Mysterious Messenger](https://github.com/shawna-p/mysterious-messenger) - An entire game built around a custom messenger imitation.
+ [carpe-diem](https://github.com/moonlitworks/carpe-diem) - Complete source for [Carpe Diem](https://store.steampowered.com/app/423880/Carpe_Diem/)
+ [Without Romance](https://github.com/moonlitworks/without-romance) - A SuNoFES 2020 project.
+ [KatawaShoujo-RenPy8](https://github.com/gcammisa/KatawaShoujo-RenPy8) - A port of the classic Katawa Shoujo visual novel to run on modern versions of RenPy.

### Other

+ [1080p wipes](https://lemmasoft.renai.us/forums/viewtopic.php?f=52&t=37628#p407567) - A collection of 1080p-sized ImageDissolve transition images, neither quite code nor quite an image by itself.

## Tools

### In-engine developer tools

These are meant to be built into the project at least during development, and thus are a cross between libraries and standalone tools.

+ [Ren'Edit](https://minute.itch.io/renedit) - A beta-tester support tool to easily acquire corrections and comments.
+ [ActionEditor](https://github.com/kyouryuukunn/renpy-ActionEditor3) - A powerful director tool for manipulating [camera](https://www.renpy.org/doc/html/model.html), viewing the results and generating code to produce the interactively-defined effects.
+ [MouseFinderTool](https://github.com/CharlieFuu69/RenPy_MouseFinderTool) - A set of developer tools to pinpoint mouse position of things. Documentation in Spanish only.
+ [RVRE](https://github.com/picobyte/RVRE) - The editor provides a means to proofread your visual novel while running it and without leaving.
+ [Caption Tool](https://npckc.itch.io/caption-tool-for-renpy) - A tool to add image and sound captions for accessibility purposes.
+ [renpy-TranslationTools](https://github.com/Gouvernathor/renpy-TranslationTools) - Tools to aid in managing translations in certain corner cases. Also the rare example of embedding RenPy-script in Python, rather than the reverse as is usual.
+ [RenPy automatic translations](https://github.com/Moshibit/RenPy_automatic_translations) - A tool to automate machine translation of your project.
+ [Demotools](https://github.com/Ayowel/renpy-demotools) - An extension that can be used to produce automated demos, screencasts, and otherwise pretend there's a player at the keyboard.

### Standalone developer tools

These are software unto themselves.

#### General

+ [renpy-graphviz](https://github.com/EwenQuim/renpy-graphviz) - Draws a flowchart of a RenPy project based on jumps, calls and labels. Has an online version.
+ [renpydeskgen](https://github.com/Polymehr/renpydeskgen) - Shell script to generate Linux `*.desktop` files for RenPy games.
+ [vnproofer](https://github.com/devorbitus/vnproofer) - Project proofreading and spellchecking tool that works by passing scripts through [cspell](https://www.npmjs.com/package/cspell).
+ [renxel](https://github.com/KagariSoft/renxel) - Transmute RenPy translation files to Excel tables and back.
+ [Ren'Py VSCode Project Template](https://github.com/tiliv/renpy-vscode-template) - a configuration for Visual Studio Code to enable running, linting and building from the IDE.
+ [Visual glBlendFunc + glBlendEquation Tool](https://www.andersriggelsen.dk/glblendfunc.php) - Not RenPy specific, this will be very helpful if you want to figure out `blend` transform property to get a particular visual effect.
+ [Node based script editor](https://github.com/FiendChain/ScriptEditor) - Kind of like Twine's dialogue tree view, but for RenPy.
+ [renpyfmt](https://github.com/kobaltcore/renpyfmt) - A formatter for RenPy code. Work in progress, but looks promising.

#### Continuous integration

+ [renkit](https://github.com/kobaltcore/renkit) - A toolkit for managing Ren'Py instances via the command line, intended for build automation and continuous integration.
+ [renpy-lint-action](https://github.com/ProjectAliceDev/renpy-lint-action) - This GitHub action allows you to run the linter on a Ren'Py visual novel project in a workflow for testing purposes.
+ [renpy-build-action](https://github.com/ProjectAliceDev/renpy-build-action) - This GitHub action allows you to make distributable builds of a Ren'Py visual novel project in a workflow and use the built files for distribution.

#### Unpacking and decompilation

+ [unrpyc](https://github.com/CensoredUsername/unrpyc) - The `*.rpyc` file decompiler.
+ [unrpa](https://github.com/Lattyware/unrpa) - The most famous RPA archive extractor.
+ [RPA Explorer](https://github.com/UniverseDevel/RPA-Explorer) - Essentially a GUI for `unrpa`.
+ [rpatool](https://github.com/Shizmob/rpatool) - The less famous RPA archive extractor.
+ [warpa](https://github.com/mensch272/warpa) - RPA archive manipulation tool written in Rust.
+ [arpy](https://github.com/chrsm/arpy) - Golang implementation of an RPA unpacker.
+ [RenPy-UnAPK](https://github.com/DrDRR/RenPy-UnAPK) - A tool to unpack and decompile an Android build's APK file. Sparsely documented, but there's not much to document.

#### Conversion

+ [Twine to Ren'Py tool](https://ludowoods.itch.io/twine-to-renpy-tool) - A tool to port a [Twine](https://twinery.org/) project to RenPy. Cross-platform, requires Python 2.7 on platforms other than Windows.
+ [articy2renpy](https://github.com/TheSchnappi/articy2renpy) - A converter for [articy:draft](https://www.articy.com/en/) JSON exports to Ren'Py *.rpy script files.
+ [articy3_renpy3](https://github.com/SqFKYo/articy3_renpy3) - Another variation on articy to RenPy converter.

### End-user tools

These tools are made for end-users, rather than developers.

+ [Translator3000](https://github.com/NyashniyVladya/Translator3000) - Runs RenPy games through automated translation. Trial version.
+ [rpycg](https://github.com/lure0xaos/rpycg) - Injects RenPy code into published games to enable developer mode and manually poke at the internals. Windows only.
+ [renpy2linux](https://github.com/Shizmob/renpy2linux) - A script to convert Ren'Py releases to Windows, OSX and Linux-compatible ones, when the only thing you have is one of the three. Requires Linux or OSX to work.

## Assets

No visual novel is complete without artwork and sound. Beware and carefully observe the license terms!

### Asset libraries

+ [Itch.io](https://itch.io/game-assets/genre-visual-novel) - Visual novel specific assets available on Itch.io, both free and paid.
+ [DLSite](https://www.dlsite.com/home/tool) - A large variety of game assets for visual novels from Japanese artists, all of them paid.
+ [Pixabay](https://pixabay.com/) - a variety of Creative Commons images, videos, music and sound effects.
+ [Free Music Archive](https://freemusicarchive.org/) - Royalty-free and CC music.
+ [OpenGameArt](https://opengameart.org/) - assets for a variety of game types, many useful for visual novels.
+ [FreeSound](https://freesound.org/) - major source of free sounds of every description.
+ [SoundBible](https://soundbible.com/) - A collection of sound effects.
+ [Soundimage](https://soundimage.org/) - Specially aimed at game developers.
+ [GameSounds](https://gamesounds.xyz/) - Large library of sounds aimed for games.
+ [FreePD](https://freepd.com/) - Music
+ [Altphotos](https://altphotos.com/) - CC0 stock photos ready to be mutated into artwork.
+ [Filmmusic](https://filmmusic.io/)
+ [Free Stock Music](https://www.free-stock-music.com/)
+ [Shadertoy](https://www.shadertoy.com/) - Lots of publicly available GLSL shader code. Adapting it to RenPy remains on you, however.
+ [The Spriters Resource](https://www.spriters-resource.com/) - A massive library of sprites, including visual novel sprites, ripped from published titles. While not legal to use per se, invaluable when making a fan-game.

#### Fonts

+ [FontSquirrel](https://www.fontsquirrel.com/) - Free TTF/OTF fonts.
+ [FontStruct](https://fontstruct.com/) - a large library of decorative and special-purpose fonts, many of them permissively licensed. Also a web service to build fonts from scratch.
+ [OpenFontLibrary](https://fontlibrary.org/)

#### Individual libre artists

While you can search through places like [DeviantArt](https://deviantart.com), [Soundcloud](https://soundcloud.com/) and [Bandcamp](https://bandcamp.com/) for artists offering their work under one or another variant of [Creative Commons](https://creativecommons.org/), there are certain prolfic ones, and knowing them in advance will make things easier.

+ [Incompetech](https://incompetech.com/music/royalty-free/music.html) - Kevin MacLeod's music. *Everyone* has heard it.
+ [caryoscelus](https://caryoscelus.bandcamp.com/)
+ [PeriTune](https://peritune.com/)
+ [Alexander Zhelanov](https://soundcloud.com/alexandr-zhelanov)
+ [Savfk](https://soundcloud.com/savfk)
+ [Silverman Sound Studios](https://soundcloud.com/silvermansound)
+ [MaxKoMusic](https://soundcloud.com/maxkomusic)
+ [Audionautix](https://audionautix.com/)

### Asset generators

#### Sound generators

+ [ChipTone](https://sfbgames.itch.io/chiptone) - online generator.
+ [FxTone](https://raylibtech.itch.io/rfxgen) - online generator.
+ [LabChirp](https://labbed.itch.io/labchirp)
+ [SteosVoice](https://cybervoice.io/en/) - High quality AI-based speech synthesis useful for generating voice for visual novels.

#### Character sprite generators

+ [Sutemo's Character Creator](https://emily2.itch.io/sutemo) - online only.
+ [Mannequin](https://ar14.itch.io/mannequin) - free and paid versions, multiplatform.
+ [Manga Maker ComiPo](https://store.steampowered.com/app/262490/Manga_Maker_Comipo/) - has been used to produce sprites for at least one novel available on Steam. Windows only.
+ [VRoid Studio](https://store.steampowered.com/app/1486350/VRoid_Studio_v1130/) - Avatar generator meant for VTubers, can in a pinch be used to manufacture sprite images. Crossplatform, free as in beer. For posing them, you might want to use [VRM Posing Desktop](https://store.steampowered.com/app/1895630/VRM_Posing_Desktop/), which is Windows-only and not free.
+ [Charat Rouge](https://charat.me/en/rouge/) / [Charat Blanc](https://charat.me/en/blanc/) - online character sprite generator, limited to portraits, license prohibits commercial use of the result.
+ [Stella Character Generator](https://visustella.itch.io/stella-character-generator) - paid, Windows only.
+ [Open Peeps](https://www.openpeeps.com/) - CC0 library of parts suitable for producing character art. Substantial assembly required.

#### Other generators

+ [TextureLab](https://njbrown.itch.io/texturelab) - Procedural texture generator.
+ [Procgen Arcana](https://watabou.github.io/) - A collection of generators intended primarily for tabletop roleplaying which produce useful maps.
+ [Celestia](https://celestia.space/) - Produce *correct* images of the sky in space at a given time. Open source and cross platform.
+ [Space Engine](https://store.steampowered.com/app/314650/SpaceEngine/) - A more powerful commercial competitor to Celestia.
+ [Stellarium](http://stellarium.org/) - For when you don't want to go to space.

#### AI-powered generators

Most of these are only useful to produce background images, as getting the detail and specificity required of anything else out of them is impractical. But free backgrounds are free backgrounds.

+ [ArtBreeder](https://www.artbreeder.com/)
+ [DreamStudio](https://beta.dreamstudio.ai/)
+ [WaifuLabs](https://waifulabs.com/) - limited usefulness, good for inspiration.
+ [craiyon](https://www.craiyon.com/)
+ [NeuralBlender](https://neuralblender.com/create-art)
+ [SumoPaint](http://sumopaint.com/) - An online paint program that integrates a [Stable Diffusion](https://en.wikipedia.org/wiki/Stable_Diffusion)-based image generator.

### Asset editing tools

#### Graphics

+ [Krita](https://krita.org/) - The best open source paint program.
  + [Generate Ren'Py Scripting](https://github.com/SeanHRN/generate-renpy-scripting) - A plugin for Krita, outputs a block of Ren'Py script to display the images of the active Krita document as they appear on the canvas, working in tandem with the [krita-batch-exporter](https://github.com/GDQuest/krita-batch-exporter).
+ [GIMP](https://www.gimp.org/) - The more arcane and ancient, but likewise powerful open source paint program.
+ [Synfig Studio](https://www.synfig.org/) - Free animation software.
+ [Inkscape](https://inkscape.org/) - best open source vector image editor.
+ [Boxy SVG](https://boxy-svg.com/) - free as in beer online-also vector image editor, cloud services require payment.
+ [IMGOnline.com.ua](https://www.imgonline.com.ua/eng/) - a collection of online texture processing tools.
+ [Waifu2X](https://waifu2x.booru.pics/) - AI-based image upscaler.
+ [FotoSketcher](https://fotosketcher.com/) - A better way of making photos look like paintings. Windows-only, runs under Wine.
+ [VanceAI](https://vanceai.com/) - A number of online image processing tools that includes interesting photo-to-sketch implementations.
+ [Calligraphr](https://www.calligraphr.com/) - A web service that generates a TTF from supplied images, meant primarily to produce handwritten fonts.
+ [Homestyler](https://www.homestyler.com/) - Online interior design tool, useful to produce an image of an interior that you will later torture with an AI painting tool.

#### Sound

+ [Audacity](https://www.audacityteam.org/) - Open source audio editor.
+ [Ocenaudio](https://www.ocenaudio.com/en/) - Less powerful, but more convenient, free (as in beer) audio editor.
+ [Ardour](https://ardour.org) - A complete free Digital Audio Workstation.
+ [LMMS](https://lmms.io/) - A loop-based Digital Audio Workstation.

#### Video

+ [FFMpeg](https://ffmpeg.org/) - the Swiss army knife of video *and audio* format conversion and filtering. If you need a GUI for it, there's [QWinFF](https://qwinff.github.io/), [Axiom](https://github.com/MattMcManis/Axiom), [Videomass](https://github.com/jeanslack/Videomass), to name but a few.

## Support

You can find a community of RenPy users in your language, provided it's one of:

+ [Discord English](https://discord.gg/6ckxWYm)
+ [Discord Spanish](https://discord.gg/KWDk6se)
+ [Discord French](https://discord.gg/SZN5uxeMf5)
+ [Discord Russian](https://discord.gg/umzUwffsXk)

## Other Awesome Lists

Other amazingly awesome lists can be found in [awesome](https://github.com/sindresorhus/awesome), [awesome-awesome](https://github.com/emijrp/awesome-awesome) and [awesome-awesomeness](https://github.com/bayandin/awesome-awesomeness).

Those should be of particular interest for RenPy users:

+ [awesome-python](https://github.com/vinta/awesome-python)
+ [awesome-glsl](https://github.com/vanrez-nez/awesome-glsl)
+ [magictools](https://github.com/ellisonleao/magictool)
