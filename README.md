for i,v in pairs(game:GetService("Workspace").Powerups:GetDescendants()) do
if v.ClassName == "TouchTransmitter" then
if game.Players.LocalPlayer.Character.Humanoid.Health ~= 0 and game.Players.LocalPlayer.Character and v.Parent.Parent.ClassName == "Model" then
firetouchinterest(game.Players.LocalPlayer.Character:FindFirstChildOfClass("Part"), v.Parent, 0) --0 is touch
wait()
firetouchinterest(game.Players.LocalPlayer.Character:FindFirstChildOfClass("Part"), v.Parent, 1) -- 1 is untouch
end
end
end
