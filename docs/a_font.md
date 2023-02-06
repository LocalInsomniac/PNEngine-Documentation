# Font

Fonts are used for general text rendering. They can be either bitmaps or TrueType, and are accompanied with a JSON file that defines how the fonts are rendered in-game.

## Properties

#### Bitmap Fonts

| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
| `frames` | Integer | `1` | The amount of characters in the bitmap, in ASCII format. |
| `first` | String | `"!"` | The first character included in the bitmap. |
| `proportional` | Boolean | `true` | Whether or not to space the font based on the width of each character. |
| `space` | Integer | `true` | The amount of pixels to leave between each character. |

#### TrueType Fonts

| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
| `size` | Float | `8` | The size of the font in pixels. |
| `bold` | Boolean | `false` | Determines whether or not the font should be rendered in bold. |
| `italics` | Boolean | `false` | Determines whether or not the font should be rendered in italics. |
| `first` | Integer | `32` | The first character to include from the font. |
| `last` | Integer | `128` | The last character to include from the font. |
| `smooth` | Boolean | `true` | Whether or not to smooth the edges of the font. **(Not implemented)** |
| `sdf` | Boolean | `true` | Whether or not to use Signed Distance Field rendering for the font. **(Not implemented)** |