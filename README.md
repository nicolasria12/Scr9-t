--carregar biblioteca
local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()

local Window = Fluent:CreateWindow({
    Title = "Arko Hub " .. Fluent.Version,
    TabWidth = 160, Size = UDim2.fromOffset(580, 460), Theme = "Dark"
})

local Tabs = {
    Main = Window:AddTab({ Title = "Scam" }),
    Settings = Window:AddTab({ Title = "Settings", Icon = "settings" })
}
--parágrafos
Tabs.Main:AddParagraph({ Title = "Frezze Trade", Content = "Frezze the trade" })
--botoes
Tabs.Main:AddButton({ Title = "Start Frezze Trade", Callback = function() 
print"Frezze Trade"
end })

Tabs.Main:AddParagraph({ Title = "Start Scam", Content = "Force accept" })

Tabs.Main:AddButton({ Title = "Force accept", Callback = function() 
print"Force accept"
end })
