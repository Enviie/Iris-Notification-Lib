# Iris Notification Docs

# Loadstring 

```
local Notification = loadstring(game:HttpGet("https://api.irisapp.ca/Scripts/IrisBetterNotifications.lua"))()
```
# Notification.Notify

```
bool Notification.Notify(<string> Title, <string> Description, <string> ImageAsset, <Table> Settings = Default)
```
# Notification.WallNotification

```
bool Notification.WallNotification(<string> Title, <string> Description, <Table> Settings = Default)
```
# Notification Settings Table

```
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

```
local Notification = loadstring(game:HttpGet("https://api.irisapp.ca/Scripts/IrisBetterNotifications.lua"))()

Notification.Notify("Yeeet", "yeet", "rbxasset://textures/ui/GuiImagePlaceholder.png", {
    Duration = 2,       
    Main = {
        Rounding = true,
    }
});

Notification.WallNotification("Test", "The Fitness Gram Pacer Test", {
        Duration = 3,

        TitleSettings = {
            Enabled = false
        }
    });
```
- ImageID must be in rbxasset format, Settings is optional!
