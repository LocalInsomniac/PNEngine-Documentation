# Level

Levels are JSON files that contain information on the level itself and its
contents. A level in PNEngine consists of one or more rooms that can be
displayed with a static model and contains actors.

Events are also defined within levels and are assigned a unique ID and a
[Script](Script.md). They can be triggered on level start, by entering a room
it's assigned to or using an Event Trigger.

## Properties

| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
| `name` | String | `N/A` | The name of the level to display in Discord's Rich Presence. Note that Title Cards will not use this name and will instead display the name defined by `level.<filename of the level>` in the current language. |
| `icon` | String | `N/A` | The icon to display in Discord's Rich Presence. |
| `music` | Array | `N/A` | The music track(s) to play upon entering the level. The array can hold up to 4 music tracks, but only the first one will play at full volume. |
| `ambient_color` | Integer or Array | `N/A` | The ambient color to tint unlit models and particles with. Integers are considered BGR values and arrays have a red, green, blue and optional alpha component. |
| `fog_distance` | Array | `N/A` | An array containing the starting and ending distance of the fog in level units. |
| `fog_color` | Integer or Array | `N/A` | The color of the fog to tint unlit models and particles with. Integers are considered BGR values and arrays have a red, green, blue and optional alpha component. |
| `directional_lights` | Array | `N/A` | An array containing the structs of directional lights at the start of the level. For directional light properties, see [Directional Light Properties](#directional-light-properties). |
| `rooms` | Array | `N/A` | An array containing the structs of the level's rooms. For properties, see [Room Properties](#room-properties). |
| `generics` | Array | `N/A` | An array containing the structs of the generic objects to create at the start of the level. For properties, see [Generic Object Properties](#generic-object-properties). |
| `events` | Array | `N/A` | An array containing the structs of the level's events. For properties, see [Event Properties](#event-properties). |
| `assets` | Array | `N/A` | An array containing the names of the assets to manually load when entering the level. Note that this should only be used for assets that are not in the level and are required for level scripting. |

## Directional Light Properties

| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
| `active` | Boolean | `true` | Determines if the light is initially active. |
| `normal` | Array | `[0, 0, -1]` | The normal vector for the light to face toward. |
| `color` | Integer or Array | `16777215`, `[1, 1, 1]` or `[1, 1, 1, 1]` | The color of the light. Integers are considered BGR values and arrays have a red, green, blue and optional alpha component. |

## Room Properties

| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
| `id` | Integer | `N/A` | The unique ID of the room. |
| `model` | String | `N/A` | The model and collision mesh to use for the room. |
| `actors` | Array | `N/A` | An array containing the structs of the room's actors. For properties, see [Room Actor Properties](#room-actor-properties). |
| `event` | Integer | `N/A` | The ID of the event to trigger upon entering the room. |

### Room Actor Properties

| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
| `type` | String | `N/A` | The actor's type without the `act`-prefix. |
| `x` | Float | `0` | The actor's starting X position. |
| `y` | Float | `0` | The actor's starting Y position. |
| `z` | Float | `0` | The actor's starting Z position. |
| `angle` | Float | `0` | The actor's starting angle. |
| `tag` | Integer | `0` | The actor's tag for use with level scripting. |
| `persistent` | Boolean | `0` | Whether or not the actor will stay destroyed upon re-entering the room. |
| `special` | Struct | `N/A` | The special properties of the actor, which may vary based on its type. |

## Generic Object Properties

| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
| `type` | String | `N/A` | The generic object's type without the `gen`-prefix. |
| `special` | Struct | `N/A` | The special properties of the generic object, which may vary based on its type. |

## Event Properties

| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
| `id` | Integer | `N/A` | The unique ID of the event. |
| `script` | String | `N/A` | The name of the script to execute upon triggering the event. |
| `start` | Bool | `false` | Whether or not to trigger this event immediately on level start. |
| `persistent` | Bool | `false` | Whether or not to keep running the event's script between room changes. |
| `skippable` | Bool | `false` | Whether or not to allow skipping the event by pressing Interact. |