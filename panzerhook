local Network = require(game:GetService("ReplicatedStorage").Library.Client.Network)
local Fire, Invoke, Fired,Invoked = Network.Fire, Network.Invoke, Network.Fired, Network.Invoked
local old
old = hookfunction(getupvalue(Fire, 1), function(...)
    return true
end)

local playmod = require(game:GetService("ReplicatedStorage").Library.Audio)
oldplay = hookfunction(playmod.Play, function(...)
    return {["RollOffMinDistance"] = 0}
end)
