for i=14,1,-1 do
  Network = require(game.ReplicatedStorage.Modules.Network)
  local Player = game:GetService("Players").LocalPlayer
  local Wipe = {
      ["config"] = "slots",
      ["wipe_slot"] = "Slot"..i
  }
Network.connect("MenuOptions", "FireServer", Player.Character, Wipe)
end
