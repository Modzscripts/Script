# Script
Script by Andrômeda scripts


local Library = loadstring(game:HttpGet("https://pastebin.com/raw/vff1bQ9F"))()

local Window = Library.CreateLib("Darkmoon X V1", "Synapse")

-- Tabs

local Tab1 = Window:NewTab("Menu")

local Tab2 = Window:NewTab("Game")

local Tab1Section = Tab1:NewSection("Player")

local Tab2Section = Tab1:NewSection("Auto Farm:")

-- Itens

Tab1Section:NewButton("Pulos Infinitos", "ativar pulos infinitos", function()

    local InfiniteJumpEnabled = true

game:GetService("UserInputService").JumpRequest:connect(function()

	if InfiniteJumpEnabled then
   if infinite
		game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")

	end

end)

end)

Tab1Section:NewToggle("Fov", "Mudar Fov", function(state)

    if state then

        game.Workspace.CurrentCamera.FieldOfView = 120

    else

        game.Workspace.CurrentCamera.FieldOfView = 80

    end

end)

Tab1Section:NewSlider("Velocidade", "Player Speed", 1000, 1, function(v)

    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = v

end)

Tab1Section:NewSlider("força do pulo", "Player Jump", 1000, 1, function(a)

    game.Players.LocalPlayer.Character.Humanoid.JumpPower = a

end)
