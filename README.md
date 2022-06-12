if game.PlaceId == 8540346411 then
    local BooHub = loadstring(game:HttpGet("https://raw.githubusercontent.com/zachisfunny/BooHub/main/Boo"))()
    local UI = BooHub.Load({
         Title = "👻 Boo Hub" ,
         Style = 0,
         SizeX = 260,
         SizeY = 260,
         Theme = "Dark"
    })
    local Page = UI.New({
        Title = "Main"
    })
    local Page2 = UI.New({
        Title = "Farm"
    }) local Page3 = UI.New({
        Title = "Rebirths"
    })
    local Page4 = UI.New({
        Title = "Upgrades"
    })
    Page.Label({
    Text = "Made by zach.#6257"
})
    Page.Slider({
        Text = "Walk Speed",
        Callback = function(value)
             game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value
        end,
        Min = 16,
        Max = 100,
        Def = 0
    })
    Page2.Toggle({
        Text = "Auto Click",
        Callback = function(value)
            getgenv().Click = value
        while wait() do
           if not getgenv().Click then break end
    
    
    game:GetService("ReplicatedStorage").Events.Click3:FireServer()
    
             
    wait()
        end 
        end,
        Enabled = false
    })
    
        Page.Toggle({
        Text = "Anti-AFK",
        Callback = function(value)
            getgenv().anti = value
        while wait() do
           if not getgenv().anti then break end
wait(3)
local VirtualUser=game:service'VirtualUser'
game:service('Players').LocalPlayer.Idled:connect(function()
VirtualUser:CaptureController()
VirtualUser:ClickButton2(Vector2.new())
end)
        end 
        end,
        Enabled = false
    })
    Page3.Toggle({
        Text = "Auto Rebirth 1",
        Callback = function(value)
    
            getgenv().Rebirth1 = value
        while wait() do
           if not getgenv().Rebirth1 then break end
    local args = {
        [1] = 1
    }
    game:GetService("ReplicatedStorage").Events.Rebirth:FireServer(unpack(args))
               wait()
            end 
        
       end,
        Enabled = false
    })
    Page3.Toggle({
        Text = "Auto Rebirth 5",
        Callback = function(value)
    
            getgenv().Rebirth2 = value
        while wait() do
           if not getgenv().Rebirth2 then break end
    local args = {
        [1] = 2
    }
    
    game:GetService("ReplicatedStorage").Events.Rebirth:FireServer(unpack(args))
    
               wait()
            end 
        
       end,
        Enabled = false
    })
    Page3.Toggle({
        Text = "Auto Rebirth 10",
        Callback = function(value)
    
            getgenv().Rebirth3 = value
        while wait() do
           if not getgenv().Rebirth3 then break end
    local args = {
        [1] = 3
    }
    
    game:GetService("ReplicatedStorage").Events.Rebirth:FireServer(unpack(args))
    
               wait()
            end 
        
       end,
        Enabled = false
    })
    Page3.Toggle({
        Text = "Auto Rebirth 25",
        Callback = function(value)
    
            getgenv().Rebirth4 = value
        while wait() do
           if not getgenv().Rebirth4 then break end
    local args = {
        [1] = 4
    }
    
    game:GetService("ReplicatedStorage").Events.Rebirth:FireServer(unpack(args))
    
               wait()
            end 
        
       end,
        Enabled = false
    })
    Page3.Toggle({
        Text = "Auto Rebirth 100",
        Callback = function(value)
    
            getgenv().Rebirth5 = value
        while wait() do
           if not getgenv().Rebirth5 then break end
    local args = {
        [1] = 5
    }
    
    game:GetService("ReplicatedStorage").Events.Rebirth:FireServer(unpack(args))
    
               wait()
            end 
        
       end,
        Enabled = false
    })
    Page3.Toggle({
        Text = "Auto Rebirth 500",
        Callback = function(value)
    
            getgenv().Rebirth6 = value
        while wait() do
           if not getgenv().Rebirth6 then break end
    local args = {
        [1] = 6
    }
    
    game:GetService("ReplicatedStorage").Events.Rebirth:FireServer(unpack(args))
    
               wait()
            end 
        
       end,
        Enabled = false
    })
    Page3.Toggle({
        Text = "Auto Rebirth 2.5k",
        Callback = function(value)
    
            getgenv().Rebirth7 = value
        while wait() do
           if not getgenv().Rebirth7 then break end
    local args = {
        [1] = 7
    }
    
    game:GetService("ReplicatedStorage").Events.Rebirth:FireServer(unpack(args))
    
               wait()
            end 
        
       end,
        Enabled = false
    })
    Page3.Toggle({
        Text = "Auto Rebirth 5k",
        Callback = function(value)
    
            getgenv().Rebirth8 = value
        while wait() do
           if not getgenv().Rebirth8 then break end
    local args = {
        [1] = 8
    }
    
    game:GetService("ReplicatedStorage").Events.Rebirth:FireServer(unpack(args))
    
               wait()
            end 
        
       end,
        Enabled = false
    })
    Page4.Toggle({
        Text = "Auto all Upgrades",
        Callback = function(value)
    
            getgenv().Upgrade = value
        while wait() do
           if not getgenv().Upgrade then break end
    game:GetService("ReplicatedStorage").Functions.Upgrade:InvokeServer("GemsMultiplier")
    game:GetService("ReplicatedStorage").Functions.Upgrade:InvokeServer("WalkSpeed")
    game:GetService("ReplicatedStorage").Functions.Upgrade:InvokeServer("ClickMultiplier")
    game:GetService("ReplicatedStorage").Functions.Upgrade:InvokeServer("RebirthButtons")
    game:GetService("ReplicatedStorage").Functions.Upgrade:InvokeServer("LuckMultiplier")
    
               wait()
            end 
        
       end,
        Enabled = false
    })
