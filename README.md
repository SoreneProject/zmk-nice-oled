# nice!oled

## Features

- OLED display support
- Custom status screen
- WPM counter
- Layer indicator
- Profile indicator
- Output status
- HID indicators
- Modifiers indicators
- Luna the dog animation

## Installation

1. Add the following to your `config.yml`:

```yaml
include:
  - nice_view_adapter
  - nice_oled
```

2. Add the following to your `config.dts`:

```dts
&nice_view {
    compatible = "nice,view";
};
```

3. Add the following to your `config.dts`:

```dts
&nice_view {
    compatible = "nice,view";
};
```

4. Add the following to your `config.dts`:

```dts
&nice_view {
    compatible = "nice,view";
};
```

## Configuration

### Display

The display can be configured using the following Kconfig options:

- `CONFIG_NICE_VIEW_WIDGET_STATUS`: Enable custom status screen
- `CONFIG_NICE_VIEW_WIDGET_INVERTED`: Invert display colors
- `CONFIG_NICE_OLED_WIDGET_WPM`: Enable WPM counter
- `CONFIG_NICE_OLED_WIDGET_HID_INDICATORS`: Enable HID indicators
- `CONFIG_NICE_OLED_WIDGET_MODIFIERS_INDICATORS`: Enable modifiers indicators

### Animation

The animation can be configured using the following Kconfig options:

- `CONFIG_NICE_OLED_GEM_ANIMATION`: Enable animation on peripheral
- `CONFIG_NICE_OLED_GEM_ANIMATION_MS`: Animation length in milliseconds
- `CONFIG_NICE_OLED_POKEMON_ANIMATION`: Enable Pokemon animation on peripheral
- `CONFIG_NICE_OLED_POKEMON_ANIMATION_MS`: Pokemon animation length in milliseconds
- `CONFIG_NICE_OLED_VIM`: Enable static vim on peripheral
- `CONFIG_NICE_OLED_VIP_MARCOS`: Enable static vim_marcos on peripheral

## Example

```yaml
shield: corne_left nice_view_adapter nice_oled
shield: corne_right nice_view_adapter nice_oled
```
