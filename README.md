while true do
    for i = 1, 10 do
        local args = { i }

        game:GetService("ReplicatedStorage")
            :WaitForChild("Packages")
            :WaitForChild("Net")
            :WaitForChild("RE/PlotService/ClaimCoins")
            :FireServer(unpack(args))
        
        wait(0.1) -- Pequeno intervalo entre cada ponto
    end

    wait(1) -- Espera 1 segundo antes de repetir tudo
end
