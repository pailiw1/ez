local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("PAILIW HUB", "Ocean")
local Tab = Window:NewTab("MAIN")
local Section = Tab:NewSection("AUTO FARM")
Section:NewToggle("AUTO FARM", "ClICK TO USE AUTO FARM", function(state)
_G.Autofarm = state
while _G.Autofarm do wait()
game:GetService("Players").LocalPlayer .ninjaEvent:FireServer("swingKatana")
wait(.1)
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(75.06920623779297, 91261.4296875, 125.79695892333984)
end
end)
Section:NewLabel("AUTO BUY")
Section:NewToggle("AUTO BUY SWORDS", "CLICK TO USE AUTO BUY", function(state)
_G.AutoBuy = state
while _G.AutoBuy do wait()
local args = {
   [1] = "buyAllSwords",
   [2] = "Blazing Vortex Island"
}
game:GetService("Players").LocalPlayer.ninjaEvent:FireServer(unpack(args))
end
end)
Section:NewToggle("AUTO BUY BELTS", "CLICK TO USE AUTO BUY", function(state)
_G.AutoBuy = state
while _G.AutoBuy do wait()
local args = {
   [1] = "buyAllBelts",
   [2] = "Blazing Vortex Island"
}
game:GetService("Players").LocalPlayer.ninjaEvent:FireServer(unpack(args))
end
end)
Section:NewToggle("AUTO BUY SKILL", "CLICK TO USE AUTO BUY", function(state)
_G.AutoBuy = state
while _G.AutoBuy do wait()
local args = {
   [1] = "buyAllSkills",
   [2] = "Blazing Vortex Island"
}

game:GetService("Players").LocalPlayer.ninjaEvent:FireServer(unpack(args))
end
end)
Section:NewToggle("AUTO BUY SHURIKEN", "CLICK TO USE AUTO BUY", function(state)
_G.AutoBuy = state
while _G.AutoBuy do wait()
local args = {
   [1] = "buyAllShurikens",
   [2] = "Blazing Vortex Island"
}
game:GetService("Players").LocalPlayer.ninjaEvent:FireServer(unpack(args))
end
end)   
local Tab = Window:NewTab("TELEPORT")
local Section = Tab:NewSection("Select Player!")
Plr = {}
for i,v in pairs(game:GetService("Players"):GetChildren()) do
    table.insert(Plr,v.Name) 
end
local drop = Section:NewDropdown("Select Player!", "Click To Select", Plr, function(t)
   PlayerTP = t
end)
Section:NewButton("Click To TP", "", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players[PlayerTP].Character.HumanoidRootPart.CFrame
end)
Section:NewToggle("Auto Tp", "", function(t)
_G.TPPlayer = t
while _G.TPPlayer do wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players[PlayerTP].Character.HumanoidRootPart.CFrame
end
end)

Section:NewButton("Refresh Players","Refresh Dropdown", function()
  drop:Refresh(Plr)
end)
local Section = Tab:NewSection("TELEPORT")
Section:NewButton("STARTER ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-18.601409912109375, 63.35551834106445, 34.38841247558594)
end)
Section:NewButton("ENCHANTED ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(84.036865234375, 766.0159301757812, -136.031982421875)
end)
Section:NewButton("ASTRAL ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(223.908203125, 2013.869140625, 258.07452392578125)
end)
Section:NewButton("MYSTICAL ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(167.1921844482422, 4047.216064453125, 30.22384262084961)
end)
Section:NewButton("SPACE ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(113.22293090820312, 5656.71630859375, 156.75949096679688)
end)
Section:NewButton("TUNDRA ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(142.0786590576172, 9283.0302734375, 72.47932434082031)
end)
Section:NewButton("ETERNAL ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(142.34786987304688, 13679.8720703125, 73.0946273803711)
end)
Section:NewButton("SANDSTORM ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(142.1569366455078, 17686.1640625, 72.93534088134766)
end)
Section:NewButton("THUNDERSTORM ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(136.58815002441406, 24069.857421875, 73.77924346923828)
end)
Section:NewButton("ANCIENT INFERNO ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(140.1839141845703, 28254.162109375, 66.6449966430664)
end)
Section:NewButton("MIDNIGHT SHADOW ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(145.2451629638672, 33206.8125, 66.05835723876953)
end)
Section:NewButton("MYTHICAL SOULS ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(135.9132537841797, 39317.40234375, 62.21100997924805)
end)
Section:NewButton("WINTER WONDER ISLAND", "", function()
 game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(139.24807739257812, 46010.38671875, 70.423583984375)
end)
Section:NewButton("GOLDEN MASTER ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(140.44142150878906, 52607.59765625, 69.7709732055664)
end)
Section:NewButton("DRAGON LEGEND ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(140.80552673339844, 59594.51171875, 70.81268310546875)
end)
Section:NewButton("CYBERNETIC LEGEND ISLAND", "", function()
 game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(137.3865203857422, 66669, 71.58378601074219)
end)
Section:NewButton("SKYSTORM ULTRAUS ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(140.0554962158203, 70268.9921875, 66.57727813720703)
end)
Section:NewButton("CHAOS LEGENDS ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(140.10633850097656, 74440.6875, 66.5623779296875)
end)
Section:NewButton("SOUL FUSION ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(139.79010009765625, 79744.1953125, 64.30725860595703)
end)
Section:NewButton("DARK ELEMENTS ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(142.3298797607422, 83196.296875, 70.1264877319336)
end)
Section:NewButton("INNER PEACE ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(140.9358367919922, 87050.90625, 69.18633270263672)
end)
Section:NewButton("BLAZING VORTEX ISLAND", "", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(140.43966674804688, 91245.90625, 67.4275131225586)
end)
local Tab = Window:NewTab("SETTING")
local Section = Tab:NewSection("KEYBINDS")
Section:NewKeybind("Keybind", "KeybindInfo", Enum.KeyCode.RightControl, function()
	Library:ToggleUI()
end)
Section:NewSlider("Speed", "SliderInfo", 500, 0, function(s) -- 500 (MaxValue) | 60 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)
