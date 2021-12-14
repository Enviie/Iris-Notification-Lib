# Iris Notification Docs

# Loadstring 

```lua
local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/Enviie/Iris-Notification-Lib/main/Iris%20Notification%20Main.lua"))()
```
# Notification.Notify

```lua
bool Notification.Notify(<string> Title, <string> Description, <string> ImageAsset, <Table> Settings = Default)
```
# Notification.WallNotification

```lua
bool Notification.WallNotification(<string> Title, <string> Description, <Table> Settings = Default)
```
# Notification.ClearAllNotifications()

```lua
void Notification.ClearAllNotifications()
```

# Notification Settings Table

```lua
Duration = 2,

TitleSettings = {
    BackgroundColor3 = Color3.fromRGB(200, 200 ,200),
    TextColor3 = Color3.fromRGB(240, 240, 240),
    TextScaled = true,
    TextWrapped = true,
    TextSize = 14,
    Font = Enum.Font.SourceSansBold,
    TextXAlignment = Enum.TextXAlignment.Left,
    TextYAlignment = Enum.TextYAlignment.Center
},

DescriptionSettings = {
    BackgroundColor3 = Color3.fromRGB(200, 200 ,200),
    TextColor3 = Color3.fromRGB(240, 240, 240),
    TextScaled = true,
    TextWrapped = true,
    TextSize = 14,
    Font = Enum.Font.SourceSansBold,
    TextXAlignment = Enum.TextXAlignment.Left,
    TextYAlignment = Enum.TextYAlignment.Top,
},

IconSettings = {
    BackgroundTransparency = 1,
    BackgroundColor3 = Color3.fromRGB(255, 255, 255),               
},

GradientSettings = {
    GradientEnabled = false,
    SolidColorEnabled = true,
    SolidColor = Color3.fromRGB(0,255,0255),
    Retract = false,
    Extend = false,
},

Main = {
    BorderColor3 = Color3.fromRGB(255, 255, 255),
    BackgroundColor3 = Color3.fromRGB(30, 30, 30),
    BackgroundTransparency = 0.05,
    Rounding = true,
    BorderSizePixel = 1
}
```

# Notification Wall Settings Table

```lua
local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/Enviie/Iris-Notification-Lib/main/Iris%20Notification%20Main.lua"))()

Notification.Notify("{ Iris }", "Yeet", "rbxassetid://7258714296", {
    Duration = 7,
    
    TitleSettings = {
        TextXAlignment = Enum.TextXAlignment.Center,
        Font = Enum.Font.SourceSansSemibold,
    },

    GradientSettings = {
        GradientEnabled = false,
        SolidColorEnabled = true,
        SolidColor = Color3.fromRGB(124, 83, 240),
        Retract = true
    }
})
Notification.WallNotification("God", "Yeet", {
    MainSettings = {
        Orientation = "Left",
        VisibleSize = UDim2.new(0.5, 0, 0.5, 0);
        HiddenSize  = UDim2.new(0, 0, 0.5, 0),
        TweenTime   = 0.8
    },
})    
```
- ImageID must be in rbxasset format, Settings is optional!
# Credit by Iris the creator for the Docs
