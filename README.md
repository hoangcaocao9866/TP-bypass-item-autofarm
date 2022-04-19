game:GetService("Players").LocalPlayer.Character.Fortnite.Did.Value = true
wait(1)
game:GetService("Players").LocalPlayer.Character.Fortnite.Parent = game:GetService("Players").LocalPlayer.Character.RagdollConstraints
wait(0.75)
game:GetService("Players").LocalPlayer.Character.RagdollConstraints.Fortnite.Parent = game:GetService("Lighting")
wait(0.5)
game:GetService("Lighting").Fortnite:Destroy()

game:GetService("StarterPlayer").StarterCharacterScripts.Value = true
wait(1)
game:GetService("Players").LocalPlayer.Character.Fortnite.Parent = game:GetService("Players").LocalPlayer.Character.RagdollConstraints
wait(0.75)
game:GetService("Players").LocalPlayer.Character.RagdollConstraints.Fortnite.Parent = game:GetService("Lighting")
wait(0.5)
game:GetService("Lighting").Fortnite:Destroy()

game:GetService("Workspace").Items.DescendantAdded:Connect(function(v)
   if v.ClassName == "MeshPart" or v.ClassName == "Part" then
       game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame * CFrame.new (0, 10, 0)
       wait()
   end
end)
