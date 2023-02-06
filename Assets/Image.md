# Image

Images are PNG files used for GUI graphics and/or textures for primitives and materials. They are located in `data\images` and may come with an optional JSON file that tells PN Engine how the image should be displayed in-game.

An image will be automatically loaded if the material that uses it gets loaded.

## Properties

| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
| `frames` | Integer | `1` | The amount of frames the image consists of. |
| `x_offset` | Integer | `0` | The X offset of the image. |
| `y_offset` | Integer | `0` | The Y offset of the image. |
| `x_repeat` | Boolean | `true` | Whether or not to tile the image horizontally. |
| `y_repeat` | Boolean | `true` | Whether or not to tile the image vertically. |