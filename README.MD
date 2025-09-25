--[[
    RMPG UI LIBRARY
    Supports PC and Mobile!

    How to use:

    1. Load the library:
        local Update = loadstring(game:HttpGet("https://raw.githubusercontent.com/Zchedrick/ON-BENDED-KNEE/main/Boyz-ll-Men"))()

    2. Create a window:
        local Library = Update:Window("Legends Of Speed")

    3. Add a tab to the window:
        local main = Library:Tab("Main", "rbxassetid://6026568198")

    4. Add UI elements to the tab:
        main:Label("Executer Time")

        main:Button("Enable Trading", function()
            print("Trading Enabled")
        end)

        main:Toggle("Auto Rebirth", false, "Automatically rebirth", function(state)
            print("Auto Rebirth:", state)
        end)

        main:TextBox("Enter Name", "Type here...", function(text)
            print("You typed:", text)
        end)

        main:Slider("WalkSpeed", 16, 500, 16, function(value)
            game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value
        end)

        main:Dropdown("Select Player", {"Player1", "Player2"}, false, function(value)
            print("Selected:", value)
        end)

    Credit to RMPG_Sen
]]

-- Example Implementation:
local Update = loadstring(game:HttpGet("https://raw.githubusercontent.com/Zchedrick/ON-BENDED-KNEE/main/Boyz-ll-Men"))()
local Library = Update:Window("Legends Of Speed")
local main = Library:Tab("Main", "rbxassetid://6026568198")

main:Label("Executer Time")

main:Button("Enable Trading", function()
    print("Trading Enabled")
end)

main:Toggle("Auto Rebirth", false, "Automatically rebirth", function(state)
    print("Auto Rebirth:", state)
end)

main:TextBox("Enter Name", "Type here...", function(text)
    print("You typed:", text)
end)

main:Slider("WalkSpeed", 16, 500, 16, function(value)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value
end)

main:Dropdown("Select Player", {"Player1", "Player2"}, false, function(value)
    print("Selected:", value)
end)
