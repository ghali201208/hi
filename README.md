local Players = game:GetService("Players")
local ReplicatedStorage = game:GetService("ReplicatedStorage")
local LocalPlayer = Players.LocalPlayer


local myName = LocalPlayer.Name


local finalRP = "hi " .. myName .. ". Good luck"

local args = {
    [1] = "RolePlayName",
    [2] = finalRP
}


local re = ReplicatedStorage:WaitForChild("RE"):WaitForChild("1RPNam1eTex1t")
re:FireServer(unpack(args))
