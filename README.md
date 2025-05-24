# My Windhawk Configuration

## 🛠️ Mods Included  

### Customize Windows notifications placement  
Modify where notifications appear on your screen for a cleaner experience.  
```json
{"monitor":1,"monitorInterfaceName":"","horizontalPlacement":"right","horizontalDistanceFromScreenEdge":0,"verticalPlacement":"top","verticalDistanceFromScreenEdge":-20}
```

### Taskbar Clock Customization  
Customize the appearance of the taskbar clock, including date and time format.  
```json
{"ShowSeconds":0,"TimeFormat":"h':'mm tt","DateFormat":"d 'de' MMMM","WeekdayFormat":"dddd","WeekdayFormatCustom":"","TopLine":"%date%  %time%","BottomLine":"","MiddleLine":"","TooltipLine":"","Width":180,"Height":60,"MaxWidth":0,"TextSpacing":-1,"oldTaskbarOnWin11":0}
```

### Taskbar Height and Icon Size  
Adjust taskbar height and icon size for a refined look.  
```json
{"IconSize":16,"TaskbarHeight":30,"TaskbarButtonWidth":27}
```

### Taskbar on Top for Windows 11  
Move the taskbar to the top for a unique workspace setup.  
```json
{"taskbarLocation":"top","taskbarLocationSecondary":"sameAsPrimary","runningIndicatorsOnTop":0}
```

### Windows 11 Notification Center Styler  
Refine the look of the Notification Center with margin adjustments and acrylic styling.  
```json
{"theme":"","controlStyles[0].target":"Grid#ControlCenterRegion","controlStyles[0].styles[0]":"Margin=0,0,0,460","controlStyles[1].target":"Grid#NotificationCenterGrid","controlStyles[1].styles[0]":"VerticalAlignment=Stretch","controlStyles[2].target":"Grid#CalendarCenterGrid","controlStyles[2].styles[0]":"Margin=0,12,0,15","controlStyles[3].target":"Windows.UI.Xaml.Controls.Grid#MediaTransportControlsRegion","controlStyles[3].styles[0]":"Margin=0,12,0,-960","controlStyles[0].styles[1]":"Background:=<AcrylicBrush TintColor=\"Black\" TintOpacity=\"0.4\" />"}
```
