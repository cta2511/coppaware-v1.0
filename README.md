-- antiban script:
setfflag("DFStringCrashPadUploadToBacktraceToBacktraceBaseUrl", "")
setfflag("DFIntCrashUploadToBacktracePercentage", "0")
-- the rest of the hub:

local Mercury = loadstring(game:HttpGet("https://raw.githubusercontent.com/deeeity/mercury-lib/master/src.lua"))()

-- GUI:

local GUI = Mercury:Create{
    Name = "Mercury",
    Size = UDim2.fromOffset(600, 400),
    Theme = Mercury.Themes.Dark,
    Link = "https://coppaware.xyz"
}

GUI:Notification{
	Title = "Join Coppaware!",
	Text = "join here: discord.gg/yu95P48XaV",
	Duration = 20,
	Callback = function() end
}

-- tabs:

local Tab = GUI:Tab{
	Name = "general-purpose",
	Icon = "rbxassetid://8569322835"
}

-- buttons:

Tab:Button{
	Name = "Backdoor Scanner (MAY BAN YOU)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/3BKW2FbU'))() end
}

Tab:Button{
	Name = "Netless Bypass (USEFUL FOR OLD SCRIPTS)",
	Description = nil,
	Callback = function() for i,v in next, game:GetService("Players").LocalPlayer.Character:GetDescendants() do
    if v:IsA("BasePart") and v.Name ~="HumanoidRootPart" then 
    game:GetService("RunService").Heartbeat:connect(function()
    v.Velocity = Vector3.new(-30,0,0)
    end)
    end
    end
 
    game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Notification";
        Text = "Netless Ran";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16; end
}

Tab:Button{
	Name = "Selexity Animation Hub",
	Description = nil,
	Callback = function() loadstring(game:HttpGet(('https://raw.githubusercontent.com/o5u3/Selexity/main/Main'),true))() end
}

Tab:Button{
	Name = "Dex v4 Rework",
	Description = nil,
	Callback = function() loadstring(game:HttpGetAsync("https://gist.githubusercontent.com/DinosaurXxX/b757fe011e7e600c0873f967fe427dc2/raw/ee5324771f017073fc30e640323ac2a9b3bfc550/dark%2520dex%2520v4"))() end
}

Tab:Button{
	Name = "FE Server Finder",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://www.scriptblox.com/raw/Server-Browser_80", true))() end
}

Tab:Button{
	Name = "Unnamed ESP",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/kvr0AuWz'))() end
}

Tab:Button{
	Name = "Anti-Fling (can't undo)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/nsQM0Gdn'))() end
}

Tab:Button{
	Name = "Remote Spy",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/exxtremestuffs/SimpleSpySource/master/SimpleSpy.lua", true))() end
}

-- note to self, don't forget the { and } and the "," near the "name =" thing

-- administrative scripts tab

local Tab = GUI:Tab{
	Name = "administrative-scripts",
	Icon = "rbxassetid://8569322835"
}

Tab:Button{
	Name = "Infinite Yield",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))() end
}

Tab:Button{
	Name = "Fates Admin",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/fatesc/fates-admin/main/main.lua"))() end
}

Tab:Button{
	Name = "Homebrew Admin",
	Description = nil,
	Callback = function() loadstring(game:HttpGet(('https://raw.githubusercontent.com/mgamingpro/HomebrewAdmin/master/Main'),true))() end
}

Tab:Button{
	Name = "CMD-X (IY but skidded)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/CMD-X/CMD-X/master/Source", true))() end
}

Tab:Button{
	Name = "Shattervest Admin (very old)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/VT3pDKec", true))() end
}

Tab:Button{
	Name = "Reviz Admin v2",
	Description = nil,
	Callback = function() loadstring(game:HttpGet(('https://pastebin.com/raw/Caniwq2N'),true))() end
}

local Tab = GUI:Tab{
	Name = "chat-mods",
	Icon = "rbxassetid://8569322835"
}

Tab:Button{
	Name = "Chat Bypasser (BANNABLE)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://the-shed.xyz/roblox/scripts/ChatBypass", true))() end
}

Tab:Button{
	Name = "ChatHax v2",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/ant-7802/--/main/straightmilk.lua'))() end
}

Tab:Button{
	Name = "Chat AutoTranslator (translates you and other people)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/CMD-X/CMD-X/master/Source", true))() end
}

local Tab = GUI:Tab{
	Name = "fun-stuff",
	Icon = "rbxassetid://8569322835"
}

Tab:Button{
	Name = "Bring All (more info at pastebin.com/YRcRY2eE)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/DigitalityScripts/roblox-scripts/main/Bring%20All'))() end
}

Tab:Button{
	Name = "Kill All (more info at pastebin.com/YRcRY2eE)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/DigitalityScripts/roblox-scripts/main/Kill%20All'))() end
}

Tab:Button{
	Name = "E to Fling (R6 only)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/q3y5ZeY9"))() end
}

Tab:Button{
	Name = "FE Part Flinger (works on NDS)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/aFMXLZ3j", true))() end
}

Tab:Button{
	Name = "FE Part Grabber",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/KcmdCdMK'))() end
}

Tab:Button{
	Name = "FE Stream Sniper",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/Blissful4992/Miscellaneous/main/StreamSniper.lua"))() end
}

local Tab = GUI:Tab{
	Name = "hubs",
	Icon = "rbxassetid://8569322835"
}

Tab:Button{
	Name = "OwlHub",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/CriShoux/OwlHub/master/OwlHub.txt"))(); end
}

Tab:Button{
	Name = "DarkHub (arsenal)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://darkhub.xyz/remote-script.lua"))() end
}

Tab:Button{
	Name = "Corrupts Hub (PAID, corruptshub.com)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://corruptshub.com/hub/V4/V4Loader"))() end
}

Tab:Button{
	Name = "Domain X (free version)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://shlex.dev/release/domainx/latest.lua',true))() end
}

Tab:Button{
	Name = "Lunar UI",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/VapingCat/Lunar-UI/main/script.lua", true))() end
}

Tab:Button{
	Name = "MrDestroyer Hub v2",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/MrDestroyerSkid/Project-Destroyer/main/Destroyer"))() end
}

Tab:Button{
	Name = "CC Aimbot",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/dfHDEVP5"))() end
}

Tab:Button{
	Name = "Spec's Hub",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/specowos/specs-scripts/main/ui/main.lua"))() end
}

Tab:Button{
	Name = "Nullware v3",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://gist.githubusercontent.com/M6HqVBcddw2qaN4s/2d722888a388017c18028cd434c43a25/raw/dcccf1027fe4b90780e47767aaf584389c9d7771/EULma3fU90PUOKUn?identifier"))() end
}

Tab:Button{
	Name = "Hubba Hubba",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://files.shade4real.net/flinger.txt'))() end
}

Tab:Button{
	Name = "iExploit Leaked",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://iexploit.xyz/scripts/plasma/storage/Loader'))() end
}

Tab:Button{
	Name = "C00lgui v2",
	Description = nil,
	Callback = function() loadstring(game:GetObjects("rbxassetid://9827584846")[1].Source)() end
}

local Tab = GUI:Tab{
	Name = "game-specific-scripts",
	Icon = "rbxassetid://8569322835"
}

Tab:Button{
	Name = "Fencing Spray Dupe",
	Description = nil,
	Callback = function() game:GetService('RunService').Stepped:connect(function()
for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
if v.Name == "Spray" then
if v.Handle.Mesh then
v.Handle.Mesh:Destroy()
end
v.Parent = workspace
end
end
end)
local function paint()
for i,v in pairs(game.Workspace:GetChildren())do
if v.Name == "Handle" then
v.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
v.Transparency = 1
v.CanCollide = false
wait()
v.CFrame = game.Players.LocalPlayer.Character["Left Leg"].CFrame
end
end
end
local function equip()
for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren())do
if v.Name == "Spray" then
game.Players.LocalPlayer.Character.Humanoid:EquipTool(v)
end
end
end
while wait(0.05) do
paint()
equip()
end end -- there are 2 ends because of how the script works
}

Tab:Button{
	Name = "Fencing Spray Thing (run the script above first)",
	Description = nil,
	Callback = function() local screenGui = game:GetObjects("rbxassetid://3546404827")[1]
  local mainFrame = screenGui.Frame
    local pages = mainFrame.Pages
      local pageLayout = pages.UIPageLayout
      local pageScripts = pages.Scripts
        local interactiveButton = pageScripts.Character.Elements.TextButton
        local utility = pageScripts.Utility
          local utilityElements = utility.Elements
      local pageOptions = pages.Options
    local titleFrame = mainFrame.Title
    local toolbar = mainFrame.Toolbar

screenGui.LocalScript:Destroy()
screenGui.Parent = game:GetService("CoreGui")
interactiveButton.Parent = nil
mainFrame.Visible = true

gripCenter = CFrame.new(0, 0, 1) * CFrame.Angles(math.rad(90), 0, 0)
offset = CFrame.Angles(0, 0, 0)

_player = {
	p = game:GetService("Players").LocalPlayer;
	b = function()
		return _player.p:FindFirstChild("Backpack")
	end;
	c = function()
		return _player.p.Character
	end;
}
_functions = {
	respawn = function()
		local c = _player.c()
		if workspace:FindFirstChild(_player.p.Name) then 
			spawn(function()
				wait(.5)
				if _player.c() ~= workspace:FindFirstChild(_player.p.Name) then
					workspace:FindFirstChild(_player.p.Name):BreakJoints()
				end
			end)
		end
		if c then
			c:BreakJoints()
			c:ClearAllChildren()
		end
		local newChar = Instance.new("Model", workspace)
		local hum = Instance.new("Humanoid", newChar)
		local torso = Instance.new("Part", newChar)
		newChar.Name = "respawn_"
		torso.Name = "Torso"
		torso.Transparency = 1
		_player.p.Character = newChar
		torso.Name = ""
		torso.CanCollide = false
		newChar:MoveTo(Vector3.new(999999, 999999, 999999))
	end;
	tools = function(int)
		local amount = int or 200

local LocalPlayer = game:GetService("Players").LocalPlayer
local spray = workspace.Handle
local savecframe = spray.CFrame
LocalPlayer.Character.Humanoid:UnequipTools()
local currentamount = #LocalPlayer.Backpack:GetChildren()
spray.CanCollide = false
spray.Transparency = 1
local anim = Instance.new("Animation")
anim.AnimationId = "rbxassetid://188632011"
local loadanim = LocalPlayer.Character.Humanoid:LoadAnimation(anim)
loadanim.Looped = true
loadanim:Play()
for _, tool in pairs(LocalPlayer.Backpack:GetChildren()) do
tool.Parent = LocalPlayer
end
repeat
repeat
spray.CFrame = LocalPlayer.Character.HumanoidRootPart.CFrame
wait()
until LocalPlayer.Character:FindFirstChild("Spray") ~= nil
LocalPlayer.Character:FindFirstChild("Spray").Parent = LocalPlayer
until #LocalPlayer:GetChildren() - 4 - currentamount >= amount + 1
loadanim:Stop()
anim:Destroy()
for _, tool in pairs(LocalPlayer:GetChildren()) do
if tool:IsA("Tool") then
tool.Parent = LocalPlayer.Backpack
end
end
spray.CFrame = savecframe
spray.CanCollide = true
spray.Transparency = 0


		
	end;
	load = function()
		local b = _player.b()
		local c = _player.c()
		local grip = function(tool, cf)
			local origin = CFrame.new(cf.p)
			local x, y, z = cf:toEulerAnglesXYZ()
			local new = CFrame.Angles(x, y, z)
			local grip = (origin * new):inverse()
			tool.Grip = grip
		end
		local model = c:WaitForChild("gay") -- stupid name choice from what a few months ago?? i have nothing against it i swear
		local parts = {}
		wait(1)
		
		for i, Model in pairs(c:GetChildren()) do
			if Model:IsA("Model") and Model.Name == "gay" then
				for i, v in pairs(Model:GetDescendants()) do
					if v:IsA("BasePart") then
						v.LocalTransparencyModifier = 1
						if v.Name ~= "Ignore" then
							table.insert(parts, v)
						end
					end
					if not v:IsA("BasePart") and not v:IsA("JointInstance") and not v:IsA("BodyMover") and not v:isA("Humanoid") and not v:IsA("Model") then
						v:Remove()
					end
				end
				Model.ChildAdded:Connect(function(c)
					c.Parent = nil
				end)
			end
		end
		
		for _, part in pairs(parts) do
			local m = Instance.new("BlockMesh", part)
			m.Scale = Vector3.new(0, 0, 0)
		end
		
		local tools = b:GetChildren()
		for i, tool in pairs(tools) do
			if tool.Parent then
				wrap(function()
					tool.Parent = c
					for i, v in pairs(tool:GetDescendants()) do
						if v:IsA("Sound") or v:IsA("TouchTransmitter") then
							v:Destroy()
						elseif v:IsA("BasePart") then
							v.Massless = true
							v.CanCollide = false
						elseif v:IsA("LocalScript") or v:IsA("Script") then
							v:Destroy()
						end
					end
					
					if tool:FindFirstChild("Handle") then
						local handle = tool.Handle
						local fakeHandle = handle:Clone()
						fakeHandle.Name = "FakeHandle"
						fakeHandle.Parent = tool
						local w = Instance.new("Weld", handle)
						w.Part0 = fakeHandle
						w.Part1 = handle
						handle.Size = Vector3.new(0, 0, 0)
					end
					
					tool.Parent = b
				end)
			end
			if (not parts[i]) then
				tools[i] = nil
				tool:Destroy()
			end
		end
		
		wait(.2)
		local amt = #tools
		
		wrap(function()
			local connection1
			
			connection1 = game:GetService("RunService").RenderStepped:Connect(function(step)
				for i = 1, amt do
					local tool = tools[i]
					if parts[i] then
						tool.Parent = b
						tool.Parent = c
					end
				end
				
				if _player.c() ~= c or c:FindFirstChildWhichIsA("Humanoid").Health == 0 then
					connection1:Disconnect()
				end
				
				utilityElements.Replicate.Text = ("Replicate (%dfps)"):format(1/step)
			end)
		end)
		
		local connection2
		connection2 = game:GetService("RunService").Heartbeat:Connect(function()
			for i = 1, amt do
				local tool = tools[i]
				if parts[i] then
					if parts[i].Transparency ~= 1 then
						local p = _cframe.toWorldPoint(parts[i].CFrame) * offset
						grip(tool, p)
					else
						local p = _cframe.toWorldPoint(CFrame.new(0, -250, 0))
						grip(tool, p)
					end
				end
			end
			if _player.c() ~= c or c:FindFirstChildWhichIsA("Humanoid").Health == 0 then
				connection2:Disconnect()
			end
		end)
	end;
}
_cframe = {
	diff = function(a, b)
		return (a:Inverse() * b)
	end;
	toWorldPoint = function(a)
		local arm = _player.c():FindFirstChild('Right Arm') or _player.c():FindFirstChild('RightHand')
		local off = arm.CFrame * gripCenter:Inverse()
		if arm.Name == "RightHand" then
			off = arm.CFrame * CFrame.Angles(math.rad(-90), 0, 0)
		end
		return _cframe.diff(off, a)
	end;
	tween = function(object,style,direction,t,goal)
	    local tweenservice = game:GetService("TweenService")
	    local tweenInfo = TweenInfo.new(t,Enum.EasingStyle[style],Enum.EasingDirection[direction])
	    local tween = tweenservice:Create(object,tweenInfo,goal)
	    tween:Play()
	    return tween
	end;
}
scriptList = {
	Character = {
		['Titan']			= {"rbxassetid://3600286284", "rbxassetid://3070358214"};
		['Winged Titan']	= {"rbxassetid://3593786550", "rbxassetid://3070358214"};
		['Part Surround']	= {"rbxassetid://3546680077", "rbxassetid://3546673786"};
	},
	Mechanical = {
		['Spiderbot']		= {"rbxassetid://3040869607", "rbxassetid://3070355648"};
		['Drone']			= {"rbxassetid://3074236927", "rbxassetid://3074245958"};
		['Noise']			= {"rbxassetid://3193712297", "rbxassetid://3070358314"};
	},
	Aesthetic = {
		['Wings']			= {"rbxassetid://3040946714", "rbxassetid://3070358381"};
		['Tail']			= {"rbxassetid://3041387168", "rbxassetid://3070358314"};
		['Star Glitcher']	= {"rbxassetid://3074734519", "rbxassetid://3074751071"};
		['Tentacles']		= {"rbxassetid://3074817074", "rbxassetid://3074820325"};
	},
	Weapon = {
		['Master Hand']		= {"rbxassetid://3040943596", "rbxassetid://3070358267"};
		['Ravenger']		= {"rbxassetid://3040945482", "rbxassetid://3070358154"};
	},
}
wrap = function(f)
	return coroutine.wrap(f)()
end

if game:GetService("RunService"):IsStudio() then
	guiLib = require(screenGui.GuiLib)
else
	guiLib = loadstring(screenGui.GuiLib.Source)()
end

for title, tbl in pairs(scriptList) do
	local frame = pageScripts[title]
	for name, info in pairs(tbl) do
		local btn = interactiveButton:Clone()
		btn.Name = name
		btn.Text = name
		btn.Parent = frame.Elements
		btn.Icon.Image = info[2]
		
		guiLib.circleInteractive(btn)
		guiLib.colorInteractive(btn)
		
		btn.MouseButton1Click:Connect(function()
			local scr = game:GetObjects(info[1])[1]
			local source = scr.Source
			
			if game:GetService("RunService"):IsStudio() == false then
				for i, v in pairs(scr:GetChildren()) do
					v.Parent = script
				end
				wrap(function()
					local func = loadstring(source)
					spawn(func)
				end)
			else
				scr.Disabled = true
				scr.Parent = _player.c()
				wait(.1)
				scr.Disabled = false
			end
		end)
	end
end

repeat wait() until pageLayout.CurrentPage

guiLib.draggable(mainFrame, titleFrame)
for i, v in pairs(toolbar:GetChildren()) do
	if v:IsA("TextButton") then
		guiLib.circleInteractive(v, 2, 1)
		v.MouseButton1Click:Connect(function()
			pageLayout:JumpTo(pages[v.Name])
		end)
		pageLayout.Changed:Connect(function(p)
			if pageLayout.CurrentPage.Name == v.Name then
				guiLib.tween(v, "Sine", "Out", .5, {BackgroundColor3 = Color3.fromRGB(255, 118, 26)})
			else
				guiLib.tween(v, "Sine", "Out", .5, {BackgroundColor3 = Color3.fromRGB(236, 109, 17)})
			end
		end)
	end
end

for i, v in pairs(utilityElements:GetChildren()) do
	if v:IsA("TextButton") then
		guiLib.circleInteractive(v)
		guiLib.colorInteractive(v)
	end
end

utilityElements.Reset.MouseButton1Click:Connect(function()
	local c = _player.c()
	c.Humanoid.Health = 0
	wait(.55)
	for i, v in pairs(c:GetChildren()) do
		if v:IsA("BackpackItem") then
			v.Parent = _player.b()
			v.Parent = _player.p
		end
	end
	repeat wait() until _player.c() ~= c
	_player.c():WaitForChild("Right Arm")
	wait(.25)
	for i, v in pairs(_player.p:GetChildren()) do
		if v:IsA("Tool") then
			v.Parent = _player.b()
		end
	end
end)

utilityElements.Block.MouseButton1Click:Connect(function()
	local c = _player.c()
	for _, v in pairs(c:GetChildren()) do
		if v:IsA("BackpackItem") then
			for _, m in pairs(v:GetDescendants()) do
				if m:IsA("DataModelMesh") then
					m:Destroy()
				end
			end
		end
	end
end)

local noclip = false
utilityElements.Noclip.MouseButton1Click:Connect(function()
	noclip = not noclip
end)

utilityElements.Tools.MouseButton1Click:Connect(function()
	if utilityElements.Tools.Text == "Load Tools" then
		_functions.tools(120)
	else
		utilityElements.Tools.Text = "Load Tools"
	end
end)

utilityElements.Replicate.MouseButton1Click:Connect(function()
	_functions.load()
end)

local flipped = 0
utilityElements.Flip.MouseButton1Click:Connect(function()
	flipped = (flipped + 1) % 4
	if flipped == 0 then
		offset = CFrame.Angles(0, 0, 0)
	elseif flipped == 1 then
		offset = CFrame.Angles(math.rad(90), 0, 0)
	elseif flipped == 2 then
		offset = CFrame.Angles(0, math.rad(90), 0)
	elseif flipped == 3 then
		offset = CFrame.Angles(0, 0, math.rad(90))
	end
end)

game:GetService("RunService").Stepped:Connect(function()
	local c = _player.c()
	if noclip then
		local descendants = c:GetDescendants()
		for i = 1, #descendants do
			local v = descendants[i]
			if v:IsA("BasePart") and v.Name ~= "HumanoidRootPart" then
				v.CanCollide = false
			end
		end
	end
end)

workspace:WaitForChild("S") end
}

-- without me eminem

Tab:Button{
	Name = "Cryptonic Hub (for the new versions of ragdoll engine)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/martinelcrac/cryptonichub/main/Ragdollengine.lua'))() end
}

Tab:Button{
	Name = "Meepcity GUI v2",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/synolope/meepcracked/main/loader.lua'))() end
}

Tab:Button{
	Name = "Da Hood Crasher (takes a few minutes)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/lerkermer/lua-projects/master/SuperCustomServerCrasher'))() end
}

Tab:Button{
	Name = "Art Stealer v2 (READ THIS: controlc.com/e911eb32)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/aCFfd9Uq"))() end
}

Tab:Button{
	Name = "NDS/Natural Disasters Survival GUI",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/2dgeneralspam1/scripts-and-stuff/master/scripts/LoadstringUjHI6RQpz2o8", true))() end
}

Tab:Button{
	Name = "AdminJoy v2 (old kohls admin script)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/67zRS6vS'))() end
}

Tab:Button{
	Name = "Funky Friday Autoplay",
	Description = nil,
	Callback = function() local vu = game:GetService("VirtualUser")
game:GetService("Players").LocalPlayer.Idled:connect(function()
   vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
   wait(1)
   vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
end)
loadstring(game:HttpGet("https://raw.githubusercontent.com/wally-rblx/funky-friday-autoplay/main/main.lua",true))()
 local message = Instance.new("Message", workspace)
        message.Text = "Loaded! If the script is not working, press 'F9' to check for any errors."
        wait(4.5)
        message:Destroy() end
}

Tab:Button{
	Name = "Sniff Hub",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/2dgeneralspam1/Sniff-Hub/main/Sniff%20Hub"))() end
}


Tab:Button{
	Name = "Wizard Tycoon 2 GUI",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/TrixAde/scripts/main/Wizard2PlayerTycoonTrixHub.lua"))() end
}

Tab:Button{
	Name = "Basic ARB/Auto Rap Battles GUI",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/55B8EXcR'))() end
}

Tab:Button{
	Name = "MM2 GUI (not working rn)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('NEEDS TO BE UPDATED'))() end
}

Tab:Button{
	Name = "Scorpion Blue (key in gg/YNC3u8jCt5)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://www.scorpionadm.in/script'))() end
}

Tab:Button{
	Name = "Prevail X",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/mHfK0Xk4'))() end
}

Tab:Button{
	Name = "Scorpion Cracked",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/TrixAde/scripts/main/PrisonLifeScorpionAdmin5%24.lua'))() end
}

Tab:Button{
	Name = "Nexus Hub",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/GwnStefano/NexusHub/main/Main'))() end
}

local Tab = GUI:Tab{
	Name = "r6-animations-and-hubs",
	Icon = "rbxassetid://8569322835"
}

Tab:Button{
	Name = "FE Bike Script (get hats here: pastebin.com/9vCnqaaF)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/9vCnqaaF"))() end
}

Tab:Button{
	Name = "FE Winged Creature",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/atk1bMcg"))() end
}

Tab:Button{
	Name = "FE Tornado (paid hats: pastebin.com/E82iYWUz)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/E82iYWUz"))() end
}

Tab:Button{
	Name = "FE Flying Gunner (paid hats: pastebin.com/cPNhDNJR)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/cPNhDNJR"))() end
}

Tab:Button{
	Name = "FE Human Car",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/3xUHm1qq"))() end
}

Tab:Button{
	Name = "FE Floppa (info+source here: pastebin.com/LFH0YKP5)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/LFH0YKP5"))() end
}

Tab:Button{
	Name = "Ornithopter (info on hats: bit.ly/3xkwomD)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet(('https://pastebin.com/raw/nAWpBaQF'),true))() end
}

Tab:Button{
	Name = "Semi-FE Sonic (effects are client-sided, run netless first)",
	Description = nil,
	Callback = function() loadstring(game:HttpGetAsync("https://pastebin.com/raw/SyF5t70A"))() end
}

Tab:Button{
	Name = "FE Hammer (hats: controlc.com/cbfa6964)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/Lgirrm5c"))() end
}

Tab:Button{
	Name = "HatHub v1 (hats: pastebin.com/raw/EzrGr8w2)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/1Cjz1RMH"))() end
}

Tab:Button{
	Name = "HatHub v2 (hats: gg/naEjFwvK3g)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://textbin.net/raw/rvohv1nvuf"))() end
}

Tab:Button{
	Name = "Syntax v2 (key is Syntaxbesthub)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet(('https://raw.githubusercontent.com/Vallater/SyntaxV2/b7a88a7b84174e3c2220c7a8ca477e40699ddd2c/Syntaxontop'),true))() end
}

Tab:Button{
	Name = "Syntax v2 Reborn (key is also Syntaxbesthub)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet(('https://raw.githubusercontent.com/Memeboiyot/SyntaxRebornOfficial/main/SyntaxReborn'),true))() end
}

Tab:Button{
	Name = "Syntax v3 (key is SyntaxV3Free)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/Memeboiyot/Syntax-V3-Free/main/Syntax%20v3", true))() end
}

Tab:Button{
	Name = "SCP 096 (hats: pastebin.com/raw/2tiTqQH7)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/2tiTqQH7"))() end
}

Tab:Button{
	Name = "Chinese Loubou Slasher Infinite Robots",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/KissxTay/caramelldansen/main/chinese%20event", true))() end
}

Tab:Button{
	Name = "FE Parkour v2 (cmds: controlc.com/8b1445c1)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/1dup3HSe',true))() end
}

Tab:Button{
	Name = "FE Drivable Car (requires Eltoria RX750 or ANY other waist item)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/MonkoTubeYT/carscript/master/!carscript.lua',true))() end
}

Tab:Button{
	Name = "FE Hat Universe v2",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/vGL3pJyf", true))() end
}

Tab:Button{
	Name = "FE Hat Universe v1 (run netless first)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/4B4fktPS", true))() end
}

Tab:Button{
	Name = "Fatass Script (hat needed: demonic greatsword)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/tBk7NxXe"))() end
}

Tab:Button{
	Name = "FE Block Gun (hats: controlc.com/f52e5df8)",
	Description = nil,
	Callback = function() return(function(h,a,a)local k=string.char;local e=string.sub;local n=table.concat;local m=math.ldexp;local o=getfenv or function()return _ENV end;local l=select;local g=unpack or table.unpack;local j=tonumber;local function p(h)local b,c,f="","",{}local d=256;local g={}for a=0,d-1 do g[a]=k(a)end;local a=1;local function i()local b=j(e(h,a,a),36)a=a+1;local c=j(e(h,a,a+b-1),36)a=a+b;return c end;b=k(i())f[1]=b;while a<#h do local a=i()if g[a]then c=g[a]else c=b..e(b,1,1)end;g[d]=b..e(c,1,1)f[#f+1],b,d=c,c,d+1 end;return table.concat(f)end;local i=p('22B21C27521D21G27521C22F22922L22D21D21M27923B22D21W22R22D21U21Y22H22B27E21J27922O22K22922127M21V21D21N27923G22N22B22922K27U27W27M21D21L27923722G22921U22922B21W28A21F2792392201121D21O27922V22922H21W23A22N21U28E22H22K22C21D21K27T2861G23C28V21U21D28M27528O1221D1W27922Q22N22A22K22N22022B27V21V21V27P21U22D29427827522M22D22021W21D21I27929A22M22C22K27E21P27923522B27Q29T28Z22122V22D2932A529K22D22L22N21Y27E21Q27H27J23822D21V27Q2A922922M21W27Z29E21C23D21V23527727923H2AZ22G28027922R21S22D22B22H2862BE21V2BG28C27522B28Z22N21X21W22H2A12AO2BT29W22928K2C121C29W21V21X27D29D27922E21W21S21D21H27922S28Z21V22N27F2AE21W21W28I22G27D2B429529K22N2CR2BY22N22M21D27S27522U2BL21W28Z132CC2A022D21Z27927924W22U26O2DF2DK21D2AV27523A2BZ22C2DP21U21V21W2912AN29Z21C23I27C27E2812752352CQ2CS2CU21W28Q2E321C2E52CR22B2CT22D2B429H29627522O22N29U2D022M2DK27525S1F2ER2752DJ2ER25C2EU2ER21G26O2C623622121S22929T2CH27922C22D2C42BG27G27529O22922C2DU21U2BZ22F2CO27527I21W23J22A22I2D727Z21327921U22A2202F821V27J22H22C1A1V1V151312151212161114182C622R2BW21U27Q2DB21C21S22K29C2DY2FC2FJ2BC2BT28F29C2A627522A21X22K2AB2A42BS21C21Z28Z22J21V2F72GP29J27523C2CA2B322N2G629L2CY22O28G2A428S27522S28H22M2HE28G2EH22B2212D327922A28F2A92AB2CW27523H2G32AB29T21F21D21D2112792DP2A92DS2DU2DW22C23J22E23729S27Z2D421C2AY2FL22N2I22CI2752AR21X2G42I921C2FR23H2BW2J52DY22G2FD29Y2A72JE2C628527D28H21D2AD27523721X21U29W2B42372E12JL21E27922K2A42B72JZ2K02I422A21Y2J623D2HX2CR22M2GP2HT21C23622N22C2212EM2EO22H2D12C623723A28H2CB21D2792CG2DY28H21U22L28B29K22H22F22G21W1G2352KX2GY21C27V2L72EK21C23G22D2CE2L52L72J121C2D82DT2CN2KS2FH2EV142342IG2FZ2EV192EX2DK25C23Z2LT2752K327528H2CG2JN2EC22K2L122M2KJ28W2KL2D22EB2ED2E72EH21W1021D21R2L022F2G628W22123922M22929N29X2GQ28H2CN2HH2M82MA23J2FM2MJ2C42ME2GQ27V2CG2K12292CN2EB2362BX2D822M1123822N21Z2D22IV2372D12A128J2J62HJ22L2HL2G62L823822H2MX2FG21C22Q21X22M27L27N27P2AC2AP2A927M22R28K21S2BK2JF27528U28W28M2FP21C2JU22M2NQ2H62G627E2H221C23C2FD2JZ2BG2IV23F22D2212NL2NN21C2IV2N12L827B2CB2O32FR2O827O2GP2O32O52O727M2PH27E2H92OY2HR22A2FD2A42DY2OL2A42LC2G42CQ2FN2IU27T22G22129U22B27Z2O32352H62NM22R2AB22D21S2ON2IV28827X2DT2BH27528328528727V2QK21D2FY2IA22922022H22L2CA22R2QY2H52N72D122Q2FJ22H2J42L82NW21W2BG2B721S2NM2L822G21X22F27E2N12R12QZ27V2EP2R622C2R821V2DK1T2791Y23F2792LO21C1G1C2DK2JX1Y2752JX2B72S521C2JX1G2F12S22ER2LJ2792JX2KS2S72792OW2DL2SC2SG2DK27S102DF29628C2SM2762792SE2SB2SM2JX2O32SB2SD2ER2812SM2KS2M72T12KS2KS2AV2T321C2TC2S82SQ2MN2SM28M2TJ21C28M28M2MN2S02TQ2SQ2TH2TP2JX2JX2TT2SZ2KS2JX2N121C28S2SL2DF2S12T12DF2S62TK2T52UC2SQ2UB2792T92SZ2TP2TE21C2TG2TK2TY2TL21C2TN2TI2T02752TR21C2U121C2KS28M2UD2SQ2UR2U02U92V12SQ2U529J2KS2DY2TU21C2152VF2UO2S02JX2J22OV2FZ2B322C22N2KY2LJ2F722H2QL2DY2PC27R27T2QR27Y2OO2FR2QJ2W22DY2E02CB2LJ29O21Z28A2DY22E2DQ2FA2M22MV2I82OW2BZ2G421U2M32GR2GT2RA2FE2EV2EZ2S121C2S42792962WW21C1M23H2792192V92VD172X52V92X32XA2U321C21G2X92752X62SL2RZ2S92RX1B2TV2DY2T12UY2CI2XR2TV2SO28M2VE2TK2752782VE2162V91G1Q2P821C2A627S1G2KS27S27S2LC2Y72TZ2SR2YD21C28C2T12H92YF28C2UF2Y72TK2H227S2Y32S12XG2792YV2UT2RZ27S2O32Y52Y727S2E31U21C2X02DF2Z828C2SO22O2Y728C2KS21I22A2SQ2U72SQ2YX2752ZM2ZO21C1A2XB122791L2X72XF2XH21C2ZX2XK2SQ2Z32ZT2YH2EB2TV2S12SM2782KD2SJ2XF2V92VE2ZT2KS2XC2751O2V92JX2ZR310M2X8279310I2Z031042T02FY31072DF2ON2RX2Y0310F2752T12Y121C2XT31122782SO2782YH2SM2CI2TP2CI2CI2V42A62DN2UT27527S2XQ311N2Y731182Z52Y82DF27S2YH2792YJ2DK2CI311W2DF31162SI310O2V921C2XJ2SQ2792VH2SZ275312C2V12LC2K82DU2B32GP2B72A121Z2OO2MH2EF2E82J62MC2EP2I32D52D72D92EV2762M72QA2MA312U2N82MG2E6312R2MJ2ML31372EE2EG2B428Q2U122Q2L12MQ21W2MS2MU2MW22C2ON2102AP28I2EP28Y2GO22D2MT2WJ2MX1Z2AE2OH22K2212E52372MJ27M2IQ2IB2F92LC2IB220313V27Q2DF25S2731Y22B2BB2EB314E2D629O2BM313L2WS2RC2RH2RJ2AU2AP2HE2D129U2AT2A129T2EV22H2LS2N1313322F22M2N42O12B42R42D22II27522Q2FD28J2ME2CK21U21T21X313X313N2AB2942U122O2FM2NW21U31452QX21V23J22M31442KZ2QV220315O315Q27E2SY314E23522M22F2R321U314Q2842MR2VL275162RX2742SK2UW2SQ311D2UX2TV2DK2XY310E311C311M2TV2LJ2XU2V33172311A31113117311U2752SM2A62SO316W2A62U42TK27828M2UU2UA316W3176310B316X2DF2CI2X131732TW311231743119317W317A2OW317D317B317227S317F310F31222HH2XX310F317Q317N310F3171311E2YR2DF31873112317H21C2HH278296317I310F28C28M2SU310F27G281318V310C21C318Y31122AD3192310F2AV2TM2752CI1X316T311H311M318O318N317A318Z21C3141313R318H318E319D311J21C315I311V313031212VA31992Z9319V317A318T21C318V2CI212319131A1319W2FY31952CI2142UZ31722A6319B3114275317E319E319W2VH2A631A2319J21C313R2SP31AH2S02JC2JH2OW2KO2KQ27E2S12CG2OW2JJ27M229316721C2IB315B28W21X2FC2WU2F0279311L1Y112VI2UI2TK31BK2TV2TA31132SR2UN2T72ZY2SA2V831BM2CI1M2DF2812ZI2ZZ2UJ312722R313023I2VI3128310E312B2VI1831AT2FB2JE2ON316N2JZ2N92CQ2M12C7312T2EN2MD2KM2IV2D628J2D92GQ312N2WU23Z313031302ET2J629L2CZ2ME2ER26O22V2LX2DG2342F32DY21Z28V21W21C24421S1D21M26F24326O1F31CM22K31BD2ER2DH31DA2792LR2LV31DD2K42292K6312H2K9312K27E31412752KF2KH316F316H2LA316K314S2I22IV2I52VP2I82H9314E316A315R314U2BG2JC314X31CM2ZF21E25025Q25W21T26H2552392MM2AE316G316I31EF2MR21C1K23K21K25426725923323A21C1521F1223R25G24D22S23927524026G25122V1421Y2372PB2E12W327J2PG2OA2C62AY22A2FM2Q22E422C22C23D28K22L21C24Q24P31GJ31GJ23T31DQ2QI2W12QL31A42FQ27J2W521U2KP2VR28E28G313T28A2LJ2J32J52OW22S28G2RK2A42OW2HQ2JS2PU2792W827E2DY2EF28G31CW2KM2PJ2O631G42GP2M7315K2OD21U2OF2QF2OI2L82PW2GQ22A2K52KN2KP31G12N12NV2NX22C2HO21W31HB2A431B02WH21C315O2CM2GQ23C28W2DK1J2LO2RY2VI310K310F2XE2ZR278310R2751I2M131C72ER1Y23627931BU2VI2SY31BP31J62LJ31BO2IV2TD2V92962TH2H92UU2O3317Q31082SZ31712U52A62U827931J92SZ31JB2U2319X2TX317928M31BG31122YQ2VD319Y2ZP2V931J62U131BO2U52UG31JP27531AF31722YC316T2UN31JE2TK2SY2UU31KK311231JK310G31K3311U31KB21C31KD31JA31KG31JD31722JX31E8317228M31AQ317721C31K1310F318R31K431KS31JR2V931JT2ZY31KI2SQ31JG316W2EB31JJ2ER31K231L831KR3172319W317C31JS31KW2KS31LF31KZ31JX319Q317927831L631JM2DF2ZM31D031J62DY31J62QU2SR2SV31KE21C31AB31LR2SQ312F2T631LP21C31GR31MJ31ML31KV31AG31LE31KY21C217316T2YH21831L131MS316T2UY31MW317Q31MT31MP311631MW2TU31M22YY31K52DF31ML318V2XI21C21A31MM317931KF31MP31KH31MR2UB2UU1H2RX318B1I2DF22C31KP31LN21B31NA2791J316T2DF1K31MR2ZX2EV2YH31BM31BY2TH31MN316W1N3130311031J631O031MP2DF310M31BM1P31MR2Y631MP2YH1R2SR2YH1S2ER2YH2SO22I2ZY2ZR31OY31IV21C23O31K52RZ27531OO2S231BK31OR31BM31OU31BM2RW31BO2Z831NK2V92RW2SO2RU2UN2ZR31PM31C227522231P527931P82Z42DF31PB31P827531PD31PZ21C2RW31IQ31PS2KS1V31PQ21C31Q631Q92233127312F310A31P621C31OH2S231NG31O231MR31ND31MI31BM31BI31BM2ZV2SB31KS1331NI21C1431LT31JV2TK31PV2TK2JX31PB31R421C31PD31R71531OS2SQ31QZ2T12YH316P2UU31PH2SR2UY2X9317531QY31RK2TV316P2TU317P2TK31QZ31OP2SQ31LF28M31JI31K031792CI2YQ2JX311I2V82XE31JC2KS316P31JN31NY312E31QX31RV31BQ31KX2TH31R3316U21C31R631SL31R931SL31RB31RF31RD31RC2JX31RH316W31RJ31RN31RM317O31RO31RN31RR2SZ31RT31ST31RW2JX31RY31L531LZ31TB31MF31S331OV317A316N2ZY31BS2UN31SB318J31SD31AC31MF31KS31KA31BP31NF2LT31IO27531QJ1G311L310L31MA27931OM31SJ31MU2SQ31SN31OT31SU31R831TG2JX2SO31CZ31PN310031UF31Q921M31TV31QH31PV31PA31U231Q031UP31Q331MC31SY31JU31PK2DF26W31OZ310031UY31P227231PT31P72T031Q231PY2DK31Q12RV2X231QT21C2732V931Q82ZR31VF2LO31QF2RX31QH31TY31K931O32TH31QO2UG31BS2DF31QR2ER31VD310E31QV31SF31R031LV21C31SK31OQ31UA31SP31U931SS2JX31SR31R731RE31R731SW2TV31UU2TV28M31T031WJ31T231T131T42V931T62JX31SG31WA31R12TV31S0318W31S231TD2UG31S62TU31S831JU31TM2SN31TO312F31BO31WT31JU31W331W531U731W731XG31WU31WC31SL31WE31SL31WG28M31WI31RL31RP28M31XL2UY31WP2V2318031WS31U631T931MX31WX31M031WZ31S431TH31S72UH31X5319G31X731KS31K72SZ31J631TS2VE21A31UL31NZ2T031FR31QM31VR313031O72ER31VW2DK31VY2TK31W031TQ31W431R031CD31S921C31X631AS31KS31X92SZ31SK2UN31Z031Y931SC31YC31QX31YF31VZ310U2752V023J31X327531IZ31272UT31SG2SA31VL312D2V12GV2JE2DK2SA31ZN310A31SG2WW31ZS31TP2V12S12GU27931DF31IK31GI31GK24P26X31DQ2S122K31CO2KK31CR27931CT2LL2DA312M2DD31DT2ER31D22LC31D4315G31D731D92LV23431D031DU2DI2LQ2LS2DF31OM2751M31VD310Q310G3100321B31IO2XE317C31GG2XM2SP316S31BO31M72YS31XZ2Y72UU2LC317Q31LH319Z31TG31S62HH2KS31S6321M317931UD321P27S2UU31LJ31122KD318H2M7310E321X2SZ27G2V4321G31MR2H92TU321L31JL3222318431WU3225316W321S3112322S321V2SB322D2V93220322M31MF322331T8321Q316W31JZ310F31YD317A322B2TK322X2KS322F31SE31ZT2252YW3211317U31YV2ER31BU318D316T3116319P31J4317831BS31162782T12CI2782J12963187313R2IV2DK2LC31BS28C319U2SM2812YF27528C281318R32412YK2SR3248323431A52YQ324E319Y2SW324I31IO324O2792Z827G2YF31OY2812EB2ZR2SU2KS2Z42AV2AD28S1G22W2VJ32552SR2AV325D2DF2AV322L2VJ2EB2T12MN2AD2V02MN317I2VE2Z8325327G31412S729J1Y28M2II31KD2J731AO2II31UD31MT314131OU31UG27932672S2325T31AJ325X31LY31J623B32622SQ21I326531UB326831UQ31P2325R326B31AO2S72DN27S3141316S2ZJ2VJ31NP31IS310032702Y82ZK28C2VH327131CB310328C31L02Z428C28C313R21E23C31X027923E324I316V31TB327C27527G27G319R31A5322J327Q2SQ2U3327I27G320031TB31ML327H31TB31TI2S72812Z331K4324H2T128S328D2SR2AD2CI31M931A52AD2WW3288316T28S324Q328C2U6328R2T1328G21C328I281328K2SR324B311U2T1324Z328S275329331AB2SM28S2Y331MP328E31MT2SM2AD31N631722AV2X631MF2MN329J31M331AC318R2812VH32573295319X2YL329T281329S31A5281329731K4329A2SR329C31722AD329M2SM329I3179329L2ER28S325O31YA329Q329431A532492752AD328I329T2AD31BS329331NG329E31MD2T82UV2JX318V28131NX2SE3292317A322Q2UV32AN328J31Y8329Z31NF32A632AU2DK328X2SQ32AY21C31NX31NP32B232AK32B532AV32AP328Z31A52SE329821C32A3328Q28S329D32AL31C931MF2AV31QJ2SM2MN31O32DK32AE319Y28131NS329Y28132BL32AM32BN32B8329331NP32BS32BU31K432BW32BB32A82752AV31O531722MN31BY32C6329O32AG21C32CA3172281310M31MF28131OD32D321C3217317231M432A4328R2Y632A931SM32AD2VJ31BS328E2ZX32BV31UB31C3311X329T2UN324A31ZO32B228128M32DT318C2EU2812RW32BD2DK32DR31RJ32DR32E032BP32CC32D021C31Q832D631BI31MF28S32E632DL31NX31C3329X2S22Y632932ZV1Y2MN319532E931ND32BG31QW31O032DR31ND32DR31SG32EX27932BG31RB31WG32ER32DW2X932AT31ME2FQ32B72SD1D32B931CD32DN31NY32F6329W21C32F832BY32FA31C332BO32DW32FG329T325H32FJ32B932F82TO32BC27531A432BE32AQ31A532FS31A532FU31US31MP32932ZT32FH2V428119317928132EB32E72WX32E92XO317C2RZ28132ED2S223232B91E32E932FE32E1310A329T31BE31C32DF32DR32102S8327I32DU317928S31J2329B328R32BX2UV23731792AV31SG27928S325G32D92EC32H832HN31MF2AD32GI328T32BM32HT2AD238328F2UV31FR2HH28S31NS2AD32BS32HS32CL326132BS31FI32EE32EA328N328R23D32HM327I32IB32I6328R28S2FY32BS327L32IB32HA32DB32CM32F932HG2OX32DG32HL32BS31QH32IY31792AD32CK2UV2AD32HD2AV329G32C32LD317929J329M2792AD29J318R28S2VH32I431K432IZ32BY32J32AD32J5329H310132AB32JS31MF29J31QJ32JE319G32JH32CY2UV32BS32IQ32DL32HD2AD32FA32DE32IA329N32IX31K42X432IB32KE32BB32JO2UV32J621C32J831ZI2DZ32JB32BZ2DF32JF319Y32JI32K232KD32J132BT316T32JP31MY32DE31ZK329K31QI32KP32JX32BY32JG31YA32I232KV328R32K432I732K632FZ32DE32IO32KB318028S2ZF32IP32ID32IS32BY22Q32IU32KA32HJ32DH32HM22P32HO32LY32HQ31B727932I121C31C532I431CD28S32M032BB32LN32LA2SG32JK328R32MA318V28S22S31Z232HM32LE32IK32L132BY22U32LT32IW2TW31QZ28S22T2RX32GF32MW32KX32KG32M432M632HM32MX32M132MC32M42SE32MF32N027532MI31IF32ML32K332LP32L132FY32LS317C2AD2AV32IH32LK2V428S22V32HO32NT32M131QH32N332LC32NS32KX32N831K432NA32HM32NV31A131OD32MJ32NG32MK32H932NI32LG32MR32C032IV32CV32KC328R325932IB32OL32BB32NX31K432N432BS32ON31IO2AD32N822E329432NB21C32ON32NE32MK31WG28S32GF32HB28S22X32IR21C22Y2SC327I2AV2VE31OR32HK31NY28S32IJ328E22Z32PA23032PA32PC32842AV2SI2ZF32PI310332DA1G32EK28S2V42AV23132MT32DI328R32GS32DL233329N325H28S31RJ32CU32MW2LT22831Q922T2LT2ZR23031YJ28S31WT2Y6328E2292X22X428S22Y2LT316P2ZR32QX31P232QN32PX31RO32ND32O821C32QT32QI31IO28S2352RX32PN32HR32KZ32HU32BY32HW32HY2AD32I031K432I332HM32H42X231K42KY31SA31Q932RU310U32QD2793219328R32RX32QI2ZR32RX32RB32R5310U32RG31142Y632L02FY2Z432L02VH1W31OM32KU32I42RZ32PK31V632MO32PN2Z4328E2ZK2XC28S27Z2KS2X631PO32QL310023E32QO32DS328E28S32DV32I7323W32I732GB31K431YQ32MO27432DL32PR32PE318421C32PV2VJ31VK2VI');local a=(bit or bit32);local d=a and a.bxor or function(a,c)local b,d,e=1,0,10 while a>0 and c>0 do local f,e=a%2,c%2 if f~=e then d=d+b end a,c,b=(a-f)/2,(c-e)/2,b*2 end if a<c then a=c end while a>0 do local c=a%2 if c>0 then d=d+b end a,b=(a-c)/2,b*2 end return d end local function c(c,a,b)if b then local a=(c/2^(a-1))%2^((b-1)-(a-1)+1);return a-a%1;else local a=2^(a-1);return(c%(a+a)>=a)and 1 or 0;end;end;local a=1;local function b()local f,e,b,c=h(i,a,a+3);f=d(f,48)e=d(e,48)b=d(b,48)c=d(c,48)a=a+4;return(c*16777216)+(b*65536)+(e*256)+f;end;local function j()local b=d(h(i,a,a),48);a=a+1;return b;end;local function f()local c,b=h(i,a,a+2);c=d(c,48)b=d(b,48)a=a+2;return(b*256)+c;end;local function p()local d=b();local a=b();local e=1;local d=(c(a,1,20)*(2^32))+d;local b=c(a,21,31);local a=((-1)^c(a,32));if(b==0)then if(d==0)then return a*0;else b=1;e=0;end;elseif(b==2047)then return(d==0)and(a*(1/0))or(a*(0/0));end;return m(a,b-1023)*(e+(d/(2^52)));end;local m=b;local function q(b)local c;if(not b)then b=m();if(b==0)then return'';end;end;c=e(i,a,a+b-1);a=a+b;local b={}for a=1,#c do b[a]=k(d(h(e(c,a,a)),48))end return n(b);end;local a=b;local function r(...)return{...},l('#',...)end local function h()local k={};local d={};local a={};local i={[#{"1 + 1 = 111";{18;786;729;638};}]=d,[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]=nil,[#{{479;149;11;320};{409;201;359;130};{6;611;543;350};{487;103;874;755};}]=a,[#{{259;334;220;711};}]=k,};local a=b()local e={}for c=1,a do local b=j();local a;if(b==3)then a=(j()~=0);elseif(b==0)then a=p();elseif(b==1)then a=q();end;e[c]=a;end;i[3]=j();for a=1,b()do d[a-1]=h();end;for h=1,b()do local a=j();if(c(a,1,1)==0)then local d=c(a,2,3);local g=c(a,4,6);local a={f(),f(),nil,nil};if(d==0)then a[3]=f();a[4]=f();elseif(d==1)then a[3]=b();elseif(d==2)then a[3]=b()-(2^16)elseif(d==3)then a[3]=b()-(2^16)a[4]=f();end;if(c(g,1,1)==1)then a[2]=e[a[2]]end if(c(g,2,2)==1)then a[3]=e[a[3]]end if(c(g,3,3)==1)then a[4]=e[a[4]]end k[h]=a;end end;return i;end;local function m(a,b,e)a=(a==true and h())or a;return(function(...)local d=a[1];local f=a[3];local n=a[2];local j=r local b=1;local i=-1;local o={};local h={...};local k=l('#',...)-1;local a={};local c={};for a=0,k do if(a>=f)then o[a-f]=h[a+1];else c[a]=h[a+#{{52;706;905;524};}];end;end;local a=k-f+1 local a;local f;while true do a=d[b];f=a[1];if f<=54 then if f<=26 then if f<=12 then if f<=5 then if f<=2 then if f<=0 then local f;c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];elseif f==1 then local h;local l,k;local f;local e;e=a[2];f=c[a[3]];c[e+1]=f;c[e]=f[a[4]];b=b+1;a=d[b];e=a[2]c[e]=c[e](c[e+1])b=b+1;a=d[b];e=a[2];f=c[a[3]];c[e+1]=f;c[e]=f[a[4]];b=b+1;a=d[b];e=a[2];f=c[a[3]];c[e+1]=f;c[e]=f[a[4]];b=b+1;a=d[b];e=a[2]l,k=j(c[e](c[e+1]))i=k+e-1 h=0;for a=e,i do h=h+1;c[a]=l[h];end;b=b+1;a=d[b];e=a[2]c[e]=c[e](g(c,e+1,i))b=b+1;a=d[b];if c[a[2]]then b=b+1;else b=a[3];end;else if(c[a[2]]==c[a[4]])then b=b+1;else b=a[3];end;end;elseif f<=3 then c[a[2]]=a[3];elseif f==4 then local h;local f;c[a[2]]={};b=b+1;a=d[b];c[a[2]]={};b=b+1;a=d[b];c[a[2]]=(a[3]~=0);b=b+1;a=d[b];c[a[2]]=(a[3]~=0);b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];else c[a[2]][a[3]]=a[4];end;elseif f<=8 then if f<=6 then c[a[2]]=c[a[3]]*c[a[4]];elseif f>7 then c[a[2]]={};else local a=a[2]c[a](c[a+1])end;elseif f<=10 then if f==9 then c[a[2]]=#c[a[3]];else local d=a[2];local b=c[a[3]];c[d+1]=b;c[d]=b[a[4]];end;elseif f>11 then local f;local e;c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];e=a[2];f=c[a[3]];c[e+1]=f;c[e]=f[a[4]];b=b+1;a=d[b];e=a[2]c[e]=c[e](c[e+1])b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];e=a[2];f=c[a[3]];c[e+1]=f;c[e]=f[a[4]];else local h;local f;f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];f=a[2]c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];if(c[a[2]]~=a[4])then b=b+1;else b=a[3];end;end;elseif f<=19 then if f<=15 then if f<=13 then local f;c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];elseif f>14 then local g;local f;e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2];g=c[a[3]];c[f+1]=g;c[f]=g[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];else local h;local f;c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];if not c[a[2]]then b=b+1;else b=a[3];end;end;elseif f<=17 then if f==16 then local h;local f;f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];f=a[2]c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]]*c[a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]]*c[a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f](c[f+1])b=b+1;a=d[b];b=a[3];else c[a[2]]=c[a[3]]-c[a[4]];end;elseif f>18 then if c[a[2]]then b=b+1;else b=a[3];end;else local h;local f;c[a[2]]=c[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2]c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2]c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2]c[f]=c[f](c[f+1])b=b+1;a=d[b];c[a[2]]();b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];end;elseif f<=22 then if f<=20 then local f;local e;c[a[2]]={};b=b+1;a=d[b];c[a[2]]={};b=b+1;a=d[b];e=a[2];f=c[a[3]];c[e+1]=f;c[e]=f[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];e=a[2]c[e]=c[e](g(c,e+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];e=a[2];f=c[a[3]];c[e+1]=f;c[e]=f[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];e=a[2]c[e]=c[e](g(c,e+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];elseif f==21 then local b=a[2];local d=c[a[3]];c[b+1]=d;c[b]=d[a[4]];else local h;local f;f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];f=a[2]c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];f=a[2]c[f]=c[f](c[f+1])b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];e[a[3]]=c[a[2]];end;elseif f<=24 then if f==23 then local h;local f;c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];f=a[2]c[f]=c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];f=a[2]c[f]=c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=#c[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]][c[a[4]]];b=b+1;a=d[b];f=a[2]c[f](g(c,f+1,a[3]))else local b=a[2]c[b]=c[b](g(c,b+1,a[3]))end;elseif f>25 then c[a[2]]=c[a[3]][a[4]];else do return end;end;elseif f<=40 then if f<=33 then if f<=29 then if f<=27 then if not c[a[2]]then b=b+1;else b=a[3];end;elseif f>28 then do return c[a[2]]end else c[a[2]]=c[a[3]][c[a[4]]];end;elseif f<=31 then if f==30 then local h;local f;f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];f=a[2]c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]]*c[a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]]*c[a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f](c[f+1])b=b+1;a=d[b];b=a[3];else local e=a[2];local f=a[4];local d=e+2 local e={c[e](c[e+1],c[d])};for a=1,f do c[d+a]=e[a];end;local e=e[1]if e then c[d]=e b=a[3];else b=b+1;end;end;elseif f==32 then c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];if(c[a[2]]==c[a[4]])then b=b+1;else b=a[3];end;else c[a[2]]=c[a[3]];end;elseif f<=36 then if f<=34 then local b=a[2]c[b](g(c,b+1,a[3]))elseif f>35 then local a=a[2]c[a]=c[a](c[a+1])else if(c[a[2]]~=a[4])then b=b+1;else b=a[3];end;end;elseif f<=38 then if f>37 then for a=a[2],a[3]do c[a]=nil;end;else if c[a[2]]then b=b+1;else b=a[3];end;end;elseif f==39 then c[a[2]][a[3]]=a[4];else b=a[3];end;elseif f<=47 then if f<=43 then if f<=41 then c[a[2]][a[3]]=c[a[4]];elseif f>42 then local h;local f;f=a[2]c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];else c[a[2]]=c[a[3]][a[4]];end;elseif f<=45 then if f>44 then do return c[a[2]]end else do return end;end;elseif f==46 then c[a[2]]=c[a[3]];else local d=a[2]local e={c[d](g(c,d+1,i))};local b=0;for a=d,a[4]do b=b+1;c[a]=e[b];end end;elseif f<=50 then if f<=48 then local a=a[2]c[a]=c[a](c[a+1])elseif f>49 then if(c[a[2]]==a[4])then b=b+1;else b=a[3];end;else c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]]-c[a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];if(c[a[2]]<a[4])then b=a[3];else b=b+1;end;end;elseif f<=52 then if f==51 then local b=a[2]local e={c[b](g(c,b+1,i))};local d=0;for a=b,a[4]do d=d+1;c[a]=e[d];end else e[a[3]]=c[a[2]];end;elseif f>53 then c[a[2]]=(a[3]~=0);else c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];if(c[a[2]]==c[a[4]])then b=b+1;else b=a[3];end;end;elseif f<=81 then if f<=67 then if f<=60 then if f<=57 then if f<=55 then b=a[3];elseif f>56 then c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];else local f;c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))end;elseif f<=58 then local f;c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2]c[f](g(c,f+1,a[3]))b=b+1;a=d[b];b=a[3];elseif f==59 then local f;local h;local k,m;local l;local f;c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2];l=c[a[3]];c[f+1]=l;c[f]=l[a[4]];b=b+1;a=d[b];f=a[2]k,m=j(c[f](c[f+1]))i=m+f-1 h=0;for a=f,i do h=h+1;c[a]=k[h];end;b=b+1;a=d[b];f=a[2]k={c[f](g(c,f+1,i))};h=0;for a=f,a[4]do h=h+1;c[a]=k[h];end b=b+1;a=d[b];b=a[3];else local h;local f;f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];f=a[2]c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f]()b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]]*c[a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]]*c[a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];b=a[3];end;elseif f<=63 then if f<=61 then local h;local f;f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];f=a[2]c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];f=a[2]c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];elseif f>62 then e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=(a[3]~=0);b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][c[a[4]]];else e[a[3]]=c[a[2]];end;elseif f<=65 then if f>64 then c[a[2]]();else local b=a[2]local e={c[b](c[b+1])};local d=0;for a=b,a[4]do d=d+1;c[a]=e[d];end end;elseif f>66 then local a=a[2]c[a]=c[a]()else local f;e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=(a[3]~=0);b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=(a[3]~=0);b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];end;elseif f<=74 then if f<=70 then if f<=68 then local a=a[2]c[a](c[a+1])elseif f>69 then local a=a[2]c[a]=c[a](g(c,a+1,i))else local h;local f;f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];f=a[2]c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f](c[f+1])end;elseif f<=72 then if f==71 then local b=a[2]c[b]=c[b](g(c,b+1,a[3]))else c[a[2]]=m(n[a[3]],nil,e);end;elseif f>73 then local f;f=a[2]c[f]=c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]];b=b+1;a=d[b];f=a[2]c[f](c[f+1])else c[a[2]][a[3]]=c[a[4]];end;elseif f<=77 then if f<=75 then c[a[2]]=e[a[3]];elseif f==76 then local a=a[2]c[a]=c[a](g(c,a+1,i))else if(c[a[2]]~=a[4])then b=b+1;else b=a[3];end;end;elseif f<=79 then if f==78 then c[a[2]]=(a[3]~=0);else c[a[2]]();end;elseif f==80 then local b=a[2]c[b](g(c,b+1,a[3]))else if(c[a[2]]==a[4])then b=b+1;else b=a[3];end;end;elseif f<=95 then if f<=88 then if f<=84 then if f<=82 then local a=a[2]c[a]=c[a]()elseif f>83 then local f;c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];else c[a[2]]=(a[3]~=0);b=b+1;end;elseif f<=86 then if f==85 then c[a[2]]=(a[3]~=0);b=b+1;else c[a[2]]=a[3];end;elseif f==87 then local a=a[2]local d,b=j(c[a](c[a+1]))i=b+a-1 local b=0;for a=a,i do b=b+1;c[a]=d[b];end;else local h;local i;local g;local f;c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2];g=c[a[3]];c[f+1]=g;c[f]=g[a[4]];b=b+1;a=d[b];f=a[2]c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2];g=c[a[3]];c[f+1]=g;c[f]=g[a[4]];b=b+1;a=d[b];f=a[2]i={c[f](c[f+1])};h=0;for a=f,a[4]do h=h+1;c[a]=i[h];end b=b+1;a=d[b];b=a[3];end;elseif f<=91 then if f<=89 then c[a[2]]=c[a[3]]-c[a[4]];elseif f==90 then if(c[a[2]]<a[4])then b=a[3];else b=b+1;end;else c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];if(c[a[2]]==a[4])then b=b+1;else b=a[3];end;end;elseif f<=93 then if f>92 then c[a[2]]=c[a[3]]*c[a[4]];else if not c[a[2]]then b=b+1;else b=a[3];end;end;elseif f>94 then c[a[2]]=c[a[3]][c[a[4]]];else c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=(a[3]~=0);b=b+1;a=d[b];e[a[3]]=c[a[2]];b=b+1;a=d[b];c[a[2]]=(a[3]~=0);b=b+1;a=d[b];e[a[3]]=c[a[2]];end;elseif f<=102 then if f<=98 then if f<=96 then if(c[a[2]]<a[4])then b=a[3];else b=b+1;end;elseif f==97 then if(c[a[2]]==c[a[4]])then b=b+1;else b=a[3];end;else local e=a[2];local f=a[4];local d=e+2 local e={c[e](c[e+1],c[d])};for a=1,f do c[d+a]=e[a];end;local e=e[1]if e then c[d]=e b=a[3];else b=b+1;end;end;elseif f<=100 then if f>99 then local h;local f;f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2];h=c[a[3]];c[f+1]=h;c[f]=h[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];if not c[a[2]]then b=b+1;else b=a[3];end;else local f;c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=c[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=c[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=c[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=c[a[3]];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];do return end;end;elseif f==101 then c[a[2]]={};else local f;local g;c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]][a[3]]=a[4];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];g=a[2];f=c[a[3]];c[g+1]=f;c[g]=f[a[4]];end;elseif f<=105 then if f<=103 then c[a[2]]=#c[a[3]];elseif f==104 then local a=a[2]local d,b=j(c[a](c[a+1]))i=b+a-1 local b=0;for a=a,i do b=b+1;c[a]=d[b];end;else local b=a[2]local e={c[b](c[b+1])};local d=0;for a=b,a[4]do d=d+1;c[a]=e[d];end end;elseif f<=107 then if f==106 then for a=a[2],a[3]do c[a]=nil;end;else c[a[2]]=e[a[3]];end;elseif f>108 then local f;c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f](c[f+1])b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=e[a[3]];b=b+1;a=d[b];c[a[2]]=c[a[3]][a[4]];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];c[a[2]]=a[3];b=b+1;a=d[b];f=a[2]c[f]=c[f](g(c,f+1,a[3]))b=b+1;a=d[b];c[a[2]][a[3]]=c[a[4]];else c[a[2]]=m(n[a[3]],nil,e);end;b=b+1;end;end);end;return m(true,{},o())();end)(string.byte,table.insert,setmetatable); end
}

Tab:Button{
	Name = "FE Pathfinding Zombie (has fling, hats: https://controlc.com/ba680be2)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://gist.githubusercontent.com/someunknowndude/18f1d979ad9a25ad69064be75f55f735/raw/dc36f1e9ad906a7434bd77bcd0ce8218fb5f4d88/zombie.lua"))() end
}

local Tab = GUI:Tab{
	Name = "r15-supported-scripts",
	Icon = "rbxassetid://8569322835"
}

Tab:Button{
	Name = "Bighead v3 (requires rthro head)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://raw.githubusercontent.com/sysGhost-aka-BiKode/Scripts2022/main/BigHeadV3_Unpatched", true))() end
}

Tab:Button{
	Name = "Giant Avatar (max all r15 scaling settings, set proportions to 0)",
	Description = nil,
	Callback = function()     local LocalPlayer = game:GetService("Players").LocalPlayer
local Character = LocalPlayer.Character
local Humanoid = Character:FindFirstChildOfClass("Humanoid")
 
function rm()
	for i,v in pairs(Character:GetDescendants()) do
		if v:IsA("BasePart") then
			if v.Name == "Handle" or v.Name == "Head" then
				if Character.Head:FindFirstChild("OriginalSize") then
					Character.Head.OriginalSize:Destroy()
				end
			else
				for i,cav in pairs(v:GetDescendants()) do
					if cav:IsA("Attachment") then
						if cav:FindFirstChild("OriginalPosition") then
							cav.OriginalPosition:Destroy()  
						end
					end
				end
				v:FindFirstChild("OriginalSize"):Destroy()
				if v:FindFirstChild("AvatarPartScaleType") then
					v:FindFirstChild("AvatarPartScaleType"):Destroy()
				end
			end
		end
	end
end
 
rm()
wait(0.5)
Humanoid:FindFirstChild("BodyProportionScale"):Destroy()
wait(1)
 
rm()
wait(0.5)
Humanoid:FindFirstChild("BodyHeightScale"):Destroy()
wait(1)
 
rm()
wait(0.5)
Humanoid:FindFirstChild("BodyWidthScale"):Destroy()
wait(1)
 
rm()
wait(0.5)
Humanoid:FindFirstChild("BodyDepthScale"):Destroy()
wait(1)
 
rm()
wait(0.5)
Humanoid:FindFirstChild("HeadScale"):Destroy()
wait(1)
end
}

Tab:Button{
	Name = "Small Avatar (set all scaling settings to the lowest, max proportions",
	Description = nil,
	Callback = function() local LocalPlayer = game:GetService("Players").LocalPlayer
local Character = LocalPlayer.Character
local Humanoid = Character:FindFirstChildOfClass("Humanoid")
 
local function rm()
	for i,v in pairs(Character:GetDescendants()) do
		if v:IsA("BasePart") then
			if v.Name ~= "Head" then
				for i,cav in pairs(v:GetDescendants()) do
					if cav:IsA("Attachment") then
						if cav:FindFirstChild("OriginalPosition") then
							cav.OriginalPosition:Destroy()
						end
					end
				end
				v:FindFirstChild("OriginalSize"):Destroy()
				if v:FindFirstChild("AvatarPartScaleType") then
					v:FindFirstChild("AvatarPartScaleType"):Destroy()
				end
			end
		end
	end
end
 
rm()
wait(0.5)
Humanoid:FindFirstChild("BodyTypeScale"):Destroy()
wait(0.2)
 
rm()
wait(0.5)
Humanoid:FindFirstChild("BodyWidthScale"):Destroy()
wait(0.2)
 
rm()
wait(0.5)
Humanoid:FindFirstChild("BodyDepthScale"):Destroy()
wait(0.2)
 
rm()
wait(0.5)
Humanoid:FindFirstChild("HeadScale"):Destroy()
wait(0.2) end
}

Tab:Button{
	Name = "Hat Resize",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://github.com/DigitalityScripts/roblox-scripts/raw/main/hat%20resize'))() end
}

Tab:Button{
	Name = "Hat + Head Resize",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/DigitalityScripts/roblox-scripts/main/hat%20%2B%20head%20resize'))() end
}

Tab:Button{
	Name = "Hat Resize + Drop",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/DigitalityScripts/roblox-scripts/main/hat%20resize%20%2B%20drop'))() end
}

local Tab = GUI:Tab{
	Name = "outdated-scripts",
	Icon = "rbxassetid://8569322835"
}

Tab:Button{
	Name = "Harked",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/pwG8jKVV'))() end
}

Tab:Button{
	Name = "FE Hat Universe v1 (requires netless, cmds at pastebin.com/1i2n062w)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/4B4fktPS'))() end
}

Tab:Button{
	Name = "Energize R6",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/0MLPL32f'))() end
}

Tab:Button{
	Name = "C00lgui Reborn",
	Description = nil,
	Callback = function() loadstring(game:GetObjects("rbxassetid://8127297852")[1].Source)() end
}

Tab:Button{
	Name = "Telekenesis v1",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/KduE9A6z'))() end
}

Tab:Button{
	Name = "Prisonbreaker",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/FGdzK66Q'))() end
}

Tab:Button{
	Name = "Adminjoy v1",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/FGtgjKwD'))() end
}

Tab:Button{
	Name = "Client Zero (old asf)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/d03A0sMv'))() end
}

Tab:Button{
	Name = "FrappeFxcker v3 (mostly patched except tps)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/2K5UjCiY'))() end
}

Tab:Button{
	Name = "OG Fe Fling GUI (synapse only)",
	Description = nil,
	Callback = function() if syn then request = syn.request end
local req = request({
    Url = 'https://files.shade4real.net/flingerOLD.txt'
})
loadstring(req.Body)() end
}

-- CREDITS



GUI:Credit{
	Name = "MastersMZ",
	Description = "Showcased the scripts in here (but didn't make them)",
	V3rm = "MasterXasterMM1",
	Discord = "MastersMZ#5717"
}

GUI:Credit{
	Name = "Dark Eccentric",
	Description = "Also a showcaser, you can find the script owners on their channels.",
	V3rm = "||unknown",
	Discord = "DE#8076"
}
