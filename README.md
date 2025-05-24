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
{
  "theme": "",
  "controlStyles": [
    {
      "target": "Border#AcrylicBorder",
      "styles": [
        "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.4\" />"
      ]
    },
    {
      "target": "Windows.UI.Xaml.Controls.Grid#RootPanel",
      "styles": [
        "MaxHeight=490",
        "Margin=0,-235,0,0"
      ]
    },
    {
      "target": "Windows.UI.Xaml.Controls.Grid#TopLevelSuggestionsListHeader",
      "styles": ["Visibility=Collapsed"]
    },
    {
      "target": "Windows.UI.Xaml.Controls.Grid#NoTopLevelSuggestionsText",
      "styles": ["Visibility=Collapsed"]
    },
    {
      "target": "Windows.UI.Xaml.Controls.Grid#TopLevelSuggestionsContainer",
      "styles": ["Visibility=Collapsed"]
    },
    {
      "target": "Windows.UI.Xaml.Controls.Grid#ShowMoreSuggestions",
      "styles": ["Visibility=Collapsed"]
    },
    {
      "target": "Windows.UI.Xaml.Controls.Grid#UndockedRoot",
      "styles": ["Margin=0,0,0,0"]
    },
    {
      "target": "Windows.UI.Xaml.Controls.TextBlock#PinnedListHeaderText",
      "styles": ["Visibility=Collapsed"]
    },
    {
      "target": "StartDocked.PowerOptionsView",
      "styles": ["Margin=0,220,0,0"]
    },
    {
      "target": "StartDocked.UserTileView#UserTile",
      "styles": ["Visibility=Collapsed"]
    },
    {
      "target": "StartDocked.AppListView#NavigationPanePlacesListView",
      "styles": ["Margin=0,220,0,0"]
    },
    {
      "target": "Windows.UI.Xaml.Controls.Border#BorderUnderline",
      "styles": ["Visibility=Collapsed"]
    },
    {
      "target": "Windows.UI.Xaml.Controls.Grid#MainContent",
      "styles": ["Margin=0,0,0,0"]
    },
    {
      "target": "Windows.UI.Xaml.Controls.Border#AcrylicOverlay",
      "styles": ["Visibility=Collapsed"]
    },
    {
      "target": "Windows.UI.Xaml.Controls.Border#BorderElement",
      "styles": [
        "Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0\" />"
      ]
    }
  ]
}
```

### Windows 11 Taskbar Styler  
```json
{"theme":"","styleConstants[0]":"","resourceVariables[0].variableKey":"","resourceVariables[0].value":"","controlStyles[0].target":"Taskbar.Beacon#BeaconControl","controlStyles[0].styles[0]":"Transform3D:=<CompositeTransform3D ScaleX=\"1.2\" ScaleY=\"1.2\" ScaleZ=\"1.2\" />","controlStyles[0].styles[1]":"Margin=0,-10,-6,0","controlStyles[1].target":"Taskbar.TaskListLabeledButtonPanel#IconPanel","controlStyles[1].styles[0]":"Padding=0,0,0,0","controlStyles[2].target":"Windows.UI.Xaml.Controls.Image#Icon","controlStyles[2].styles[0]":"Margin=5,0,0,0","controlStyles[3].target":"Windows.UI.Xaml.Shapes.Rectangle#RunningIndicator","controlStyles[3].styles[0]":"Margin=5,0,0,0","controlStyles[3].styles[1]":"Width=10","controlStyles[3].styles[2]":"Height=2"}
```
**Note:** Icons used for the Start Button are located in my C: drive (`C:\Customization\Icons\Start Button\`)
You can download them from the main branch or use your own custom path and buttons.
There should be three versions: **Normal**, **Hover**, and **Pressed**.
