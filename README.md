local Library = loadstring(game:HttpGet("https://pastebin.com/raw/vff1bQ9F"))()
local Window = Library.CreateLib("SuperNatural Simulatir | Made By Laurence#0962", "BloodTheme")

local PrisonBreakerV16 = Instance.new("ScreenGui")
local openmain = Instance.new("Frame")
local open = Instance.new("TextButton")
local main = Instance.new("Frame")
local title = Instance.new("TextLabel")
local home = Instance.new("TextButton")
local guis = Instance.new("TextButton")
local teams = Instance.new("TextButton")
local funcs = Instance.new("TextButton")
local homemain = Instance.new("Frame")
local title_2 = Instance.new("TextLabel")
local TextLabel = Instance.new("TextLabel")
local teamsmain = Instance.new("Frame")
local cop = Instance.new("TextButton")
local inmate = Instance.new("TextButton")
local neutral = Instance.new("TextButton")
local crim = Instance.new("TextButton")
local guismain = Instance.new("Frame")
local prisonbreakerv15 = Instance.new("TextButton")
local prisondestroyer = Instance.new("TextButton")
local kickgui = Instance.new("TextButton")
local scriptsmain = Instance.new("Frame")
local godmode = Instance.new("TextButton")
local destroy = Instance.new("TextButton")
local hitbox = Instance.new("TextButton")
local antikickmainon = Instance.new("Frame")
local antikickon = Instance.new("TextButton")
local antikickmainoff = Instance.new("Frame")
local antikickoff = Instance.new("TextButton")
local modguns = Instance.new("TextButton")
PrisonBreakerV16.Name = "PrisonBreakerV1.6"
PrisonBreakerV16.Parent = game.CoreGui

openmain.Name = "openmain"
openmain.Parent = PrisonBreakerV16
openmain.BackgroundColor3 = Color3.new(1, 1, 1)
openmain.Position = UDim2.new(0.0104873544, 0, 0.549140036, 0)
openmain.Size = UDim2.new(0, 100, 0, 26)

open.Name = "open"
open.Parent = openmain
open.BackgroundColor3 = Color3.new(1, 0, 0.498039)
open.Position = UDim2.new(0, 0, -0.0299201012, 0)
open.Size = UDim2.new(0, 100, 0, 26)
open.Font = Enum.Font.GothamBlack
open.Text = "Open/Close"
open.TextColor3 = Color3.new(0, 0, 0)
open.TextSize = 18
open.TextWrapped = true
open.MouseButton1Down:connect(function()
    Library:ToggleUI()
end)

local Tab1 = Window:NewTab("Credits")
local Tab1Section = Tab1:NewSection("Thank For Using FireNatural Simulator")

Tab1Section:NewButton("alt1lr#3351", "No Description", function()
setclipboard('alt1lr#3351')
end)

Tab1Section:NewButton("Discord", "No Description", function()
setclipboard('https://discord.gg/zs4FP4VYYx')
end)

Tab1Section:NewButton("Youtube", "No Description", function()
setclipboard('https://m.youtube.com/channel/UCxfiH1VLU1H6td_ny_Bt0oQ')
end)

local Tab2 = Window:NewTab("SuperNatural")
local Tab2Section = Tab2:NewSection("Script")

Tab2Section:NewToggle("Auto Sell", "No Description", function(state)
    if state then
        _G.sell = true
while _G.sell do
    wait(0.1) -- change what you need delay
local args = {
    [1] = {
        [1] = "SellMuscle"
    }
}

game:GetService("ReplicatedStorage").RemoteEvent:FireServer(unpack(args))
end
    else
        _G.sell = false
while _G.sell do
    wait(0.1) -- change what you need delay
local args = {
    [1] = {
       [1] = "SellMuscle"
    }
}

game:GetService("ReplicatedStorage").RemoteEvent:FireServer(unpack(args))
end
    end
end)

Tab2Section:NewToggle("Auto Gain", "No Description", function(state)
    if state then
        _G.gain = true
while _G.gain do
    wait(0.00000000000000000000000000000000000000000000000000001) -- its good delay didnt change
local args = {
    [1] = {
       [1] = "GainMuscle"
    }
}

game:GetService("ReplicatedStorage").RemoteEvent:FireServer(unpack(args))
end




    else
        _G.gain = False
while _G.gain do
    wait(0.5) -- its good delay didnt change
local args = {
    [1] = {
       [1] = "GainMuscle"
    }
}

game:GetService("ReplicatedStorage").RemoteEvent:FireServer(unpack(args))
end  
    end
end)

local Tab2Section = Tab2:NewSection("Custom")

Tab2Section:NewTextBox("Auto Sell", "No Discription", function(txt)
_G.sell = true
while _G.sell do
    wait(txt) -- change what you need delay
local args = {
    [1] = {
        [1] = "SellMuscle"
    }
}

game:GetService("ReplicatedStorage").RemoteEvent:FireServer(unpack(args))
end
end)

Tab2Section:NewTextBox("Auto Gain", "No Discription", function(txt)
_G.gain = true
while _G.gain do
    wait(txt) -- its good delay didnt change
local args = {
    [1] = {
       [1] = "GainMuscle"
    }
}

game:GetService("ReplicatedStorage").RemoteEvent:FireServer(unpack(args))
end
end)
