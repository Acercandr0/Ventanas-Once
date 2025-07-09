# Ventanas Once 3.0 🦅

#### ⚠️ README FIRST ⚠️
- The Start Menu and Action Center are configured for a 2880x1800 pixel resolution with 200% scaling.

- The Start Menu's styling is **specifically for Windows 11's new design** (Insider program), using updated targets, so it might not work correctly with the older Start Menu layout.

- If your screen has a different resolution (for example, 1920x1080), you'll need to adjust the targets and styles that affect their position to ensure correct functionality and proper display.

#### Table of contents
* [🔗 Links](#-links)
* [📷 Previews](#-previews)
* [🦅 Windhawk Mods](#-windhawk-mods)
    * [1. Translucent Windows](#1-translucent-windows)
    * [2. Windows 11 File Explorer Styler](#2-windows-11-file-explorer-styler)
    * [2. Windows 11 Start Menu Styler](#2-windows-11-start-menu-styler)
    * [3. Windows 11 Taskbar Styler](#3-windows-11-taskbar-styler)
    * [4. Windows 11 Notification Center Styler](#4-windows-11-notification-center-styler)
    * [5. Taskbar Clock Customization](#5-taskbar-clock-customization)
    * [6. Taskbar Tray Icon Spacing](#6-taskbar-tray-icon-spacing)
    * [7. CEF/Spotify Tweaks](#7-cefspotify-tweaks)
    * [8. Disable grouping on the taskbar](#8-disable-grouping-on-the-taskbar)
    * [9. Customize Windows notifications placement](#9-customize-windows-notifications-placement)
    * [10. Dark mode context menus](#10-dark-mode-context-menus)
    * [11. Taskbar on top for Windows 11](#11-taskbar-on-top-for-windows-11)

* [🔨 Fix the dark mode text with SecureUxTheme](#-fix-the-dark-mode-text-with-secureuxtheme)
* [🦊 Firefox Theme](#-firefox-theme)


## 🔗 Links
##### [Wallpaper](https://4kwallpapers.com/black-dark/ios-13-stock-ipados-dark-green-black-background-amoled-ipad-794.html)
##### [Spicetify theme](https://github.com/sanoojes/spicetify-colorful)
##### [qBittorrent theme](https://github.com/witalihirsch/qBitTorrent-fluent-theme/tree/main/themes)
##### [Firefox theme](https://github.com/Acercandr0/Ventanas-Once/blob/main/chrome.7z)
##### [SecureUXTheme Tool](https://github.com/namazso/SecureUxTheme)
##### [Rectify 11 Themes](https://github.com/Acercandr0/Ventanas-Once/blob/main/Rectify11%20Themes.7z) You can use any dark theme for this.
##### [Start Buttons](https://github.com/Acercandr0/Ventanas-Once/blob/main/Start%20Button.7z) Make a dir called 'C:\Customization\Icons\Start Button' and unzip the start buttons here.

## 📷 Previews

![Preview 1](https://github.com/Acercandr0/Ventanas-Once/blob/main/prev1.png)

![Preview 2](https://github.com/Acercandr0/Ventanas-Once/blob/main/prev2.png)

![Preview 3](https://github.com/Acercandr0/Ventanas-Once/blob/main/prev3.png)

![Preview 4](https://github.com/Acercandr0/Ventanas-Once/blob/main/prev4.png)

![Preview 5](https://github.com/Acercandr0/Ventanas-Once/blob/main/prev5.png)

![Preview 6](https://github.com/Acercandr0/Ventanas-Once/blob/main/prev6.png)

![Preview 7](https://github.com/Acercandr0/Ventanas-Once/blob/main/prev7.png)

![Preview 8](https://github.com/Acercandr0/Ventanas-Once/blob/main/prev8.png)

## 🦅 Windhawk Mods

1. **Download and install Windhawk** from [windhawk.net](https://windhawk.net).
2. **Open Windhawk** and go to **“Explore”** in the upper right menu.
3. **Search for the mod name**, click **“Details”**, and then **“Install”**. Accept any pop-ups.
4. **Go to the mod’s “Advanced” tab** and **paste the provided JSON configuration**.
5. **Apply the changes** and restart any affected applications if necessary.

Follow 3-4-5 steps for **each mod** mentioned:

### 1. Translucent Windows
```json
{
  "ThemeBackground": 1,
  "type": "acrylicblur",
  "ExtendFrame": 1,
  "TitlebarColor.ColorTitlebar": 0,
  "TitlebarColor.titlerbarstyles_active": "",
  "TitlebarColor.titlerbarstyles_inactive": "",
  "TitlebarTextColor.ColorTitlebarText": 0,
  "TitlebarTextColor.titlerbarcolorstyles_active": "",
  "TitlebarTextColor.titlerbarcolorstyles_inactive": "",
  "BorderColor.ColorBorder": 1,
  "BorderColor.borderstyles_active": "0",
  "BorderColor.borderstyles_inactive": "0",
  "BorderColor.MenuBorderColor": 0,
  "TextAlphaBlend": 0,
  "AccentBlurBehind": "b3000000",
  "ImmersiveDarkTitle": 1,
  "CornerOption": "default",
  "RainbowSpeed": 1,
  "BorderColor.RainbowBorder": 0,
  "TitlebarColor.RainbowTitlebar": 0,
  "RuledPrograms[0].target": "olk.exe",
  "RuledPrograms[0].type": "acrylicblur",
  "RuledPrograms[0].BorderColor.ColorBorder": 1,
  "RuledPrograms[0].BorderColor.borderstyles_active": "0",
  "RuledPrograms[0].BorderColor.borderstyles_inactive": "0"
}
```

### 2. Windows 11 File Explorer Styler
```json
{
  "theme": "",
  "controlStyles[0].target": "Microsoft.UI.Xaml.Controls.AppBarSeparator",
  "controlStyles[0].styles[0]": "Visibility=Collapsed",
  "controlStyles[1].target": "Grid#DetailsViewControlRootGrid",
  "controlStyles[1].styles[0]": "Background=Transparent",
  "controlStyles[2].target": "StackPanel#DetailsViewThumbnail",
  "controlStyles[2].styles[0]": "Background=Transparent",
  "controlStyles[3].target": "Grid#CommandBarControlRootGrid",
  "controlStyles[3].styles[0]": "Background=Transparent",
  "controlStyles[3].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[4].target": "FileExplorerExtensions.GalleryViewControl#GalleryViewControl > Grid",
  "controlStyles[4].styles[0]": "Background=Transparent",
  "controlStyles[5].target": "FileExplorerExtensions.GalleryViewControl#GalleryViewControl > Grid > Grid#GalleryRootGrid",
  "controlStyles[5].styles[0]": "Background=Transparent",
  "controlStyles[6].target": "TabViewItem > Grid#LayoutRoot > Canvas > Microsoft.UI.Xaml.Shapes.Path#SelectedBackgroundPath",
  "controlStyles[6].styles[0]": "Fill=Transparent",
  "controlStyles[7].target": "Microsoft.UI.Xaml.Controls.Grid#NavigationBarControlGrid",
  "controlStyles[7].styles[0]": "Background=Transparent",
  "controlStyles[8].target": "CommandBar#FileExplorerCommandBar",
  "controlStyles[8].styles[0]": "Background=Transparent",
  "controlStyles[9].target": "Microsoft.UI.Xaml.Controls.Border#RightBottomBorderLine",
  "controlStyles[9].styles[0]": "Visibility=Collapsed",
  "controlStyles[10].target": "Microsoft.UI.Xaml.Controls.Border#LeftBottomBorderLine",
  "controlStyles[10].styles[0]": "Visibility=Collapsed",
  "controlStyles[11].target": "Microsoft.UI.Xaml.Controls.Border#BottomBorderLine",
  "controlStyles[11].styles[0]": "Visibility=Collapsed",
  "controlStyles[12].target": "TabViewItem > Grid#LayoutRoot > Grid#TabContainer",
  "controlStyles[12].styles[0]": "BorderBrush=Transparent",
  "controlStyles[12].styles[1]": "Background=Transparent"
}
```

### 2. Windows 11 Start Menu Styler
⚠️ This json only work with the NEW Windows 11 StartMenu.
```json
{
  "controlStyles[0].target": "Windows.UI.Xaml.Controls.Border#BorderElement",
  "controlStyles[0].styles[0]": "Background=Transparent",
  "controlStyles[1].target": "Windows.UI.Xaml.Controls.Border#StartDropShadow",
  "controlStyles[1].styles[0]": "Visibility=Collapsed",
  "controlStyles[2].target": "Border#AcrylicBorder",
  "controlStyles[2].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.5\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[2].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[3].target": "Windows.UI.Xaml.Controls.Border#AcrylicOverlay",
  "controlStyles[3].styles[0]": "Background=Transparent",
  "controlStyles[4].target": "Windows.UI.Xaml.Controls.Grid#UnderlineContainer",
  "controlStyles[4].styles[0]": "Visibility=Collapsed",
  "controlStyles[5].target": "Windows.UI.Xaml.Controls.Border#dropshadow",
  "controlStyles[5].styles[0]": "Visibility=Collapsed",
  "controlStyles[6].target": "Windows.UI.Xaml.Controls.Grid#FrameRoot",
  "controlStyles[6].styles[0]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"-368\" />",
  "controlStyles[6].styles[1]": "MaxHeight=500",
  "controlStyles[7].target": "Windows.UI.Xaml.Controls.SemanticZoom#TopLevelRoot",
  "controlStyles[7].styles[0]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"368\" />",
  "controlStyles[8].target": "Windows.UI.Xaml.Controls.Border#RightCompanionDropShadow",
  "controlStyles[8].styles[0]": "Visibility=Collapsed",
  "controlStyles[9].target": "Windows.UI.Xaml.Controls.Border#AppBorder",
  "controlStyles[9].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[10].target": "Windows.UI.Xaml.Controls.Border#TaskbarSearchBackground",
  "controlStyles[10].styles[0]": "Background=Transparent",
  "controlStyles[11].target": "Windows.UI.Xaml.Controls.Border#dropshadow",
  "controlStyles[11].styles[0]": "Visibility=Collapsed",
  "controlStyles[3].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[12].target": "Windows.UI.Xaml.Controls.Grid#UserTileIcon",
  "controlStyles[12].styles[0]": "Width=36",
  "controlStyles[12].styles[1]": "Height=36",
  "controlStyles[9].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[13].target": "Windows.UI.Xaml.Controls.Border#LayerBorder",
  "controlStyles[13].styles[0]": "Visibility=Collapsed",
  "controlStyles[14].target": "StartMenu.FolderModal",
  "controlStyles[14].styles[0]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"368\" />",
  "controlStyles[15].target": "Windows.UI.Xaml.Controls.Border",
  "controlStyles[15].styles[0]": "BorderThickness=0,0,0,0"
}
```

### 3. Windows 11 Taskbar Styler  
```json
{
  "theme": "",
  "styleConstants[0]": "",
  "resourceVariables[0].variableKey": "",
  "resourceVariables[0].value": "",
  "controlStyles[0].target": "Taskbar.TaskListLabeledButtonPanel#IconPanel",
  "controlStyles[0].styles[0]": "MaxWidth=30",
  "controlStyles[0].styles[1]": "Padding=0",
  "controlStyles[1].target": "Windows.UI.Xaml.Controls.Image#Icon",
  "controlStyles[1].styles[0]": "Margin=-10,0,0,0",
  "controlStyles[2].target": "Taskbar.TaskListLabeledButtonPanel@RunningIndicatorStates > Rectangle#RunningIndicator",
  "controlStyles[2].styles[0]": "Margin=-10,0,0,0",
  "controlStyles[2].styles[1]": "Width@ActiveRunningIndicator=20",
  "controlStyles[2].styles[2]": "Height=2",
  "controlStyles[2].styles[3]": "Width@InactiveRunningIndicator=7",
  "controlStyles[3].target": "Taskbar.ExperienceToggleButton#LaunchListButton[AutomationProperties.AutomationId=StartButton] > Taskbar.TaskListButtonPanel@CommonStates > Border#BackgroundElement",
  "controlStyles[3].styles[0]": "Background@InactiveNormal:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Normal.png\" />",
  "controlStyles[3].styles[1]": "Background@InactivePointerOver:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Hover.png\" />",
  "controlStyles[3].styles[2]": "Background@InactivePressed:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Pressed.png\" />",
  "controlStyles[3].styles[3]": "BorderThickness=0",
  "controlStyles[3].styles[4]": "Background@ActiveNormal:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Pressed.png\" />",
  "controlStyles[3].styles[5]": "Background@ActivePointerOver:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Hover.png\" />",
  "controlStyles[3].styles[6]": "Background@ActivePressed:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Pressed.png\" />",
  "controlStyles[3].styles[7]": "MaxWidth=13",
  "controlStyles[3].styles[8]": "MaxHeight=13",
  "controlStyles[3].styles[9]": "CornerRadius=0",
  "controlStyles[4].target": "Taskbar.ExperienceToggleButton#LaunchListButton[AutomationProperties.AutomationId=StartButton] > Taskbar.TaskListButtonPanel > Microsoft.UI.Xaml.Controls.AnimatedVisualPlayer#Icon",
  "controlStyles[4].styles[0]": "Visibility=Collapsed",
  "controlStyles[5].target": "SystemTray.OmniButton#NotificationCenterButton > Grid > ContentPresenter > ItemsPresenter > StackPanel > ContentPresenter > SystemTray.IconView#SystemTrayIcon > Grid > Grid > SystemTray.TextIconContent",
  "controlStyles[5].styles[0]": "Visibility=Collapsed",
  "controlStyles[6].target": "Taskbar.TaskbarFrame > Grid#RootGrid > Taskbar.TaskbarBackground > Grid > Rectangle#BackgroundFill",
  "controlStyles[7].target": "SystemTray.Stack#NonActivatableStack",
  "controlStyles[7].styles[0]": "Visibility=Collapsed",
  "controlStyles[8].target": "Windows.UI.Xaml.Controls.Image",
  "controlStyles[8].styles[0]": "MaxHeight=15",
  "controlStyles[8].styles[1]": "MaxWidth=15",
  "controlStyles[9].target": "Taskbar.TaskbarFrame#TaskbarFrame",
  "controlStyles[9].styles[0]": "Height=32",
  "controlStyles[10].target": "SystemTray.SystemTrayFrame",
  "controlStyles[10].styles[0]": "Height=32",
  "controlStyles[11].target": "Taskbar.ExperienceToggleButton#LaunchListButton",
  "controlStyles[11].styles[0]": "Width=50",
  "controlStyles[11].styles[1]": "Margin=-5,0,0,0",
  "controlStyles[12].target": "Windows.UI.Xaml.Controls.Image#OverlayIcon",
  "controlStyles[12].styles[0]": "Transform3D:=<CompositeTransform3D ScaleX=\"0.6\" ScaleY=\"0.6\" ScaleZ=\"0.6\" />",
  "controlStyles[12].styles[1]": "Margin=10,2,0,0",
  "controlStyles[13].target": "Taskbar.Badge#BadgeControl",
  "controlStyles[13].styles[0]": "Transform3D:=<CompositeTransform3D ScaleX=\"0.6\" ScaleY=\"0.6\" ScaleZ=\"0.6\" />",
  "controlStyles[13].styles[1]": "Margin=10,2,0,0",
  "controlStyles[14].target": "Microsoft.UI.Xaml.Controls.ProgressBar#ProgressIndicator",
  "controlStyles[14].styles[0]": "Margin=-10,0,0,0",
  "controlStyles[6].styles[0]": "Fill:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />"
}
```
⚠️ **Note:** The icons used for the [Start Buttons](https://github.com/Acercandr0/Ventanas-Once/blob/main/Start%20Button.7z) are stored in `C:\Customization\Icons\Start Button\`.  

### 4. Windows 11 Notification Center Styler
```json
{
  "controlStyles[0].target": "Grid#NotificationCenterGrid",
  "controlStyles[0].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.5\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[0].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[0].styles[2]": "Shadow:=",
  "controlStyles[0].styles[3]": "VerticalAlignment=Stretch",
  "controlStyles[1].target": "Grid#CalendarCenterGrid",
  "controlStyles[1].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.5\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[1].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[1].styles[2]": "Shadow:=",
  "controlStyles[2].target": "ScrollViewer#CalendarControlScrollViewer",
  "controlStyles[2].styles[0]": "Background:=<AcrylicBrush Opacity=\"0\"/>",
  "controlStyles[3].target": "Border#CalendarHeaderMinimizedOverlay",
  "controlStyles[3].styles[0]": "Background:=<AcrylicBrush Opacity=\"0\"/>",
  "controlStyles[4].target": "ActionCenter.FocusSessionControl#FocusSessionControl > Grid#FocusGrid",
  "controlStyles[4].styles[0]": "Background:=<AcrylicBrush Opacity=\"0\"/>",
  "controlStyles[5].target": "MenuFlyoutPresenter",
  "controlStyles[5].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.5\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[5].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[5].styles[2]": "Padding=2,4,2,4",
  "controlStyles[5].styles[3]": "Shadow:=",
  "controlStyles[6].target": "Border#JumpListRestyledAcrylic",
  "controlStyles[6].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.5\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[6].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[6].styles[2]": "Margin=-2,-2,-2,-2",
  "controlStyles[6].styles[3]": "Shadow:=",
  "controlStyles[7].target": "Grid#ControlCenterRegion",
  "controlStyles[7].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.5\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[7].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[7].styles[2]": "Margin=0,0,0,460",
  "controlStyles[7].styles[3]": "Shadow:=",
  "controlStyles[8].target": "Windows.UI.Xaml.Controls.Grid#L1Grid > Border",
  "controlStyles[8].styles[0]": "Background:=<SolidColorBrush Color=\"Transparent\"/>",
  "controlStyles[9].target": "Windows.UI.Xaml.Controls.Grid#MediaTransportControlsRegion",
  "controlStyles[9].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.5\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[9].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[9].styles[2]": "Margin=0,12,0,-950",
  "controlStyles[9].styles[3]": "Shadow:=",
  "controlStyles[10].target": "Grid#MediaTransportControlsRoot",
  "controlStyles[10].styles[0]": "Background:=<SolidColorBrush Color=\"Transparent\"/>",
  "controlStyles[11].target": "ContentPresenter#PageContent",
  "controlStyles[11].styles[0]": "Background:=<SolidColorBrush Color=\"Transparent\"/>",
  "controlStyles[12].target": "ContentPresenter#PageContent > Grid > Border",
  "controlStyles[12].styles[0]": "Background:=<SolidColorBrush Color=\"Transparent\"/>",
  "controlStyles[13].target": "QuickActions.ControlCenter.AccessibleWindow#PageWindow > ContentPresenter > Grid#FullScreenPageRoot",
  "controlStyles[13].styles[0]": "Background:=<SolidColorBrush Color=\"Transparent\"/>",
  "controlStyles[14].target": "QuickActions.ControlCenter.AccessibleWindow#PageWindow > ContentPresenter > Grid#FullScreenPageRoot > ContentPresenter#PageHeader",
  "controlStyles[14].styles[0]": "Background:=<SolidColorBrush Color=\"Transparent\"/>",
  "controlStyles[15].target": "Windows.UI.Xaml.Controls.Grid#ThumbnailImage",
  "controlStyles[15].styles[0]": "RenderTransform:=<ScaleTransform ScaleX=\"1.2\" ScaleY=\"1.2\" />",
  "controlStyles[15].styles[1]": "RenderTransformOrigin=0.5,0.5",
  "controlStyles[16].target": "Windows.UI.Xaml.Controls.ListView#MediaButtonsListView",
  "controlStyles[16].styles[0]": "RenderTransform:=<ScaleTransform ScaleX=\"0.9\" ScaleY=\"0.9\" />",
  "controlStyles[16].styles[1]": "RenderTransformOrigin=0.5,0.5"
}
```

### 5. Taskbar Clock Customization  
```json
{"ShowSeconds":0,"TimeFormat":"h':'mm tt","DateFormat":"d 'de' MMMM","WeekdayFormat":"dddd","WeekdayFormatCustom":"","TopLine":"%date%  %time%","BottomLine":"","MiddleLine":"","TooltipLine":"","Width":180,"Height":60,"MaxWidth":0,"TextSpacing":-1,"oldTaskbarOnWin11":0}
```
**⚠️ Note:** Change date format to your language or leave it in spanish, it's your call.

### 6. Taskbar Tray Icon Spacing
```json
{"notificationIconWidth":25,"overflowIconWidth":30,"overflowIconsPerRow":5}
```

### 7. CEF/Spotify Tweaks
This mod will help with navigations buttons transparency with Spicetify themes.
```json
{
  "showframe": 0,
  "showframeonothers": 0,
  "showmenu": 1,
  "showcontrols": 1,
  "transparentcontrols": 1,
  "transparentrendering": 0,
  "noforceddarkmode": 0,
  "forceextensions": 0,
  "ignoreminsize": 0,
  "allowuntested": 1,
  "playbackspeed": "1"
}
```

### 8. Disable grouping on the taskbar
No config, use Settings tab.

### 9. Customize Windows notifications placement
No config, use Settings tab.

### 10. Dark mode context menus
No config, use Settings tab.

### 11. Taskbar on top for Windows 11
No config, use Settings tab.


## 🔨 Fix the dark mode text with SecureUxTheme
1. Unzip Rectify11 themes in 'C:\Windows\Resources\Themes'
2. Run SecureUxTheme Tool as administrator.
3. Check 'Hook SystemSettings', 'Hook LogonUI' and 'Remove DefaultColors"
4. Install and reboot.
5. 2. Run SecureUxTheme Tool again.
6. Select 'Rectify11 dark theme" and click on "patch and apply",

## 🦊 Firefox Theme

1.  Open your browser and type `about:profiles` into the address bar, then hit Enter.
2.  Find your root profile folder (usually labeled "**Root Directory**") and click the "**Open Folder**" button next to it.
3.  Once the folder opens, **unzip** the contents of [chrome.7z](https://github.com/Acercandr0/Ventanas-Once/blob/main/chrome.7z) directly into this folder, **replacing existing files if necessary**.
4.  Now, type `about:config` into the address bar and hit Enter. **Accept the warning** if it appears.
5.  In the search bar within `about:config`, search for and **set the following preferences to `true`** (you can do this by double-clicking on them or toggling their value):
    * `widget.windows.mica`
    * `browser.theme.native-theme`
    * `browser.tabs.allow_transparent_browser`
    * `toolkit.legacyUserProfileCustomizations.enabled`
6.  **Restart Firefox** for the changes to take effect.

### That's it. Enjoy! 🍸
