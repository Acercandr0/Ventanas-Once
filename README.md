# Ventanas Once 🦅 Windhawk config

## 📷 Preview

![Preview 1](https://github.com/Acercandr0/Ventanas-Once/blob/main/Preview1.png)
![Preview 2](https://github.com/Acercandr0/Ventanas-Once/blob/main/Preview2.png)
![Preview 3](https://github.com/Acercandr0/Ventanas-Once/blob/main/Preview3.png)

### Customize Windows notifications placement  
```json
{"monitor":1,"monitorInterfaceName":"","horizontalPlacement":"right","horizontalDistanceFromScreenEdge":0,"verticalPlacement":"top","verticalDistanceFromScreenEdge":-20}
```

### Taskbar Clock Customization  
```json
{"ShowSeconds":0,"TimeFormat":"h':'mm tt","DateFormat":"d 'de' MMMM","WeekdayFormat":"dddd","WeekdayFormatCustom":"","TopLine":"%date%  %time%","BottomLine":"","MiddleLine":"","TooltipLine":"","Width":180,"Height":60,"MaxWidth":0,"TextSpacing":-1,"oldTaskbarOnWin11":0}
```
**⚠️ Note:** Change date format to english or leave it in spanish, it's your call.

### Taskbar on Top for Windows 11  
Set the taskbar on top.

### Translucent Windows
```json
{
  "ThemeBackground": 0,
  "type": "none",
  "ExtendFrame": 0,
  "TitlebarColor.ColorTitlebar": 0,
  "TitlebarColor.titlerbarstyles_active": "FF0000",
  "TitlebarColor.titlerbarstyles_inactive": "00FFFF",
  "TitlebarTextColor.ColorTitlebarText": 0,
  "TitlebarTextColor.titlerbarcolorstyles_active": "FF0000",
  "TitlebarTextColor.titlerbarcolorstyles_inactive": "00FFFF",
  "BorderColor.ColorBorder": 0,
  "BorderColor.borderstyles_active": "FF0000",
  "BorderColor.borderstyles_inactive": "00FFFF",
  "BorderColor.MenuBorderColor": 0,
  "RuledPrograms[0].target": "explorer.exe",
  "RuledPrograms[0].type": "acrylicblur",
  "RuledPrograms[0].ExtendFrame": 1,
  "RuledPrograms[0].TitlebarColor.ColorTitlebar": 0,
  "RuledPrograms[0].TitlebarColor.titlerbarstyles_active": "FF0000",
  "RuledPrograms[0].TitlebarColor.titlerbarstyles_inactive": "00FFFF",
  "RuledPrograms[0].TitlebarTextColor.ColorTitlebarText": 0,
  "RuledPrograms[0].TitlebarTextColor.titlerbarcolorstyles_active": "FF0000",
  "RuledPrograms[0].TitlebarTextColor.titlerbarcolorstyles_inactive": "00FFFF",
  "RuledPrograms[0].BorderColor.ColorBorder": 0,
  "RuledPrograms[0].BorderColor.borderstyles_active": "0",
  "RuledPrograms[0].BorderColor.borderstyles_inactive": "0",
  "RuledPrograms[0].ThemeBackground": 1,
  "RuledPrograms[0].ImmersiveDarkTitle": 1,
  "RuledPrograms[0].AccentBlurBehind": "B3000000",
  "RuledPrograms[0].CornerOption": "default",
  "RuledPrograms[1].target": "qbittorrent.exe",
  "RuledPrograms[1].type": "acrylicblur",
  "RuledPrograms[1].ExtendFrame": 1,
  "RuledPrograms[1].AccentBlurBehind": "B3000000",
  "RuledPrograms[2].target": "notepad.exe",
  "RuledPrograms[2].type": "acrylicblur",
  "RuledPrograms[2].BorderColor.ColorBorder": 0,
  "RuledPrograms[2].BorderColor.borderstyles_active": "0",
  "RuledPrograms[2].BorderColor.borderstyles_inactive": "0",
  "RuledPrograms[2].AccentBlurBehind": "B3000000",
  "RuledPrograms[3].target": "mspaint.exe",
  "RuledPrograms[3].type": "acrylicsystem",
  "TextAlphaBlend": 0,
  "AccentBlurBehind": "",
  "ImmersiveDarkTitle": 0,
  "CornerOption": "default",
  "RainbowSpeed": 1
}
```

### Windows 11 File Explorer Styler
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

### Windows 11 Notification Center Styler  
```json
{
  "controlStyles[0].target": "Grid#NotificationCenterGrid",
  "controlStyles[0].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[0].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[1].target": "Grid#CalendarCenterGrid",
  "controlStyles[1].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[1].styles[1]": "BorderThickness=0,0,0,0",
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
  "controlStyles[6].target": "Border#JumpListRestyledAcrylic",
  "controlStyles[6].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[6].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[6].styles[2]": "Margin=-2,-2,-2,-2",
  "controlStyles[7].target": "Grid#ControlCenterRegion",
  "controlStyles[7].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[7].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[7].styles[2]": "Margin=0,0,0,460",
  "controlStyles[8].target": "Windows.UI.Xaml.Controls.Grid#L1Grid > Border",
  "controlStyles[8].styles[0]": "Background:=<SolidColorBrush Color=\"Transparent\"/>",
  "controlStyles[9].target": "Windows.UI.Xaml.Controls.Grid#MediaTransportControlsRegion",
  "controlStyles[9].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[9].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[9].styles[2]": "Margin=0,12,0,-960",
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
  "controlStyles[15].target": "ScrollViewer#ListContent",
  "controlStyles[15].styles[0]": "Background:=<SolidColorBrush Color=\"Transparent\"/>",
  "controlStyles[16].target": "ActionCenter.FlexibleToastView#FlexibleNormalToastView",
  "controlStyles[16].styles[0]": "Background:=<SolidColorBrush Color=\"Transparent\"/>",
  "controlStyles[17].target": "Border#ToastBackgroundBorder2",
  "controlStyles[17].styles[0]": "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.6\" BackgroundSource=\"Backdrop\" />",
  "controlStyles[17].styles[1]": "BorderThickness=0,0,0,0",
  "controlStyles[18].target": "JumpViewUI.SystemItemListViewItem > Grid#LayoutRoot > Border#BackgroundBorder",
  "controlStyles[18].styles[0]": "FocusVisualPrimaryThickness=0,0,0,0",
  "controlStyles[18].styles[1]": "FocusVisualSecondaryThickness=0,0,0,0",
  "controlStyles[19].target": "JumpViewUI.JumpListListViewItem > Grid#LayoutRoot > Border#BackgroundBorder",
  "controlStyles[19].styles[0]": "FocusVisualPrimaryThickness=0,0,0,0",
  "controlStyles[0].styles[2]": "Shadow:=",
  "controlStyles[1].styles[2]": "Shadow:=",
  "controlStyles[7].styles[3]": "Shadow:=",
  "controlStyles[5].styles[3]": "Shadow:=",
  "controlStyles[9].styles[3]": "Shadow:="
}
```

### Windows 11 Start Menu Styler
```json
{
  "controlStyles[0].target": "Windows.UI.Xaml.Controls.Grid#RootPanel",
  "controlStyles[0].styles[0]": "Margin=0,-292,0,0",
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
  "controlStyles[7].styles[0]": "Margin=-190,270,0,0",
  "controlStyles[8].target": "StartDocked.UserTileView#UserTile",
  "controlStyles[8].styles[0]": "Visibility=Collapsed",
  "controlStyles[9].target": "StartDocked.AppListView#NavigationPanePlacesListView",
  "controlStyles[9].styles[0]": "Margin=-390,270,0,0",
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
  "controlStyles[17].styles[0]": "Margin=0,-40,0,0",
  "controlStyles[18].target": "Windows.UI.Xaml.Controls.Grid#UnderlineContainer",
  "controlStyles[18].styles[0]": "Visibility=Collapsed"
}
```

### Windows 11 Taskbar Styler  
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

**⚠️ Note:** The icons used for the Start Button are stored in `C:\Customization\Icons\Start Button\`. You can download them from the main branch and place them in the same directory, or use your own custom path and button designs by updating the settings accordingly. There should be three versions: Normal, Hover, and Pressed.

### Taskbar Tray Icon Spacing
```json
{"notificationIconWidth":25,"overflowIconWidth":30,"overflowIconsPerRow":5}
```

### CEF/Spotify Tweaks ⭐
This mod will help with navigations buttons transparency with Spicetify themes!
```json
{"showframe":0,"showframeonothers":0,"showmenu":1,"showcontrols":1,"transparentcontrols":1,"transparentrendering":0,"noforceddarkmode":0,"forceextensions":0,"ignoreminsize":0,"allowuntested":0,"playbackspeed":"1"}
```

### Disable grouping on the taskbar
As it says, prevents grouping.

[Wallpaper link](https://4kwallpapers.com/black-dark/ios-13-stock-ipados-dark-green-black-background-amoled-ipad-794.html)
