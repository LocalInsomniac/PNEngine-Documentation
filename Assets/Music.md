# Music

Music, while sharing the same system as sounds, have different properties:
- They can only be played globally in up to three different layers.
- Have multiple layers of fading in and out (in-game, level scripting, etc.)
- Loop points and an optional metadata struct for special handling.

Currently, only OGGs are supported as music tracks.

## Properties

| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
| `loop_start` | Float | `N/A` | The starting loop point in seconds. |
| `loop_end` | Float | `N/A` | The ending loop point in seconds. |
| `metadata` | Struct | `N/A` | The metadata for the music track. Can be used for special handling through the game or level scripting. |