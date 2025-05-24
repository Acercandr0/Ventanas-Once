## 📷 Preview

![Preview 1](https://github.com/Acercandr0/My-Windhawk-Configuration/blob/main/Preview1.png)  
![Preview 2](https://github.com/Acercandr0/My-Windhawk-Configuration/blob/main/Preview2.png)  
![Preview 3](https://github.com/Acercandr0/My-Windhawk-Configuration/blob/main/Preview3.png)  

# Mods and configuration:

### Customize Windows notifications placement  
```json
{"monitor":1,"monitorInterfaceName":"","horizontalPlacement":"right","horizontalDistanceFromScreenEdge":0,"verticalPlacement":"top","verticalDistanceFromScreenEdge":-20}
```

### Taskbar Clock Customization  
```json
{"ShowSeconds":0,"TimeFormat":"h':'mm tt","DateFormat":"d 'de' MMMM","WeekdayFormat":"dddd","WeekdayFormatCustom":"","TopLine":"%date%  %time%","BottomLine":"","MiddleLine":"","TooltipLine":"","Width":180,"Height":60,"MaxWidth":0,"TextSpacing":-1,"oldTaskbarOnWin11":0}
```
**Note:** Change date format to english or leave it in spanish, it's your call.

### Taskbar Height and Icon Size  
```json
{"IconSize":16,"TaskbarHeight":30,"TaskbarButtonWidth":27}
```

### Taskbar on Top for Windows 11  
```json
{"taskbarLocation":"top","taskbarLocationSecondary":"sameAsPrimary","runningIndicatorsOnTop":0}
```

### Windows 11 Notification Center Styler  
```json
{"theme":"","controlStyles[0].target":"Grid#ControlCenterRegion","controlStyles[0].styles[0]":"Margin=0,0,0,460","controlStyles[1].target":"Grid#NotificationCenterGrid","controlStyles[1].styles[0]":"VerticalAlignment=Stretch","controlStyles[2].target":"Grid#CalendarCenterGrid","controlStyles[2].styles[0]":"Margin=0,12,0,15","controlStyles[3].target":"Windows.UI.Xaml.Controls.Grid#MediaTransportControlsRegion","controlStyles[3].styles[0]":"Margin=0,12,0,-960","controlStyles[0].styles[1]":"Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.4\" />"}
```

### Windows 11 Start Menu Styler  
```json
{"theme":"","controlStyles[0].target":"Border#AcrylicBorder","controlStyles[0].styles[0]":"Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.4\" />","controlStyles[1].target":"Windows.UI.Xaml.Controls.Grid#RootPanel","controlStyles[1].styles[0]":"MaxHeight=490","controlStyles[2].target":"Windows.UI.Xaml.Controls.Grid#TopLevelSuggestionsListHeader","controlStyles[3].target":"Windows.UI.Xaml.Controls.Grid#NoTopLevelSuggestionsText","controlStyles[3].styles[0]":"Visibility=Collapsed","controlStyles[4].target":"Windows.UI.Xaml.Controls.Grid#TopLevelSuggestionsContainer","controlStyles[5].target":"Windows.UI.Xaml.Controls.Grid#ShowMoreSuggestions","controlStyles[5].styles[0]":"Visibility=Collapsed","controlStyles[4].styles[0]":"Visibility=Collapsed","controlStyles[2].styles[0]":"Visibility=Collapsed","controlStyles[6].target":"Windows.UI.Xaml.Controls.Grid#UndockedRoot","controlStyles[6].styles[0]":"Margin=0,0,0,0","controlStyles[7].target":"Windows.UI.Xaml.Controls.TextBlock#PinnedListHeaderText","controlStyles[7].styles[0]":"Visibility=Collapsed","webContentCustomJs":"","resourceVariables[0].variableKey":"","resourceVariables[0].value":"","controlStyles[1].styles[1]":"Margin=0,-235,0,0","controlStyles[8].target":"StartDocked.PowerOptionsView","controlStyles[8].styles[0]":"Margin=0,220,0,0","controlStyles[9].target":"StartDocked.UserTileView#UserTile","controlStyles[9].styles[0]":"Visibility=Collapsed","controlStyles[10].target":"StartDocked.AppListView#NavigationPanePlacesListView","controlStyles[10].styles[0]":"Margin=0,220,0,0","controlStyles[11].target":"Windows.UI.Xaml.Controls.Border#BorderUnderline","controlStyles[11].styles[0]":"Visibility=Collapsed","controlStyles[0].styles[1]":"BorderThickness=0,0,0,0","controlStyles[12].target":"Windows.UI.Xaml.Controls.Grid#MainContent","controlStyles[12].styles[0]":"Margin=0,0,0,0","controlStyles[13].target":"Windows.UI.Xaml.Controls.Border#AcrylicOverlay","controlStyles[13].styles[0]":"Visibility=Collapsed","controlStyles[14].target":"Windows.UI.Xaml.Controls.Border#BorderElement","controlStyles[14].styles[0]":"Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0\" />"}
```

### Windows 11 Taskbar Styler  
```json
{"theme":"","styleConstants[0]":"","resourceVariables[0].variableKey":"","resourceVariables[0].value":"","controlStyles[0].target":"Taskbar.Beacon#BeaconControl","controlStyles[0].styles[0]":"Transform3D:=<CompositeTransform3D ScaleX=\"1.2\" ScaleY=\"1.2\" ScaleZ=\"1.2\" />","controlStyles[0].styles[1]":"Margin=0,-10,-6,0","controlStyles[1].target":"Taskbar.TaskListLabeledButtonPanel#IconPanel","controlStyles[1].styles[0]":"Padding=0,0,0,0","controlStyles[2].target":"Windows.UI.Xaml.Controls.Image#Icon","controlStyles[2].styles[0]":"Margin=5,0,0,0","controlStyles[3].target":"Windows.UI.Xaml.Shapes.Rectangle#RunningIndicator","controlStyles[3].styles[0]":"Margin=5,0,0,0","controlStyles[3].styles[1]":"Width=10","controlStyles[3].styles[2]":"Height=2"}
```
**Note:** Icons used for the Start Button are located in my C: drive (`C:\Customization\Icons\Start Button\`)
You can download them from the main branch or use your own custom path and buttons.
There should be three versions: **Normal**, **Hover**, and **Pressed**.
