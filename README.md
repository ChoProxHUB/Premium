local a = game.workspace.tower.sections.finish.steps.floorRight
print(a.CFrame)
local o = Instance.new("Part")
local ply = game.Players.LocalPlayer.Character.HumanoidRootPart
o.Name = "D1"
o.Size = Vector3.new(1,1000,1000)
o.Parent = game.Workspace
o.CFrame = a.CFrame * CFrame.new(0,-1,0)
o.Anchored = true
game.Players.LocalPlayer.Character.HumanoidRootPart.Anchored = true
local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(20, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = a.CFrame}):Play()
wait("20")
game.Players.LocalPlayer.Character.HumanoidRootPart.Anchored = false
local aq = game.workspace.tower.finishes.Finish
print(a.CFrame)
local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(10, Enum.EasingStyle.Linear, Enum.EasingDirection.Out,0,false,0), 
{CFrame = aq.CFrame}):Play()
wait("12")
 game:GetService("TeleportService"):Teleport(game.PlaceId)
