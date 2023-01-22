## ParEdit

At the end of 2021, I decided I wanted to both learn unreal engine and make a custom song editor for the game paradiddle. I accomplished that and learned a whole bunch along the way!

[Paradiddle Discord Server](https://discord.gg/paradiddle)

[ParEdit Wiki](https://github.com/CANA-Dan/ParEdit/wiki)


**Overview**

I have quite a lot of experience mapping in the past for a game called Beat Saber, so I have a decent enough understanding of what makes a comfortable and efficient workflow. The editor in question is [EditSaber](https://github.com/Ikeiwa/EditSaber) (or all the preceding forks [EditSaber Enhanced](https://github.com/permissionBRICK/EditSaberEnhanced), [Mediocre Mapper](https://github.com/squeaksies/MediocreMapper/releases), [Mediocre Mapper Assistant 2](https://git.bsmg.dev/Top_Cat/MediocreMapAssistant2)) and it taught me a huge amount about good workflow. UI element ideas from [Chromapper](https://github.com/Caeden117/ChroMapper) were also adopted for one or two things. If you have used any of those editors listed, you'll be very comfortable using this editor; keybinds are similar, ui is similar, and overall feel is similar.

## Current Features

**Good BPM change support.** BPM changes are extensively supported, allowing you to place them down, modify their placement after the fact, and retain their relative beats while it's done so. This allows you to deal with drift or odd time signatures with ease. You can also copy and paste them, and include notes in the copy action. Movement between bpm changes with clean snapping is supported, as well as copy and pasting large sections of notes across multiple bpm changes at once.

![BPM manipulation menu](https://user-images.githubusercontent.com/24213630/171141109-946b0f4c-2599-45a0-99f1-9b349fa38670.png)

**High quality spectrogram.** A huge amount of work went into the 3D spectrogram, but it was well worth it. The spectrogram is both very fast and customizable to a high degree, allowing you to change brightness, frequency logarithm, volume exponent (sharpness), and color, all at run time without needing to regenerate the spectrogram. Additionally, you can clamp the frequencies you want to look at to get a high detail view of just those frequencies, you can separate the left and right audio channels to get a clearer view of each channel, and you can set how many threads you wish to use, up to 24 total threads. Theres also a waveform for the people who want one of those. Much faster than the spectrogram to generate as well, so a good lightweight option for weaker systems.

![Spectrogram](https://user-images.githubusercontent.com/24213630/180401942-327719f7-b9c4-4832-96e9-14a866ab1cee.png)
![Waveform](https://user-images.githubusercontent.com/24213630/196630542-d22c6da2-0075-4d5e-af37-c2080746b1bd.png)

**MIDI Out.** Using a program like [LoopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html), you can output the notes to paradiddle or a daw to get realtime feedback for timing or if your instruments are correct.

**Multi audio format support.** To keep parity with the game, the editor supports .Wav, .Flac, .MP3, and .OGG. This gives you wide flexibility in the formats you wish to use for your beat map.

**Multi audio track support.** Again, to keep parity with the game, multiple tracks are supported and will be loaded, no sweat. The spectrogram track is also separate from the game tracks, allowing you to mix and match the tracks and get exactly what you want from the spectrogram. In editor you can manage the audio tracks, allowing you to mute or solo tracks with ease. You can also view multiple spectrograms simultaniously for multi drum track setups.

![Multi Spectrogram](https://user-images.githubusercontent.com/24213630/196630920-f69f4d59-da90-4018-8b38-1bfda85dca6d.png)
![Audio Management](https://user-images.githubusercontent.com/24213630/196630938-d5231130-c952-41c6-843f-5f7085c61519.png)

**Good user made drumset support.** You can create custom drum sets in game then add them directly into the map! There's no need to work with the standard 10 piece set for a song only requiring 4 instruments. You can also make unique drum kits that would otherwise not be possible in real life.

**Import Recordings From Paradiddle.** You can import drum sessions made in paradiddle into ParEdit. This means you can, in theory, make maps totally in paradiddle and just setup the metadata in ParEdit.

## Future Plans

Importing and exporting midi.

More BPM change QOL things, like automatic bpm detection and automatic BPM change placement.

As the game updates, this editor will be too to keep up with all its features.

other than that, lots and lots of bugs and small things to be added
