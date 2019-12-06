# base16-windows-terminal

[Base16](https://github.com/chriskempson/base16) template for [Windows Terminal](https://github.com/microsoft/terminal). 

This includes both template files for use with [Base 16 Builders](https://github.com/chriskempson/base16#builder-repositories) and color files for end users to use with [Windows Terminal](https://github.com/microsoft/terminal)

## Installation

You can simply copy the contents of your chosen theme's JSON file into the schemes array in profiles.json. Then just the color scheme to your profile.

Here's an example profiles.json:

```
{
    "$schema": "https://aka.ms/terminal-profiles-schema",

    "defaultProfile": "{61c54bbd-c2c6-5271-96e7-009a87ff44bf}",

    "profiles":
    [
		{
            "guid": "{61c54bbd-c2c6-5271-96e7-009a87ff44bf}",
            "name": "Windows PowerShell",
            "commandline": "powershell.exe",
            "hidden": false,
            "colorScheme": "Monokai" //Choose your color scheme here
        },
        {
            "guid": "{2c4de342-38b7-51cf-b940-2309a097f518}",
            "hidden": false,
            "name": "Ubuntu",
            "source": "Windows.Terminal.Wsl"
        },
        {
            "guid": "{b453ae62-4e3d-5e58-b989-0a998ec441b8}",
            "hidden": false,
            "name": "Azure Cloud Shell",
            "source": "Windows.Terminal.Azure"
        }
    ],

    // Add custom color schemes to this array
    "schemes": [
      {
        "name": "Monokai",
        "background":    "#272822",
        "foreground":    "#f8f8f2",
        "black":         "#272822",
        "red":           "#f92672",
        "green":         "#a6e22e",
        "yellow":        "#f4bf75",
        "blue":          "#66d9ef",
        "magenta":       "#ae81ff",
        "cyan":          "#a1efe4",
        "white":         "#f8f8f2",
        "brightBlack":   "#75715e",
        "brightRed":     "#fd971f",
        "brightGreen":   "#383830",
        "brightYellow":  "#49483e",
        "brightBlue":    "#a59f85",
        "brightMagenta": "#f5f4f1",
        "brightCyan":    "#cc6633",
        "brightWhite":   "#f9f8f5"
      }
    ]
}
```

If you want more information on profiles.json, see [Using JSON Settings](https://github.com/microsoft/terminal/blob/master/doc/user-docs/UsingJsonSettings.md) and [Profiles.json Documentation](https://github.com/microsoft/terminal/blob/master/doc/cascadia/SettingsSchema.md#schemes).
