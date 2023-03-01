# Variables and Arrays

While instance and struct variables and arrays can be directly accessed, there are extra functions from GML exposed for ease of access and quality of life.

## Variables

- [`variable_instance_exists(instance_id, name)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/variable_instance_exists.htm)
- [`variable_instance_get_names(instance_id)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/variable_instance_get_names.htm)*
- [`variable_instance_names_count(instance_id)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/variable_instance_names_count.htm)
- [`variable_instance_get(instance_id, name)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/variable_instance_get.htm)
- [`variable_instance_set(instance_id, name, val)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/variable_instance_set.htm)
- [`variable_struct_exists(struct, name)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/variable_struct_exists.htm)
- [`variable_struct_get(struct, name)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/variable_struct_get.htm)
- [`variable_struct_set(struct, name, val)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/variable_struct_set.htm)
- [`variable_struct_remove(struct, name)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/variable_struct_remove.htm)
- [`variable_struct_get_names(struct)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/variable_struct_get_names.htm)
- [`variable_struct_names_count(struct_id)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/variable_struct_names_count.htm)
- [`instanceof(struct_id)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/instanceof.htm)

*GameMaker's `global` is not exposed to scripting.

## Arrays

- [`array_create(size, [value])`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/array_create.htm)
- [`array_copy(dest, dest_index, src, src_index, length)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/array_copy.htm)
- [`array_equals(var1, var2)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/array_equals.htm)
- [`array_get(variable, index)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/array_get.htm)
- [`array_set(variable, index, value)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/array_set.htm)
- [`array_push(variable, value, [value], [value], [etc...])`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/array_push.htm)
- [`array_pop(array)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/array_pop.htm)
- [`array_insert(variable, index, value, [value], [value], [etc...])`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/array_insert.htm)
- [`array_delete(variable, index, number)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/array_delete.htm)
- [`array_sort(variable, sorttype)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/array_sort.htm)*
- [`array_length(array_index)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/array_length.htm)
- [`array_resize(array_index, new_size)`](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Variable_Functions/array_resize.htm)

*Methods are not available in TXR.