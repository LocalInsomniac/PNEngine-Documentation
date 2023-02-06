# Material

Materials are JSON files that define how the game should display a model's submodels.

A material will be automatically loaded if the model that uses it gets loaded.

## Properties

| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
| `image` | Integer or String | `-1` | The name of the image for the material to display. `-1` is considered a blank white texture. |
| `speed` | Float | `0` | The playback speed of the material's image in frames per millisecond. |
| `bright` | Float | `0` | The brightness factor of the material. |
| `x_scroll` | Float | `0` | The horizontal scrolling speed of the material in full scrolls per millisecond. |
| `y_scroll` | Float | `0` | The vertical scrolling speed of the material in full scrolls per millisecond. |
| `specular` | Float | `0` | The intensity of specular highlights on the material. |
| `specular_exponent` | Float | `1` | The specular exponent of the material. Higher values mean smaller highlights. |