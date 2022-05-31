## ParEdit

At the end of 2021, I decided I wanted to both learn unreal engine and make a custom song editor for the game paradiddle. I accomplished that and learned a whole bunch along the way!


**Overview**

I have quite a lot of experience mapping in the past for a game called Beat Saber, so I have a decent enough understanding of what makes a comfortable and efficient workflow. The editor in question is [EditorSaber](https://github.com/Ikeiwa/EditSaber) (or all the preceding forks [EditSaber Enhanced](https://github.com/permissionBRICK/EditSaberEnhanced), [Mediocre Mapper](https://github.com/squeaksies/MediocreMapper/releases), [Mediocre Mapper Assistant 2](https://git.bsmg.dev/Top_Cat/MediocreMapAssistant2)) and it taught me a huge amount about good workflow. UI element ideas from [Chromapper](https://github.com/Caeden117/ChroMapper) were also adopted for one or two things. If you have used any of those editors listed, you'll be very comfortable using this editor; keybinds are similar, ui is similar, and overall feel is similar.

## Current Features

**Good BPM change support.** BPM changes are extensively supported, allowing you to place them down, modify their placement after the fact, and retain their relative beats while it's done so. this allows you to easily deal with drift or odd time signatures with ease. You can also copy and paste them, and include notes in the copy action. More features are planned in the future, like automatic bpm detection and automatic BPM change placement, and the ability to drag notes around with bpm change updates.

![Untitled](https://user-images.githubusercontent.com/24213630/171141109-946b0f4c-2599-45a0-99f1-9b349fa38670.png)


**High quality spectrogram.** A huge amount of work went into the spectrogram, but it was well worth it. The spectrogram has 2 main settings, the low frequency mode, and standard mode.

**Low Frequency Mode** allows the user to look at a close up of 5000hz and below, although you can go all the way down to just looking at 300 hz and below. This gives you an incredible view of all the low frequencies, allowing you to more easily pick apart close together sounds, or giving you a better idea of the tone of a drum.

**Standard Mode** gives you the full range of frequencies and allows you to more easily spot Rides, Hi-Hats, and Crashes.

![Modes](https://user-images.githubusercontent.com/24213630/171140529-c0ab47f6-95ba-41eb-bd3f-66321f7471f0.png)

**Multi audio format support.** To keep parity with the game, the editor supports .Wav, .Flac, .MP3, .OGG. This gives you wide flexibility in the formats you wish to use for your beat map.

**Multi audio track support.** Again, to keep parity with the game, multiple tracks are supported and will be loaded, no sweat. The spectrogram track is also separate from the game tracks, allowing you to mix and match the tracks and get exactly what you want from the spectrogram.

**Good user made drumset support.** You can create custom drum sets in game then add them directly into the map! There's no need to work with the standard 10 piece set for a song only requiring 4 instruments. You can also make unique drum kits that would otherwise not be possible in real life.

## Future Plans

Currently the editor is a little unstable. there are the occasional crashes and the spectrogram is slow to generate. In the future, I'm going to convert the spectrogram fully to C++ once I have all the features I want to add figured out.

I'm also planning on adding a way to add saved drum sessions to your clipboard, so you can paste them down in the editor. That way you only need to do cleanup in editor and can make the entire beat map in Paradiddle (in theory).

bookmarks, and jump points are planned to be added. These will allow you to jump around in editor or in the map in game to a specified place, put down by the mapper, similar to clone hero.

As the game updates, this editor will be too to keep up with all its features.

other than that, lots and lots of bugs and small things to be added
