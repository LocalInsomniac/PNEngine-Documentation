# Credits

PNEngine is a GameMaker framework created by [Can't Sleep](https://localinsomniac.github.io) and [nonk123](https://github.com/nonk123).

## Libraries

PNEngine makes use of the following GameMaker libraries:

| Library | Description | Context |
| ------- | ----------- | ------- |
| [Collage](https://github.com/tabularelf/Collage) | Texture page builder and image manager. | Used for loading multiple images. |
| [Input](https://github.com/JujuAdams/Input) | Comprehensive cross-platform input library. | Used for user input, rebinding and hotswapping. |
| [input-string](https://github.com/offalynne/input-string) | Multi-platform text entry utility. | Used for debugging, i.e. inputting console prompts. |
| [Lexicon](https://github.com/tabularelf/lexicon) | Localization system that simplifies adding translations. | Used for multi-language support. |
| [NekoPresence](https://github.com/nkrapivin/NekoPresence) | A Discord Rich Presence extension. | Used for showing the user's current game state on Discord. |
| PNAudio | Layer-based sound and music playback library. | Used for handling world and UI sounds as well as music tracks. |
| PNCollisions | Fast and simple 3D collision system. | Used for colliding with static and moving level geometry. |
| [Scribble](https://github.com/JujuAdams/scribble) | Modern text renderer. | Used for text formatting, i.e. fonts, colors and effects. |
| [Snidr's Model Format](https://forum.gamemaker.io/index.php?threads/smf-3d-skeletal-animation-now-with-a-custom-blender-exporter.19806/) | Simple skeletal animation system. | Used for model animation and real-time bone manipulation. PNEngine uses a custom fork of version 0.8.6 with drastic optimizations and a custom vertex buffer format to allow vertex colors. |
| [Tiny Expression Runtime](https://github.com/YAL-GameMaker/tiny-expression-runtime) | Custom interpreter that can compile and execute code in real-time. | Used for debugging and level scripting. PNEngine uses a custom fork that adds get/set for structs, treats DS Lists as arrays and links TXR threads to Event Handlers to allow pausing code execution. |