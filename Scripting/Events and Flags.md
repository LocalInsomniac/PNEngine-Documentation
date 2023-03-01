# Events and Flags

PNEngine uses flags to track progress during gameplay. A flag is a key-value
pair that can contain any kind of value. There are two types of flags that can
be accessed - global flags are carried across levels as well as save files, and
local flags are temporary values that will only be active during the current
level's session.

## Constants

| Name     | Type   | Description |
| -------- | ------ | ----------- |
| `global` | Struct | Contains all of the global flags. Global flags are always persistent and will also be included in save files. |
| `local`  | Struct | Contains all of the local flags. Local flags are only available for the current level and are cleared after changing levels. |

## Functions

- `event_wait(ticks)` - Pauses the execution of the script's event handler until the specified amount of ticks have passed.
- `event_handle(event, [args])` - Creates a new event handler with optional arguments passed to it.
- `event_invoker()` - Returns the actor that triggered the script's event handler. For EventTriggers this redirects to the actor that touched it.