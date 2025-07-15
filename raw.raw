-- Load Kavo UI Library (Movable version)
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/ZeianRussell/Kavo-UI-Library/main/Movable.source.lua"))()
local Window = Library.CreateLib("Key system", "Ocean")

-- Create a new tab and section for key input
local Tab = Window:NewTab("Get key")
local Section = Tab:NewSection("Get your key here")

-- Key format validation function (e.g., FREE_XXXXXXXX... with 24 alphanumeric characters)
local function isValidKeyFormat(key)
    return string.match(key, "Pancake") ~= nil
end

-- TextBox to enter the key
Section:NewTextBox("Enter your key", "Paste the key here", function(txt)
    if isValidKeyFormat(txt) then
        print("✅ Correct Key!")

        -- Grant access to the main script
        getgenv().KeyAccessGranted = true
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/6ac2f28ea94f854c1315df954e90445b.lua"))()
    else
        print("❌ Wrong key.")
    end
end)

-- Button to copy the key link
Section:NewButton("Copy key", "Copies link to get your key", function()
    setclipboard("https://linkunlocker.com/pancakes-waver-keysystem-e8UqG")
    print("🔗 Copied With Success.")
end)
