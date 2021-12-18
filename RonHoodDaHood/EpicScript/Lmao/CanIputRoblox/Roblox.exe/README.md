

local ScreenGui = Instance.new("ScreenGui")
local main = Instance.new("ImageLabel")
local Label = Instance.new("TextLabel")
local ZellHub = Instance.new("TextButton")
local Spaceware = Instance.new("TextButton")
local Label_2 = Instance.new("TextLabel")
local Label_3 = Instance.new("TextLabel")
local Label_4 = Instance.new("TextLabel")

--Properties:

ScreenGui.Parent = game.CoreGui

main.Name = "main"
main.Parent = ScreenGui
main.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
main.BackgroundTransparency = 1.000
main.Position = UDim2.new(0.426509112, 0, 0.615531206, 0)
main.Size = UDim2.new(0, 547, 0, 218)
main.Image = "rbxassetid://3570695787"
main.ImageColor3 = Color3.fromRGB(47, 47, 47)
main.ScaleType = Enum.ScaleType.Slice
main.SliceCenter = Rect.new(100, 100, 100, 100)
main.SliceScale = 0.120
main.Active = true
main.Draggable = true

Label.Name = "Label"
Label.Parent = main
Label.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
Label.Position = UDim2.new(0.297989011, 0, 0.0458715633, 0)
Label.Size = UDim2.new(0, 200, 0, 20)
Label.Font = Enum.Font.Roboto
Label.Text = "RonHood"
Label.TextColor3 = Color3.fromRGB(255, 255, 255)
Label.TextSize = 14.000

ZellHub.Name = "ZellHub"
ZellHub.Parent = main
ZellHub.BackgroundColor3 = Color3.fromRGB(49, 49, 49)
ZellHub.Position = UDim2.new(0.0621572249, 0, 0.69266057, 0)
ZellHub.Size = UDim2.new(0, 151, 0, 35)
ZellHub.Font = Enum.Font.SourceSans
ZellHub.Text = "ZellHub"
ZellHub.TextColor3 = Color3.fromRGB(255, 255, 255)
ZellHub.TextSize = 14.000
ZellHub.MouseButton1Down:connect(function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/RobloxHackerProLuaStuff/zellhubnew/main/SCRIPTPRO.lua"))()
end)

Spaceware.Name = "Spaceware"
Spaceware.Parent = main
Spaceware.BackgroundColor3 = Color3.fromRGB(49, 49, 49)
Spaceware.Position = UDim2.new(0.338208407, 0, 0.692660689, 0)
Spaceware.Size = UDim2.new(0, 184, 0, 35)
Spaceware.Font = Enum.Font.SourceSans
Spaceware.Text = "Spaceware"
Spaceware.TextColor3 = Color3.fromRGB(255, 255, 255)
Spaceware.TextSize = 14.000
Spaceware.MouseButton1Down:connect(function()
	loadstring(game:HttpGet"https://raw.githubusercontent.com/i-nasa/projects/main/spaceware")()
end)

Label_2.Name = "Label"
Label_2.Parent = main
Label_2.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
Label_2.Position = UDim2.new(0.144424111, 0, 0.600917459, 0)
Label_2.Size = UDim2.new(0, 200, 0, 20)
Label_2.Font = Enum.Font.Roboto
Label_2.Text = "Best Scitps"
Label_2.TextColor3 = Color3.fromRGB(255, 255, 255)
Label_2.TextSize = 14.000

Label_3.Name = "Label"
Label_3.Parent = main
Label_3.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
Label_3.Position = UDim2.new(0.73491776, 0, 0.137614682, 0)
Label_3.Size = UDim2.new(0, 116, 0, 20)
Label_3.Font = Enum.Font.Roboto
Label_3.Text = "Credits"
Label_3.TextColor3 = Color3.fromRGB(255, 255, 255)
Label_3.TextSize = 14.000

Label_4.Name = "Label"
Label_4.Parent = main
Label_4.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
Label_4.Position = UDim2.new(0.338208407, 0, 0.293577969, 0)
Label_4.Size = UDim2.new(0, 368, 0, 38)
Label_4.Font = Enum.Font.Roboto
Label_4.Text = "Gui: LoadedXzio, Scirpter: XzioW, Used:Gui To Lua,Roundifiy"
Label_4.TextColor3 = Color3.fromRGB(255, 255, 255)
Label_4.TextSize = 14.000

-- Scripts:

local function ISFQG_fake_script() -- main.KeyPress 
	local script = Instance.new('LocalScript', main)

	--[[
	print("RonHood Loaded")	
		Press Key to Open a GUI Script V2
		Script By: LoadedXzio
		
		This script works so that when you press a key on your keyboard, it opens a Gui.
		
		Put it accordingly into the StarterGui (More info on line 17
		
	--]]
	wait()
	
	local Players = game:GetService("Players")
	local Player = Players.LocalPlayer
	
	local Mouse = Player:GetMouse()
	local Gui = script.Parent -- Set path to whatever Gui you want to open. For Example: script.Parent.Parent.GuiOrFrameName
	local Open = false
	
	function PressJ(key) -- Chnage Q to whatever key you desire. Capitals matter. For Example: PressH
		if (key == "j") then -- Change "q" to whatever letter you use in the line above. Lowercase matters. For Example: "h"
			if (Open == false) then
				Gui.Visible = true
				Open = true
			elseif (Open == true) then
				Gui.Visible = false
				Open = false
			end
		end
	end
		
	Mouse.KeyDown:Connect(PressJ) -- Make sure (PressQ) matches what you have for line 20. For Example: (PressH)
end
coroutine.wrap(ISFQG_fake_script)()
