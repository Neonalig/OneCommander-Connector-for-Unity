<span style="display:block;text-align:center">

<!-- Invisible top level heading to prevent the title from being displayed twice -->
<span style="display:none">

# OneCommander Connector for Unity

</span>

![OneCommander Connector for Unity](https://github.com/Neonalig/OneCommander-Connector-for-Unity/blob/main/Resources/Branding/BrandingLargeTransparent.png?raw=true)

<em> Quickly view and open files and folders in OneCommander from your Unity project. </em>

[![OneCommander Connector for Unity on Unity Asset Store](https://github.com/Neonalig/OneCommander-Connector-for-Unity/blob/main/Resources/Branding/AssetStore.png?raw=true)](https://assetstore.unity.com/packages/tools/utilities/onecommander-connector-for-unity-247753?aid=1011lvXjM)

</span>

<br />

- [OneCommander Connector for Unity](#onecommander-connector-for-unity)
  - [Installation](#installation)
  - [Usage](#usage)
    - [Quick Access Buttons](#quick-access-buttons)
    - [Context Menu Options](#context-menu-options)
  - [Plugin Settings](#plugin-settings)
    - [App Path](#app-path)
    - [App Version](#app-version)
    - [Custom Command Line Arguments](#custom-command-line-arguments)
    - [Menus](#menus)
    - [Directory Context Menu](#directory-context-menu)
    - [Debug](#debug)
  - [Legal](#legal)

## Installation

On Windows-based platforms, this plugin attempts to automatically detect the installation of OneCommander if not performed as a portable install. If you have installed OneCommander to a custom location, you can manually specify the path to the OneCommander executable in the [plugin settings](#plugin-settings).

This plugin has built-in support for versions 3.16.3+, and partial support for prior releases with varying levels of functionality. If you are using an older version of OneCommander, you may need to pick `Legacy` as the [app version](#app-version).

This plugin is compatible with Unity 2018.3 and above.

Don't have OneCommander? Download it here: [https://onecommander.com](https://onecommander.com)

## Usage

Once [setup](#installation), you can use the [quick access buttons](#quick-access-buttons) and [context menu options](#context-menu-options) to quickly and easily view paths in OneCommander, or any other file manager, utilising extensive custom configuration options.

### Quick Access Buttons

Hover over any file or folder in the Project window, and you will see a set of quick access buttons appear in the top right corner of the asset. Clicking any of these buttons will open the path in OneCommander. As with all controls, hover over the buttons to see a tooltip with information about what each button does.

![Quick Access Buttons](https://github.com/Neonalig/OneCommander-Connector-for-Unity/blob/main/Resources/Documentation/QuickAccessButtons.png?raw=true)

### Context Menu Options

Right-click on any file or folder in the Project window, and you will see a `Show in OneCommander` option appear in the context menu. Clicking this option will open the path in OneCommander.

![Context Menu Options](https://github.com/Neonalig/OneCommander-Connector-for-Unity/blob/main/Resources/Documentation/ContextMenu.png?raw=true)

## Plugin Settings

The plugin settings can be accessed from the Unity toolbar, under `Edit > Preferences > OneCommander`.

![Plugin Settings](https://github.com/Neonalig/OneCommander-Connector-for-Unity/blob/main/Resources/Documentation/PreferencesLabelled.png?raw=true)

### App Path

①: The path to the OneCommander executable. This is automatically detected on Windows-based platforms via the Windows Registry, but can be manually specified if you have installed OneCommander to a custom location, or are using a non-Windows platform.

### App Version

②: The version of OneCommander you are using. This can be considered as preset configuration options for the command line arguments used to open the file explorer. If you are using an older version of OneCommander, you may need to pick `Legacy` as the app version. If you are not using OneCommander, you can pick `Custom` and specify your own command line arguments below (③).

### Custom Command Line Arguments

③: The command line arguments used to open the file explorer. This is only used if you have picked `Custom` as the [app version](#app-version). The following placeholders are available:

| Placeholder | Description |
| --- | --- |
| $1 | The path to the file or folder to open in the file explorer. |

### Menus

④: Whether to enable the `Show in OneCommander` context menu option.

⑤: Whether to enable the quick access buttons.

### Directory Context Menu

⑥: How to manage folders for the `Show in OneCommander` context menu option, if enabled.

- `Highlight in Parent`: Open the parent folder of the selected folder in OneCommander, and highlight the selected folder.
- `Open Normally`: Open the selected folder in OneCommander.

### Debug

⑦: Whether to enable debug logging. This can be useful for troubleshooting issues with the plugin.

- `Verbose`: Enable verbose debug logging.
- `Warning`: Enable warning debug logging.
- `Error`: Enable error debug logging.

## Legal

This is a third-party plugin, and is not affiliated with Unity Technologies or OneCommander. For help and support, please [contact the plugin developer](mailto:codychook@gmail.com), not OneCommander. Permission was granted by OneCommander to use the OneCommander logo and name in this plugin.
