# RMPG UI LIBRARY.lua
Supports PC and Mobile!

---

## Loadstring
```lua
local Update = loadstring(game:HttpGet("https://raw.githubusercontent.com/Zchedrick/ON-BENDED-KNEE/refs/heads/main/Boyz-ll-Men"))()

```lua
Create Window Here:
```lua
local Library = Update:Window("Legends Of Speed")
```
AddLabel:
```lua
local Time = main:Label("Executer Time")
```

AddTab:
```lua
local main = Library:Tab("Main", "rbxassetid://6026568198")
```
AddButton:
```lua
main:Button("Enable Trading", function()
    print("Trading Enabled")
end)
```
AddToggle:
```lua
main:Toggle("Auto Rebirth", false, "Automatically rebirth", function(state)
    print("Auto Rebirth:", state)
end)
```
AddTextBox:
```lua
main:TextBox("Enter Name", "Type here...", function(text)
    print("You typed:", text)
end)
```
AddSlider:
```lua
main:Slider("WalkSpeed", 16, 500, 16, function(value)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value
end)
```
AddDropdown:
```lua
main:Dropdown("Select Player", {"Player1", "Player2"}, false, function(value)
    print("Selected:", value)
end)
```
Credit to RMPG_Sen
