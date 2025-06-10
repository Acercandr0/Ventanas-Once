# Ventanas Once 🦅 Windhawk config

### 🔍 Readme first

• The Action Center is positioned at the top of the screen and configured for a 2880x1800 px resolution. If your screen has a different resolution, you will need to adjust the margin values accordingly to ensure a proper fit.  
• For **1920x1080 resolution**, you can find a solution [here](https://github.com/ramensoftware/windhawk-mods/issues/1053#issuecomment-2954166046).
• It's also a good idea to install StartAllBack to fix some UI inconsistencies in Windows dark mode.

### 🔗 Wallpaper
[Link](https://4kwallpapers.com/black-dark/ios-13-stock-ipados-dark-green-black-background-amoled-ipad-794.html)
### 🔗 Spicetify theme
[Link](https://github.com/spicetify/spicetify-themes/tree/master/Sleek)
### 🔗 qBittorrent theme (fluent-dark.qbtheme)
[Link](https://github.com/witalihirsch/qBitTorrent-fluent-theme/tree/main/themes)


## 📷 Preview

![Preview 1](https://github.com/Acercandr0/Ventanas-Once/blob/main/Preview1.png)

![Preview 2](https://github.com/Acercandr0/Ventanas-Once/blob/main/Preview2.png)

![Preview 3](https://github.com/Acercandr0/Ventanas-Once/blob/main/Preview3.png)

![Preview 4](https://github.com/Acercandr0/Ventanas-Once/blob/main/Preview4.png)

![Preview 5](https://github.com/Acercandr0/Ventanas-Once/blob/main/Preview5.png)

![Preview 6](https://github.com/Acercandr0/Ventanas-Once/blob/main/Preview6.png)

### 🦅 Steps to Install Windhawk and Apply the Mods

Follow these steps for **each mod** mentioned:

1. **Download and install Windhawk** from [windhawk.net](https://windhawk.net).
2. **Open Windhawk** and go to **“Explore”** in the upper right menu.
3. **Search for the mod name**, click **“Details”**, and then **“Install”**. Accept any pop-ups.
4. **Go to the mod’s “Advanced” tab** and **paste the provided JSON configuration**.
5. **Apply the changes** and restart any affected applications if necessary.

Repeat these steps for each mod you want to install.



### 1. Translucent Windows
```json
{
  "ThemeBackground": 0,
  "type": "none",
  "ExtendFrame": 0,
  "TitlebarColor": {
    "ColorTitlebar": 0,
    "titlerbarstyles_active": "FF0000",
    "titlerbarstyles_inactive": "00FFFF"
  },
  "TitlebarTextColor": {
    "ColorTitlebarText": 0,
    "titlerbarcolorstyles_active": "FF0000",
    "titlerbarcolorstyles_inactive": "00FFFF"
  },
  "BorderColor": {
    "ColorBorder": 0,
    "borderstyles_active": "0",
    "borderstyles_inactive": "00FFFF",
    "MenuBorderColor": 0,
    "RainbowBorder": 0
  },
  "TextAlphaBlend": 0,
  "AccentBlurBehind": "",
  "ImmersiveDarkTitle": 0,
  "CornerOption": "default",
  "RainbowSpeed": 1,
  "RuledPrograms": [
    {
      "target": "explorer.exe",
      "ThemeBackground": 1,
      "TextAlphaBlend": 1,
      "AccentBlurBehind": "B3000000",
      "type": "acrylicblur",
      "ExtendFrame": 1,
      "ImmersiveDarkTitle": 0,
      "TitlebarColor": {
        "ColorTitlebar": 0
      },
      "BorderColor": {
        "ColorBorder": 1,
        "borderstyles_active": "0",
        "borderstyles_inactive": "0"
      },
      "TitlebarTextColor": {
        "ColorTitlebarText": 0,
        "titlerbarcolorstyles_active": ""
      }
    },
    {
      "target": "notepad.exe",
      "TextAlphaBlend": 0,
      "ThemeBackground": 0,
      "type": "acrylicsystem",
      "ImmersiveDarkTitle": 1,
      "ExtendFrame": 0,
      "AccentBlurBehind": "",
      "BorderColor": {
        "ColorBorder": 1,
        "borderstyles_active": "0",
        "borderstyles_inactive": "0"
      }
    },
    {
      "target": "qbittorrent.exe",
      "type": "acrylicblur",
      "ImmersiveDarkTitle": 0,
      "AccentBlurBehind": "B3000000",
      "ThemeBackground": 1,
      "ExtendFrame": 1,
      "TextAlphaBlend": 1,
      "BorderColor": {
        "ColorBorder": 1,
        "borderstyles_active": "0",
        "borderstyles_inactive": "0"
      }
    }
  ]
}
```

### 2. Windows 11 File Explorer Styler
```json
{
  "controlStyles[0].target": "Microsoft.UI.Xaml.Controls.AppBarSeparator",
  "controlStyles[0].styles[0]": "Visibility=Collapsed",
  "controlStyles[1].target": "Grid#DetailsViewControlRootGrid",
  "controlStyles[1].styles[0]": "Background=Transparent",
  "controlStyles[2].target": "StackPanel#DetailsViewThumbnail",
  "controlStyles[2].styles[0]": "Background=Transparent",
  "controlStyles[3].target": "Grid#CommandBarControlRootGrid",
  "controlStyles[3].styles[0]": "Background=Transparent",
  "controlStyles[3].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[4].target": "CommandBar#FileExplorerCommandBar",
  "controlStyles[4].styles[0]": "Background=Transparent"
}
```

### 3. Windows 11 Notification Center Styler  
```json
{
  "controlStyles[0].target": "Grid#NotificationCenterGrid",
  "controlStyles[0].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[0].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[0].styles[2]": "Shadow:=",

  "controlStyles[1].target": "Grid#CalendarCenterGrid",
  "controlStyles[1].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[1].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[1].styles[2]": "Shadow:=",

  "controlStyles[2].target": "ScrollViewer#CalendarControlScrollViewer",
  "controlStyles[2].styles[0]": "Background:=<AcrylicBrush Opacity=\"0\"/>",

  "controlStyles[3].target": "Border#CalendarHeaderMinimizedOverlay",
  "controlStyles[3].styles[0]": "Background:=<AcrylicBrush Opacity=\"0\"/>",

  "controlStyles[4].target": "ActionCenter.FocusSessionControl#FocusSessionControl > Grid#FocusGrid",
  "controlStyles[4].styles[0]": "Background:=<AcrylicBrush Opacity=\"0\"/>",

  "controlStyles[5].target": "MenuFlyoutPresenter",
  "controlStyles[5].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[5].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[5].styles[2]": "Padding=2,4,2,4",
  "controlStyles[5].styles[3]": "Shadow:=",

  "controlStyles[6].target": "Border#JumpListRestyledAcrylic",
  "controlStyles[6].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[6].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[6].styles[2]": "Margin=-2,-2,-2,-2",

  "controlStyles[7].target": "Grid#ControlCenterRegion",
  "controlStyles[7].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[7].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[7].styles[2]": "Margin=0,0,0,460",
  "controlStyles[7].styles[3]": "Shadow:=",

  "controlStyles[8].target": "Windows.UI.Xaml.Controls.Grid#L1Grid > Border",
  "controlStyles[8].styles[0]": "Background:=<SolidColorBrush Color=\"Transparent\"/>",

  "controlStyles[9].target": "Windows.UI.Xaml.Controls.Grid#MediaTransportControlsRegion",
  "controlStyles[9].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[9].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[9].styles[2]": "Margin=0,12,0,-960",
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
  "controlStyles[14].styles[0]": "Background:=<SolidColorBrush Color=\"Transparent\"/>"
}
```
### 4. Customize Windows notifications placement  
```json
{"monitor":1,"monitorInterfaceName":"","horizontalPlacement":"right","horizontalDistanceFromScreenEdge":0,"verticalPlacement":"top","verticalDistanceFromScreenEdge":-20}
```

### 5. Taskbar on Top for Windows 11  
No config. Just set it to top.

### 6. Windows 11 Start Menu Styler
```json
{
  "controlStyles[0].target": "Windows.UI.Xaml.Controls.Grid#RootPanel",
  "controlStyles[0].styles[0]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"-148\" />",
  "controlStyles[0].styles[1]": "MaxHeight=430",

  "controlStyles[1].target": "Windows.UI.Xaml.Controls.Grid#TopLevelSuggestionsListHeader",
  "controlStyles[1].styles[0]": "Visibility=Collapsed",

  "controlStyles[2].target": "Windows.UI.Xaml.Controls.Grid#NoTopLevelSuggestionsText",
  "controlStyles[2].styles[0]": "Visibility=Collapsed",

  "controlStyles[3].target": "Windows.UI.Xaml.Controls.Grid#TopLevelSuggestionsContainer",
  "controlStyles[3].styles[0]": "Visibility=Collapsed",

  "controlStyles[4].target": "Windows.UI.Xaml.Controls.Grid#ShowMoreSuggestions",
  "controlStyles[4].styles[0]": "Visibility=Collapsed",

  "controlStyles[5].target": "Windows.UI.Xaml.Controls.Grid#UndockedRoot",
  "controlStyles[5].styles[0]": "Margin=0,0,0,0",

  "controlStyles[6].target": "Windows.UI.Xaml.Controls.TextBlock#PinnedListHeaderText",
  "controlStyles[6].styles[0]": "Visibility=Collapsed",

  "controlStyles[7].target": "StartDocked.PowerOptionsView",
  "controlStyles[7].styles[0]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"140\" />",

  "controlStyles[8].target": "StartDocked.UserTileView#UserTile",
  "controlStyles[8].styles[0]": "Visibility=Collapsed",

  "controlStyles[9].target": "StartDocked.AppListView#NavigationPanePlacesListView",
  "controlStyles[9].styles[0]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"140\" />",

  "controlStyles[10].target": "Windows.UI.Xaml.Controls.Grid#MainContent",
  "controlStyles[10].styles[0]": "Margin=0,0,0,0",

  "controlStyles[11].target": "Windows.UI.Xaml.Controls.Border#BorderElement",
  "controlStyles[11].styles[0]": "Background=Transparent",

  "controlStyles[12].target": "Windows.UI.Xaml.Controls.Border#RootGridDropShadow",
  "controlStyles[12].styles[0]": "Visibility=Collapsed",

  "controlStyles[13].target": "Windows.UI.Xaml.Controls.Border#RightCompanionDropShadow",
  "controlStyles[13].styles[0]": "Visibility=Collapsed",

  "controlStyles[14].target": "Border#AcrylicBorder",
  "controlStyles[14].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[14].styles[1]": "BorderThickness=0,0,0,0",

  "controlStyles[15].target": "Windows.UI.Xaml.Controls.Border#AcrylicOverlay",
  "controlStyles[15].styles[0]": "Visibility=Collapsed",

  "controlStyles[16].target": "Windows.UI.Xaml.Controls.Button#ShowAllAppsButton",
  "controlStyles[16].styles[0]": "Visibility=Collapsed",

  "controlStyles[17].target": "StartMenu.PinnedList#StartMenuPinnedList",
  "controlStyles[17].styles[0]": "RenderTransform:=<TranslateTransform X=\"0\" Y=\"-40\" />",

  "controlStyles[18].target": "Windows.UI.Xaml.Controls.Grid#UnderlineContainer",
  "controlStyles[18].styles[0]": "Visibility=Collapsed",

  "controlStyles[19].target": "Border#AppBorder",
  "controlStyles[19].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[19].styles[1]": "BorderThickness=0,0,0,0",

  "controlStyles[20].target": "Windows.UI.Xaml.Controls.Border#dropshadow",
  "controlStyles[20].styles[0]": "Visibility=Collapsed",

  "controlStyles[21].target": "Windows.UI.Xaml.Controls.Border#LayerBorder",
  "controlStyles[21].styles[0]": "Visibility=Collapsed",

  "controlStyles[22].target": "Windows.UI.Xaml.Controls.Border#TaskbarSearchBackground",
  "controlStyles[22].styles[0]": "Background=Transparent"
}
```

### 7. Windows 11 Taskbar Styler  
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
  "controlStyles[2].styles[2]": "Fill@InactiveRunningIndicator=#33FFFFFF",
  "controlStyles[2].styles[3]": "Height=2",
  "controlStyles[2].styles[4]": "Width@InactiveRunningIndicator=10",
  
  "controlStyles[3].target": "Taskbar.ExperienceToggleButton#LaunchListButton[AutomationProperties.AutomationId=StartButton] > Taskbar.TaskListButtonPanel@CommonStates > Border#BackgroundElement",
  "controlStyles[3].styles[0]": "Background@InactiveNormal:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Normal.png\" />",
  "controlStyles[3].styles[1]": "Background@InactivePointerOver:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Hover.png\" />",
  "controlStyles[3].styles[2]": "Background@InactivePressed:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Pressed.png\" />",
  "controlStyles[3].styles[3]": "BorderThickness=0",
  "controlStyles[3].styles[4]": "Background@ActiveNormal:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Pressed.png\" />",
  "controlStyles[3].styles[5]": "Background@ActivePointerOver:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Hover.png\" />",
  "controlStyles[3].styles[6]": "Background@ActivePressed:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Pressed.png\" />",
  "controlStyles[3].styles[7]": "MaxWidth=15",
  "controlStyles[3].styles[8]": "MaxHeight=15",
  "controlStyles[3].styles[9]": "CornerRadius=0",
  
  "controlStyles[4].target": "Taskbar.ExperienceToggleButton#LaunchListButton[AutomationProperties.AutomationId=StartButton] > Taskbar.TaskListButtonPanel > Microsoft.UI.Xaml.Controls.AnimatedVisualPlayer#Icon",
  "controlStyles[4].styles[0]": "Visibility=Collapsed",
  
  "controlStyles[5].target": "SystemTray.OmniButton#NotificationCenterButton > Grid > ContentPresenter > ItemsPresenter > StackPanel > ContentPresenter > SystemTray.IconView#SystemTrayIcon > Grid > Grid > SystemTray.TextIconContent",
  "controlStyles[5].styles[0]": "Visibility=Collapsed",
  
  "controlStyles[6].target": "Taskbar.TaskbarFrame > Grid#RootGrid > Taskbar.TaskbarBackground > Grid > Rectangle#BackgroundFill",
  "controlStyles[6].styles[0]": "Fill:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.3\" />",
  
  "controlStyles[7].target": "Rectangle#BackgroundStroke",
  "controlStyles[7].styles[0]": "Visibility=Collapsed",
  
  "controlStyles[8].target": "SystemTray.Stack#NonActivatableStack",
  "controlStyles[8].styles[0]": "Visibility=Collapsed",
  
  "controlStyles[9].target": "Windows.UI.Xaml.Controls.Image",
  "controlStyles[9].styles[0]": "MaxHeight=15",
  "controlStyles[9].styles[1]": "MaxWidth=15",
  
  "controlStyles[10].target": "Taskbar.TaskbarFrame#TaskbarFrame",
  "controlStyles[10].styles[0]": "Height=30",
  
  "controlStyles[11].target": "SystemTray.SystemTrayFrame",
  "controlStyles[11].styles[0]": "Height=30",
  
  "controlStyles[12].target": "Taskbar.ExperienceToggleButton#LaunchListButton",
  "controlStyles[12].styles[0]": "Width=50",
  "controlStyles[12].styles[1]": "Margin=-5,0,0,0",
  
  "controlStyles[13].target": "Windows.UI.Xaml.Controls.Image#OverlayIcon",
  "controlStyles[13].styles[0]": "Transform3D:=<CompositeTransform3D ScaleX=\"0.61\" ScaleY=\"0.61\" ScaleZ=\"0.61\" />",
  "controlStyles[13].styles[1]": "Margin=10,1,0,0",
  
  "controlStyles[14].target": "Taskbar.Badge#BadgeControl",
  "controlStyles[14].styles[0]": "Transform3D:=<CompositeTransform3D ScaleX=\"0.61\" ScaleY=\"0.61\" ScaleZ=\"0.61\" />",
  "controlStyles[14].styles[1]": "Margin=10,1,0,0",
  
  "controlStyles[15].target": "Microsoft.UI.Xaml.Controls.ProgressBar#ProgressIndicator",
  "controlStyles[15].styles[0]": "Margin=-10,0,0,0"
}
```
⚠️ **Note:** The icons used for the Start Button are stored in `C:\Customization\Icons\Start Button\`.  
You can **download them from the main branch** [here](https://github.com/Acercandr0/Ventanas-Once/blob/main/Start%20Button.7z) and place them in the same directory, or customize the path and button design by updating the settings accordingly.  

### 8. Taskbar Clock Customization  
```json
{"ShowSeconds":0,"TimeFormat":"h':'mm tt","DateFormat":"d 'de' MMMM","WeekdayFormat":"dddd","WeekdayFormatCustom":"","TopLine":"%date%  %time%","BottomLine":"","MiddleLine":"","TooltipLine":"","Width":180,"Height":60,"MaxWidth":0,"TextSpacing":-1,"oldTaskbarOnWin11":0}
```
**⚠️ Note:** Change date format to english or leave it in spanish, it's your call.

### 8. Taskbar Tray Icon Spacing
```json
{"notificationIconWidth":25,"overflowIconWidth":30,"overflowIconsPerRow":5}
```

### 10. CEF/Spotify Tweaks
This mod will help with navigations buttons transparency with Spicetify themes.
```json
{"showframe":0,"showframeonothers":0,"showmenu":1,"showcontrols":1,"transparentcontrols":1,"transparentrendering":0,"noforceddarkmode":0,"forceextensions":0,"ignoreminsize":0,"allowuntested":0,"playbackspeed":"1"}
```

### 11. Disable grouping on the taskbar (optional)
No config. Just prevents grouping.



### That's it. Enjoy! 🍸
