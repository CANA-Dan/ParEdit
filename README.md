## ParEdit

At the end of 2021, I decided I wanted to both learn unreal engine and make a custom song editor for the game paradiddle. I accomplished that and learned a whole bunch along the way!

[Paradiddle Discord Server](https://discord.gg/paradiddle)

[ParEdit Wiki](https://github.com/CANA-Dan/ParEdit/wiki)


**Overview**

I have quite a lot of experience mapping in the past for a game called Beat Saber, so I have a decent enough understanding of what makes a comfortable and efficient workflow. The editor in question is [EditorSaber](https://github.com/Ikeiwa/EditSaber) (or all the preceding forks [EditSaber Enhanced](https://github.com/permissionBRICK/EditSaberEnhanced), [Mediocre Mapper](https://github.com/squeaksies/MediocreMapper/releases), [Mediocre Mapper Assistant 2](https://git.bsmg.dev/Top_Cat/MediocreMapAssistant2)) and it taught me a huge amount about good workflow. UI element ideas from [Chromapper](https://github.com/Caeden117/ChroMapper) were also adopted for one or two things. If you have used any of those editors listed, you'll be very comfortable using this editor; keybinds are similar, ui is similar, and overall feel is similar.

## Current Features

**Good BPM change support.** BPM changes are extensively supported, allowing you to place them down, modify their placement after the fact, and retain their relative beats while it's done so. This allows you to deal with drift or odd time signatures with ease. You can also copy and paste them, and include notes in the copy action.

![BPM manipulation menu](https://user-images.githubusercontent.com/24213630/171141109-946b0f4c-2599-45a0-99f1-9b349fa38670.png)


**High quality spectrogram.** A huge amount of work went into the 3D spectrogram, but it was well worth it. The spectrogram is both very fast and customizable to a high degree, allowing you to change brightness, frequency logarithm, volume exponent (sharpness), and color, all at run time without needing to regenerate the spectrogram. Additionally, you can clamp the frequencies you want to look at to get a high detail view of just those frequencies, and you can set how many threads you wish to use, up to 16 total threads.

![Spectrogram](https://user-images.githubusercontent.com/24213630/180401942-327719f7-b9c4-4832-96e9-14a866ab1cee.png)

**Multi audio format support.** To keep parity with the game, the editor supports .Wav, .Flac, .MP3, .OGG. This gives you wide flexibility in the formats you wish to use for your beat map.

**Multi audio track support.** Again, to keep parity with the game, multiple tracks are supported and will be loaded, no sweat. The spectrogram track is also separate from the game tracks, allowing you to mix and match the tracks and get exactly what you want from the spectrogram. In editor you can manage the audio tracks, allowing you to mute or solo tracks with ease

**Good user made drumset support.** You can create custom drum sets in game then add them directly into the map! There's no need to work with the standard 10 piece set for a song only requiring 4 instruments. You can also make unique drum kits that would otherwise not be possible in real life.

## Future Plans

I'm also planning on adding a way to add saved drum sessions to your clipboard, so you can paste them down in the editor. That way you only need to do cleanup in editor and can make the entire beat map in Paradiddle (in theory).

bookmarks, and jump points are planned to be added. These will allow you to jump around in editor or in the map in game to a specified place, put down by the mapper, similar to clone hero.

More BPM change QOL things, like automatic bpm detection and automatic BPM change placement, and copy and pasting between bpm changes.

As the game updates, this editor will be too to keep up with all its features.

other than that, lots and lots of bugs and small things to be added
