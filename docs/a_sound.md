# Sound

Sounds in PN Engine can be processed in many ways. They can be played globally, in a specific world location or from an actor that has an active audio emitter. They can also be played with a base pitch, a random pitch offset and variable falloff. There are two separate sound layers: UI and World, which allows for more flexible sound design.

Sounds can be 8-bit or 16-bit, mono or stereo WAV files with each having an optional JSON file that defines how they're played in-game.

## Properties

| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
| `pitch_high` | Float | `1` | The highest random pitch offset when played. |
| `pitch_low` | Float | `1` | The lowest random pitch offset when played. |