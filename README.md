loadstring(game:HttpGet("https://raw.githubusercontent.com/veryskilledperson/anti/main/anticheats", true))()--AntiKicks
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/Rain-Design/Libraries/main/Revenant.lua", true))()
local Flags = Library.Flags

--=Library.DefaultColor = Color3.fromRGB(61, 133, 432)

local Window = Library:Window({
    Text = "Main"
})

local Window2 = Library:Window({
    Text = "Extra"
})

local Window3 = Library:Window({
    Text = "Settings"
})


Window3:Button({
    Text = "Info",
    Callback = function(bool)
        Library:Notification({
            Text = "Welcome To G3 Lite",
            Duration = 5
        })
    end
})



Window:Button({
    Text = "Kill Others",
    Callback = function()
        loadstring(game:HttpGet(('https://pastebin.com/raw/cZDNDGT4'),true))()--kill others
    end
})

Window:Button({
    Text = "Kill High Timers",
    Callback = function()
            loadstring(game:HttpGet(('https://pastebin.com/raw/kyaUbzg5'),true))()--kill high timers
    end
})
Window:Button({
    Text = "TPaura",
    Callback = function()
        loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/G-3-24/tpaura/main/aura"))()--tpaura
    end
})

Window2:Button({
    Text = "AutoClicker",
    Callback = function()
        loadstring(game:HttpGet(('https://raw.githubusercontent.com/veryskilledperson/combined/main/Autonotifi'),true))()--auto optinos
    end
})
Window:Button({
    Text = "Speed",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/veryskilledperson/speed1/main/fly", true))()--speedfly
    end
})
Window:Button({
    Text = "Reach",
    Callback = function()   
        loadstring(game:HttpGet(('https://raw.githubusercontent.com/veryskilledperson/reachui/main/reachUI'),true))()--reach ui
    end
})

Window2:Button({
    Text = "Detector",
    Callback = function()
        loadstring(game:HttpGet(('https://raw.githubusercontent.com/veryskilledperson/newadmins/main/admin%20ui9'),true))()--admin detec ui
    end
})
Window2:Button({
    Text = "Server Hop",
    Callback = function()
        loadstring(game:HttpGet(('https://raw.githubusercontent.com/veryskilledperson/server/main/hop'),true))()--serverhoop
    end
})
Window2:Button({
    Text = "AntiKick",
    Callback = function()
        loadstring(game:HttpGet(('https://raw.githubusercontent.com/veryskilledperson/master/main/README.md'),true))()--antickick
    end
})
Window2:Button({
    Text = "Toxic",
    Callback = function()
        loadstring(game:HttpGet(('https://raw.githubusercontent.com/veryskilledperson/master/main/toxic'),true))()--toxic
    end
})
Window3:Keybind({
    Text = "Toggle Library",
    Default = Enum.KeyCode.RightControl,
    Callback = function()
        Library:Toggle()
    end
})
