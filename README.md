-- Anomic Sikici
-- Version: 1

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local main = Instance.new("Frame")
local welcome = Instance.new("TextLabel")
local tptool = Instance.new("TextButton")
local admin = Instance.new("TextButton")
local esp = Instance.new("TextButton")
local welcome_2 = Instance.new("TextLabel")

--Properties:

ScreenGui.Parent = game.CoreGui

main.Name = "main"
main.Parent = ScreenGui
main.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
main.Position = UDim2.new(0.0572312437, 0, 0.123893805, 0)
main.Size = UDim2.new(0, 467, 0, 411)
main.Active = true
main.Draggable = true


welcome.Name = "welcome"
welcome.Parent = main
welcome.BackgroundColor3 = Color3.fromRGB(255, 0, 4)
welcome.Size = UDim2.new(0, 467, 0, 50)
welcome.Font = Enum.Font.SourceSans
welcome.Text = "Welcome To Anomic Crasher"
welcome.TextColor3 = Color3.fromRGB(0, 0, 0)
welcome.TextScaled = true
welcome.TextSize = 14.000
welcome.TextWrapped = true

tptool.Name = "tptool"
tptool.Parent = main
tptool.BackgroundColor3 = Color3.fromRGB(156, 255, 6)
tptool.Position = UDim2.new(0.0492505357, 0, 0.163017035, 0)
tptool.Size = UDim2.new(0, 130, 0, 86)
tptool.Font = Enum.Font.SourceSans
tptool.Text = "Isınlanma Esyası"
tptool.TextColor3 = Color3.fromRGB(0, 0, 0)
tptool.TextScaled = true
tptool.TextSize = 14.000
tptool.TextWrapped = true
tptool.MouseButton1Down:connect(function()
	mouse = game.Players.LocalPlayer:GetMouse()
	tool = Instance.new("Tool")
	tool.RequiresHandle = false
	tool.Name = "Click Teleport"
	tool.Activated:connect(function()
		local pos = mouse.Hit+Vector3.new(0,2.5,0)
		pos = CFrame.new(pos.X,pos.Y,pos.Z)
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = pos
	end)
	tool.Parent = game.Players.LocalPlayer.Backpack
end)

admin.Name = "admin"
admin.Parent = main
admin.BackgroundColor3 = Color3.fromRGB(156, 255, 6)
admin.Position = UDim2.new(0.379014999, 0, 0.163017035, 0)
admin.Size = UDim2.new(0, 130, 0, 86)
admin.Font = Enum.Font.SourceSans
admin.Text = "Admin Hilesi"
admin.TextColor3 = Color3.fromRGB(0, 0, 0)
admin.TextScaled = true
admin.TextSize = 14.000
admin.TextWrapped = true
admin.MouseButton1Down:connect(function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source", true))()
end)

esp.Name = "esp"
esp.Parent = main
esp.BackgroundColor3 = Color3.fromRGB(156, 255, 6)
esp.Position = UDim2.new(0.702355504, 0, 0.163017035, 0)
esp.Size = UDim2.new(0, 130, 0, 86)
esp.Font = Enum.Font.SourceSans
esp.Text = "ESP Hilesi (Dene Bence)"
esp.TextColor3 = Color3.fromRGB(0, 0, 0)
esp.TextScaled = true
esp.TextSize = 14.000
esp.TextWrapped = true
esp.MouseButton1Down:connect(function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/emirtube11/esp/main/README.md", true))()
end)

welcome_2.Name = "welcome"
welcome_2.Parent = main
welcome_2.BackgroundColor3 = Color3.fromRGB(255, 0, 4)
welcome_2.Position = UDim2.new(0, 0, 0.963503659, 0)
welcome_2.Size = UDim2.new(0, 141, 0, 15)
welcome_2.Font = Enum.Font.SourceSans
welcome_2.Text = "Serveri Fazla Sikme"
welcome_2.TextColor3 = Color3.fromRGB(0, 0, 0)
welcome_2.TextScaled = true
welcome_2.TextSize = 14.000
welcome_2.TextWrapped = true
