local TeleportService = game:GetService("TeleportService")
local Players = game:GetService("Players")

-- ID do lugar para onde os jogadores serão teletransportados
local 130111483311364 = 123456789 -- Substitua pelo seu próprio ID de lugar

-- Função para teletransportar todos os jogadores
local function teleportAllPlayers()
    local players = Players:GetPlayers()
    for _, player in ipairs(players) do
        TeleportService:Teleport(TARGET_PLACE_ID, player)
    end
end

-- Chame a função para teletransportar todos os jogadores
teleportAllPlayers()
