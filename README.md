local keys = {
    "SPLASH-kjfasiohfioadssvxcl",
    "SPLASH-dsaohdioascxzc",
    "SPLASH-dsalkdassdx",
    "SPLASH-DADI5-DAJ78",
    "dfsfdsf-dsfssd-dsfds",
	"SPLASH-DSASD-DSADAS"
}

local counter = 1
local keyCheck
for i,v in pairs(keys) do
    if counter == #keys then
    --not whitelisted!
    keys = ""
    game.Players.LocalPlayer:Kick("Not a valid key!")
    else
        if v == _G.Key then
            keyCheck = _G.Key
            keys = ""
        else
            counter = counter +1
        end
    end
end

local HWID = {
    "HWID",
    "HWID2",
    "HWID3",
    "E7504505-847A-491C-977A-61D395393DCF",
    "D9B717FE-E850-4A70-92B3-E90B752D7BAA"
 }
 
 local Old = game:GetService("RbxAnalyticsService"):GetClientId()
 
 if game:GetService("RbxAnalyticsService"):GetClientId() ~= Old then
     while true do end
 end
 if HWID[table.find(HWID, Old)] == Old then
 print("Whitelist")
 --scripthub
 else
     setclipboard("HWID : "..tostring(Old))
     game.Players.LocalPlayer:Kick("Wrong Hwid Dm Admin!")
 end
