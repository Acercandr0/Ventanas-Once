# Ventanas Once 3.1 🦅

#### ⚠️ README FIRST ⚠️
- The Start Menu and Action Center are configured for a 2880x1800 pixel resolution with 200% scaling.
- If your screen has a different resolution (for example, 1920x1080), you'll need to adjust the targets and styles that affect their position to ensure correct functionality and proper display.
- The Start Menu's styling is **specifically for Windows 11's new design** (Insider program), so it might not work correctly with the older Start Menu layout.

#### Table of contents
* [📷 Previews](#-previews)
* [🦅 Windhawk Mods](#-windhawk-mods)
    * [1. Translucent Windows](#1-translucent-windows)
    * [2. Windows 11 File Explorer Styler](#2-windows-11-file-explorer-styler)
    * [2. Windows 11 Start Menu Styler](#2-windows-11-start-menu-styler)
    * [3. Windows 11 Taskbar Styler](#3-windows-11-taskbar-styler)
    * [4. Windows 11 Notification Center Styler](#4-windows-11-notification-center-styler)
    * [5. Taskbar Clock Customization](#5-taskbar-clock-customization)
    * [6. Taskbar Tray Icon Spacing](#6-taskbar-tray-icon-spacing)
    * [7. Disable grouping on the taskbar](#8-disable-grouping-on-the-taskbar)
    * [8. Customize Windows notifications placement](#9-customize-windows-notifications-placement)
    * [9. Dark mode context menus](#10-dark-mode-context-menus)
    * [10. Taskbar on top for Windows 11](#11-taskbar-on-top-for-windows-11)
   
* [🦊 Firefox Theme](#-firefox-theme)

## 📷 Previews

![Preview 1](https://github.com/Acercandr0/Ventanas-Once/blob/main/Previews/prev1.png)

![Preview 2](https://github.com/Acercandr0/Ventanas-Once/blob/main/Previews/prev2.png)

![Preview 3](https://github.com/Acercandr0/Ventanas-Once/blob/main/Previews/prev3.png)

![Preview 4](https://github.com/Acercandr0/Ventanas-Once/blob/main/Previews/prev4.png)

![Preview 5](https://github.com/Acercandr0/Ventanas-Once/blob/main/Previews/prev5.png)


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
  "BorderColor.ColorBorder": 0,
  "BorderColor.borderstyles_active": "0",
  "BorderColor.borderstyles_inactive": "0",
  "BorderColor.MenuBorderColor": 0,
  "TextAlphaBlend": 1,
  "AccentBlurBehind": "B3000000",
  "ImmersiveDarkTitle": 1,
  "CornerOption": "default",
  "RainbowSpeed": 1,
  "BorderColor.RainbowBorder": 0,
  "TitlebarColor.RainbowTitlebar": 0,
  "RuledPrograms[0].target": "olk.exe",
  "RuledPrograms[0].type": "acrylicblur",
  "RuledPrograms[0].AccentBlurBehind": "A6000000"
}
```
⚠️ Recommendations:
- Installing StartAllBack or using a custom theme like those from Rectify11 can help correct text that doesn't render properly with Translucent Windows in dark mode.
- To prevent strange displays in Office programs, you can add POWERPNT.EXE and other processes to the exclusion list (in the mod's advanced tab).

### 2. Windows 11 File Explorer Styler
```json
{"theme":"","controlStyles[0].target":"Microsoft.UI.Xaml.Controls.AppBarSeparator","controlStyles[0].styles[0]":"Visibility=Collapsed",
"controlStyles[1].target":"Grid#DetailsViewControlRootGrid","controlStyles[1].styles[0]":"Background=Transparent",
"controlStyles[2].target":"StackPanel#DetailsViewThumbnail","controlStyles[2].styles[0]":"Background=Transparent",
"controlStyles[3].target":"Grid#CommandBarControlRootGrid","controlStyles[3].styles[0]":"Background=Transparent","controlStyles[3].styles[1]":"BorderThickness=0,0,0,0",
"controlStyles[4].target":"FileExplorerExtensions.GalleryViewControl#GalleryViewControl > Grid","controlStyles[4].styles[0]":"Background=Transparent",
"controlStyles[5].target":"FileExplorerExtensions.GalleryViewControl#GalleryViewControl > Grid > Grid#GalleryRootGrid","controlStyles[5].styles[0]":"Background=Transparent",
"controlStyles[6].target":"TabViewItem > Grid#LayoutRoot > Canvas > Microsoft.UI.Xaml.Shapes.Path#SelectedBackgroundPath","controlStyles[6].styles[0]":"Fill=Transparent",
"controlStyles[7].target":"Microsoft.UI.Xaml.Controls.Grid#NavigationBarControlGrid","controlStyles[7].styles[0]":"Background=Transparent",
"controlStyles[8].target":"CommandBar#FileExplorerCommandBar","controlStyles[8].styles[0]":"Background=Transparent",
"controlStyles[9].target":"Microsoft.UI.Xaml.Controls.Border#RightBottomBorderLine","controlStyles[9].styles[0]":"Visibility=Collapsed",
"controlStyles[10].target":"Microsoft.UI.Xaml.Controls.Border#LeftBottomBorderLine","controlStyles[10].styles[0]":"Visibility=Collapsed",
"controlStyles[11].target":"Microsoft.UI.Xaml.Controls.Border#BottomBorderLine","controlStyles[11].styles[0]":"Visibility=Collapsed",
"controlStyles[12].target":"TabViewItem > Grid#LayoutRoot > Grid#TabContainer","controlStyles[12].styles[0]":"BorderBrush=Transparent","controlStyles[12].styles[1]":"Background=Transparent"}
```

### 2. Windows 11 Start Menu Styler
⚠️ This json only work with the NEW Windows 11 StartMenu.
```json
{
"controlStyles[0].target":"Border#BorderElement","controlStyles[0].styles[0]":"Background=Transparent",
"controlStyles[1].target":"Border#StartDropShadow\"","controlStyles[1].styles[0]":"Visibility=Collapsed",
"controlStyles[2].target":"Border#AcrylicBorder","controlStyles[2].styles[0]":"Background:=<WindhawkBlur BlurAmount=\"20\" TintColor=\"#50181818\"/>",
"controlStyles[3].target":"Border#AcrylicOverlay","controlStyles[3].styles[0]":"Background:=Transparent","controlStyles[3].styles[1]":"BorderThickness=0,0,0,0",
"controlStyles[4].target":"Grid#UnderlineContainer","controlStyles[4].styles[0]":"Visibility=Collapsed",
"controlStyles[5].target":"Border#dropshadow","controlStyles[5].styles[0]":"Visibility=Collapsed",
"controlStyles[6].target":"Windows.UI.Xaml.Controls.Grid#FrameRoot","controlStyles[6].styles[0]":"RenderTransform:=<TranslateTransform X=\"0\" Y=\"-368\" />","controlStyles[6].styles[1]":"MaxHeight=500",
"controlStyles[7].target":"Windows.UI.Xaml.Controls.SemanticZoom#TopLevelRoot","controlStyles[7].styles[0]":"RenderTransform:=<TranslateTransform X=\"0\" Y=\"368\" />",
"controlStyles[8].target":"Windows.UI.Xaml.Controls.Border#RightCompanionDropShadow","controlStyles[8].styles[0]":"Visibility=Collapsed",
"controlStyles[9].target":"Windows.UI.Xaml.Controls.Border#AppBorder","controlStyles[9].styles[0]":"Background:=<WindhawkBlur BlurAmount=\"20\" TintColor=\"#50181818\"/>",
"controlStyles[10].target":"Windows.UI.Xaml.Controls.Border#TaskbarSearchBackground","controlStyles[10].styles[0]":"Background=Transparent",
"controlStyles[11].target":"Windows.UI.Xaml.Controls.Border#dropshadow","controlStyles[11].styles[0]":"Visibility=Collapsed",
"controlStyles[12].target":"Windows.UI.Xaml.Controls.Border#LayerBorder","controlStyles[12].styles[0]":"Visibility=Collapsed",
"controlStyles[13].target":"StartMenu.FolderModal","controlStyles[13].styles[0]":"RenderTransform:=<TranslateTransform X=\"0\" Y=\"368\" />",
"controlStyles[14].target":"StartMenu.FolderModal > Windows.UI.Xaml.Controls.Grid#Root > Windows.UI.Xaml.Controls.Border","controlStyles[14].styles[0]":"Background:=<WindhawkBlur BlurAmount=\"20\" TintColor=\"#50000000\"/>","controlStyles[14].styles[1]":"Shadow:=","controlStyles[14].styles[2]":"BorderBrush:=<SolidColorBrush Color=\"#FFFFFF\" Opacity=\"0.2\" />","controlStyles[14].styles[3]":"BorderThickness=1,1,1,1",
"controlStyles[15].target":"StartMenu.CategoryControl > Windows.UI.Xaml.Controls.Grid#RootGrid > Windows.UI.Xaml.Controls.Border","controlStyles[15].styles[0]":"Background:=<WindhawkBlur BlurAmount=\"30\" TintColor=\"#00000000\"/>","controlStyles[15].styles[1]":"BorderThickness=1,1,1,1","controlStyles[15].styles[2]":"BorderBrush:=<SolidColorBrush Color=\"#FFFFFF\" Opacity=\"0.1\" />",
"controlStyles[16].target":"Windows.UI.Xaml.Controls.Border#StartDropShadow","controlStyles[16].styles[0]":"Visibility=Collapsed"
}
```

### 3. Windows 11 Taskbar Styler  
```json
{"theme":"","styleConstants[0]":"","resourceVariables[0].variableKey":"","resourceVariables[0].value":"",
"controlStyles[0].target":"Taskbar.TaskListLabeledButtonPanel@RunningIndicatorStates > Rectangle#RunningIndicator","controlStyles[0].styles[0]":"Width@ActiveRunningIndicator=20","controlStyles[0].styles[1]":"Height=2","controlStyles[0].styles[2]":"Width@InactiveRunningIndicator=10","controlStyles[0].styles[3]":"Margin=4,0,0,0",
"controlStyles[1].target":"Taskbar.ExperienceToggleButton#LaunchListButton[AutomationProperties.AutomationId=StartButton] > Taskbar.TaskListButtonPanel@CommonStates > Border#BackgroundElement","controlStyles[1].styles[0]":"Background@InactiveNormal:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Normal.png\" />","controlStyles[1].styles[1]":"Background@InactivePointerOver:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Hover.png\" />","controlStyles[1].styles[2]":"Background@InactivePressed:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Pressed.png\" />","controlStyles[1].styles[3]":"BorderThickness=0","controlStyles[1].styles[4]":"Background@ActiveNormal:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Pressed.png\" />","controlStyles[1].styles[5]":"Background@ActivePointerOver:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Hover.png\" />","controlStyles[1].styles[6]":"Background@ActivePressed:=<ImageBrush Stretch=\"Uniform\" ImageSource=\"C:\\Customization\\Icons\\Start Button\\Pressed.png\" />","controlStyles[1].styles[7]":"CornerRadius=0","controlStyles[1].styles[8]":"MaxHeight=15","controlStyles[1].styles[9]":"MaxWidth=15",
"controlStyles[2].target":"Taskbar.ExperienceToggleButton#LaunchListButton > Taskbar.TaskListButtonPanel > Microsoft.UI.Xaml.Controls.AnimatedVisualPlayer#Icon","controlStyles[2].styles[0]":"Visibility=Collapsed",
"controlStyles[3].target":"Taskbar.TaskbarFrame > Grid#RootGrid > Taskbar.TaskbarBackground > Grid > Rectangle#BackgroundFill","controlStyles[3].styles[0]":"Fill:=<WindhawkBlur BlurAmount=\"20\" TintColor=\"#50181818\"/>",
"controlStyles[4].target":"Taskbar.ExperienceToggleButton#LaunchListButton","controlStyles[4].styles[0]":"Width=42",
"controlStyles[5].target":"Windows.UI.Xaml.Controls.Image#OverlayIcon","controlStyles[5].styles[0]":"Transform3D:=<CompositeTransform3D ScaleX=\"0.6\" ScaleY=\"0.6\" ScaleZ=\"0.6\" />","controlStyles[5].styles[1]":"Margin=10,2,0,0",
"controlStyles[6].target":"Taskbar.Badge#BadgeControl","controlStyles[6].styles[0]":"Transform3D:=<CompositeTransform3D ScaleX=\"0.6\" ScaleY=\"0.6\" ScaleZ=\"0.6\" />","controlStyles[6].styles[1]":"Margin=10,2,0,0",
"controlStyles[7].target":"SystemTray.Stack#NonActivatableStack","controlStyles[7].styles[0]":"Visibility=Collapsed",
"controlStyles[8].target":"Taskbar.TaskListLabeledButtonPanel#IconPanel","controlStyles[8].styles[0]":"Padding=0",
"controlStyles[9].target":"Windows.UI.Xaml.Controls.Image#Icon","controlStyles[9].styles[0]":"Margin=4,0,0,0",
"controlStyles[10].target":"Border#OverflowFlyoutBackgroundBorder","controlStyles[10].styles[0]":"Background:=<WindhawkBlur BlurAmount=\"20\" TintColor=\"#50181818\"/>","controlStyles[10].styles[1]":"Shadow:=","controlStyles[10].styles[2]":"BorderBrush:=<SolidColorBrush Color=\"#FFFFFF\" Opacity=\"0.2\" />",
"controlStyles[11].target":"Windows.UI.Xaml.Controls.Border#BackgroundBorder","controlStyles[11].styles[0]":"Margin=0,0,0,0"}
```
⚠️ Note: The icons used for the [Start Buttons](https://github.com/Acercandr0/Ventanas-Once/blob/main/Start%20Button.7z) are stored in `C:\Customization\Icons\Start Button\` Create the directory and extract the files there. You can also use your own custom .png files.

### 4. Windows 11 Notification Center Styler
```json
{"controlStyles[0].target":"Grid#NotificationCenterGrid","controlStyles[0].styles[0]":"Background:=<WindhawkBlur BlurAmount=\"20\" TintColor=\"#50181818\"/>","controlStyles[0].styles[1]":"BorderThickness=1,1,1,1","controlStyles[0].styles[2]":"Shadow:=","controlStyles[0].styles[3]":"VerticalAlignment=Stretch",
"controlStyles[1].target":"Grid#CalendarCenterGrid","controlStyles[1].styles[0]":"Background:=<WindhawkBlur BlurAmount=\"20\" TintColor=\"#50181818\"/>","controlStyles[1].styles[1]":"BorderThickness=1,1,1,1","controlStyles[1].styles[2]":"Shadow:=",
"controlStyles[2].target":"ScrollViewer#CalendarControlScrollViewer","controlStyles[2].styles[0]":"Background:=<AcrylicBrush Opacity=\"0\"/>",
"controlStyles[3].target":"Border#CalendarHeaderMinimizedOverlay","controlStyles[3].styles[0]":"Background:=<AcrylicBrush Opacity=\"0\"/>",
"controlStyles[4].target":"ActionCenter.FocusSessionControl#FocusSessionControl > Grid#FocusGrid","controlStyles[4].styles[0]":"Background:=<AcrylicBrush Opacity=\"0\"/>",
"controlStyles[5].target":"MenuFlyoutPresenter","controlStyles[5].styles[0]":"Background:=<WindhawkBlur BlurAmount=\"20\" TintColor=\"#50181818\"/>","controlStyles[5].styles[1]":"BorderThickness=1,1,1,1","controlStyles[5].styles[2]":"Padding=2,4,2,4","controlStyles[5].styles[3]":"Shadow:=",
"controlStyles[6].target":"Border#JumpListRestyledAcrylic","controlStyles[6].styles[0]":"Background:=<WindhawkBlur BlurAmount=\"20\" TintColor=\"#50181818\"/>","controlStyles[6].styles[1]":"BorderThickness=1,1,1,1","controlStyles[6].styles[2]":"Shadow:=","controlStyles[6].styles[3]":"BorderBrush:=<SolidColorBrush Color=\"#FFFFFF\" Opacity=\"0.2\" />",
"controlStyles[7].target":"Grid#ControlCenterRegion","controlStyles[7].styles[0]":"Background:=<WindhawkBlur BlurAmount=\"20\" TintColor=\"#50181818\"/>","controlStyles[7].styles[1]":"BorderThickness=1,1,1,1","controlStyles[7].styles[2]":"Margin=0,0,0,460","controlStyles[7].styles[3]":"Shadow:=",
"controlStyles[8].target":"Windows.UI.Xaml.Controls.Grid#L1Grid > Border","controlStyles[8].styles[0]":"Background:=<SolidColorBrush Color=\"Transparent\"/>",
"controlStyles[9].target":"Windows.UI.Xaml.Controls.Grid#MediaTransportControlsRegion","controlStyles[9].styles[0]":"Background:=<WindhawkBlur BlurAmount=\"20\" TintColor=\"#50181818\"/>","controlStyles[9].styles[1]":"BorderThickness=1,1,1,1","controlStyles[9].styles[2]":"Margin=0,0,0,-970","controlStyles[9].styles[3]":"Shadow:=",
"controlStyles[10].target":"Grid#MediaTransportControlsRoot","controlStyles[10].styles[0]":"Background:=<SolidColorBrush Color=\"Transparent\"/>",
"controlStyles[11].target":"ContentPresenter#PageContent","controlStyles[11].styles[0]":"Background:=<SolidColorBrush Color=\"Transparent\"/>",
"controlStyles[12].target":"ContentPresenter#PageContent > Grid > Border","controlStyles[12].styles[0]":"Background:=<SolidColorBrush Color=\"Transparent\"/>",
"controlStyles[13].target":"QuickActions.ControlCenter.AccessibleWindow#PageWindow > ContentPresenter > Grid#FullScreenPageRoot","controlStyles[13].styles[0]":"Background:=<SolidColorBrush Color=\"Transparent\"/>",
"controlStyles[14].target":"QuickActions.ControlCenter.AccessibleWindow#PageWindow > ContentPresenter > Grid#FullScreenPageRoot > ContentPresenter#PageHeader","controlStyles[14].styles[0]":"Background:=<SolidColorBrush Color=\"Transparent\"/>",
"controlStyles[15].target":"Windows.UI.Xaml.Controls.ListView#MediaButtonsListView","controlStyles[15].styles[0]":"RenderTransform:=<ScaleTransform ScaleX=\"0.9\" ScaleY=\"0.9\" />","controlStyles[15].styles[1]":"RenderTransformOrigin=0.5,0.5",
"controlStyles[16].target":"ActionCenter.FocusSessionControl","controlStyles[16].styles[0]":"Height=0",
"theme":"",
"styleConstants[0]":"",
"resourceVariables[0].variableKey":"",
"resourceVariables[0].value":""}
```

### 5. Taskbar Clock Customization  
```json
{"ShowSeconds":0,
"TimeFormat":"h':'mm tt",
"DateFormat":"MMMM d',' yyyy",
"WeekdayFormat":"dddd",
"WeekdayFormatCustom":"",
"TopLine":"%date%    %time%",
"BottomLine":"",
"MiddleLine":"",
"TooltipLine":"",
"Width":180,
"Height":60,
"MaxWidth":0,
"TextSpacing":0,
"WebContentsItems[0].Url":"",
"WebContentsItems[0].BlockStart":"",
"WebContentsItems[0].Start":"",
"WebContentsItems[0].End":"",
"WebContentsItems[0].MaxLength":50,
"WebContentsUpdateInterval":10,
"TimeZones[0]":"Eastern Standard Time",
"TimeStyle.Hidden":0,
"TimeStyle.TextColor":"",
"TimeStyle.TextAlignment":"",
"TimeStyle.FontSize":0,
"TimeStyle.FontFamily":"",
"TimeStyle.FontWeight":"",
"TimeStyle.FontStyle":"",
"TimeStyle.FontStretch":"",
"TimeStyle.CharacterSpacing":0,
"DateStyle.Hidden":1,
"DateStyle.TextColor":"",
"DateStyle.TextAlignment":"",
"DateStyle.FontSize":0,
"DateStyle.FontFamily":"",
"DateStyle.FontWeight":"",
"DateStyle.FontStyle":"",
"DateStyle.FontStretch":"",
"DateStyle.CharacterSpacing":0,
"oldTaskbarOnWin11":0}
```

### 6. Taskbar Tray Icon Spacing
```json
{"notificationIconWidth":30,"overflowIconWidth":32,"overflowIconsPerRow":5}
```

### 7. Disable grouping on the taskbar
No config, use Settings tab.

### 8. Customize Windows notifications placement
No config, use Settings tab.

### 9. Dark mode context menus
No config, use Settings tab.

### 10. Taskbar on top for Windows 11
No config, use Settings tab.


## 🦊 Firefox Theme
[Latin Accent Firefox Theme](https://github.com/Acercandr0/Latin-Accent)

## 🔗 [Wallpaper](https://4kwallpapers.com/black-dark/ios-13-stock-ipados-dark-green-black-background-amoled-ipad-794.html)

### That's it. Enjoy! 🍸
