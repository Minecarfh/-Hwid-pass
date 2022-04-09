-- Gui to Lua
-- Version: 3.2

-- Instances:

local pass = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local Hwid = Instance.new("TextLabel")
local UICorner_2 = Instance.new("UICorner")
local TextButton = Instance.new("TextButton")

--Properties:

pass.Name = "pass"
pass.Parent = game.StarterGui.No pass
pass.BackgroundColor3 = Color3.fromRGB(52, 52, 52)
pass.BackgroundTransparency = 0.350
pass.Position = UDim2.new(0.439798087, 0, 0.107184947, 0)
pass.Size = UDim2.new(0, 107, 0, 85)

UICorner.Parent = pass

Hwid.Name = "Hwid..."
Hwid.Parent = pass
Hwid.BackgroundColor3 = Color3.fromRGB(109, 109, 109)
Hwid.BackgroundTransparency = 0.400
Hwid.Position = UDim2.new(0.0836991668, 0, 0.221176326, 0)
Hwid.Size = UDim2.new(0, 89, 0, 47)
Hwid.Font = Enum.Font.SourceSans
Hwid.Text = "Outpot"
Hwid.TextColor3 = Color3.fromRGB(0, 0, 0)
Hwid.TextSize = 14.000

UICorner_2.Parent = Hwid

TextButton.Parent = Hwid
TextButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextButton.BackgroundTransparency = 1.000
TextButton.Position = UDim2.new(0.0561798215, 0, 0.0851063728, 0)
TextButton.Size = UDim2.new(0, 78, 0, 39)
TextButton.Font = Enum.Font.SourceSans
TextButton.Text = ""
TextButton.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton.TextSize = 14.000

-- Scripts:

local function PVUZMOV_fake_script() -- Hwid.LocalScript 
	local script = Instance.new('LocalScript', Hwid)

	script.Parent.Parent["Hwid..."].Text = "Hwid No pass"
	wait(5)
	script.Parent.Parent.Parent.Parent["No pass"]:GetActor()
end
coroutine.wrap(PVUZMOV_fake_script)()
local function LKOX_fake_script() -- Hwid.Rainbower 
	local script = Instance.new('LocalScript', Hwid)

	while wait() do
		script.Parent.TextColor3 = Color3.new(1,0,0)
		for i=1,15 do
			game:GetService("RunService").RenderStepped:wait()
			script.Parent.TextColor3 = Color3.new(script.Parent.TextColor3.r,script.Parent.TextColor3.g+(17/255),script.Parent.TextColor3.b)
		end
		for i=1,15 do
			game:GetService("RunService").RenderStepped:wait()
			script.Parent.TextColor3 = Color3.new(script.Parent.TextColor3.r-(17/255),script.Parent.TextColor3.g,script.Parent.TextColor3.b)
		end
		for i=1,15 do
			game:GetService("RunService").RenderStepped:wait()
			script.Parent.TextColor3 = Color3.new(script.Parent.TextColor3.r,script.Parent.TextColor3.g,script.Parent.TextColor3.b+(17/255))
		end
		for i=1,15 do
			game:GetService("RunService").RenderStepped:wait()
			script.Parent.TextColor3 = Color3.new(script.Parent.TextColor3.r,script.Parent.TextColor3.g-(17/255),script.Parent.TextColor3.b)
		end
		for i=1,15 do
			game:GetService("RunService").RenderStepped:wait()
			script.Parent.TextColor3 = Color3.new(script.Parent.TextColor3.r+(17/255),script.Parent.TextColor3.g,script.Parent.TextColor3.b)
		end
		for i=1,15 do
			game:GetService("RunService").RenderStepped:wait()
			script.Parent.TextColor3 = Color3.new(script.Parent.TextColor3.r,script.Parent.TextColor3.g,script.Parent.TextColor3.b-(17/255))
		end
	end
end
coroutine.wrap(LKOX_fake_script)()
local function ESLHRT_fake_script() -- TextButton.LocalScript 
	local script = Instance.new('LocalScript', TextButton)

	script.Parent.MouseButton1Click:Connect(function ()
		script.Parent.Parent.Parent.Parent.pass:Destroy()
		
	end)
end
coroutine.wrap(ESLHRT_fake_script)()
local function YSYNJM_fake_script() -- pass.LocalScript 
	local script = Instance.new('LocalScript', pass)

	frame = script.Parent.Parent.pass
	frame.Draggable = true
	frame.Selectable = true
	frame.Active = true
end
coroutine.wrap(YSYNJM_fake_script)()
