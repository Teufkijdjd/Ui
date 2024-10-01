_G.Color = Color3.fromRGB(0, 0, 255) -- Color UI
_G.Logo = 13990972098 -- ID Logo Your Hub

local normal = loadstring(game:HttpGet(('https://raw.githubusercontent.com/Lucifer4381/ui-normal-hub/main/scr')))()

local Win = library:Evil("Evo hub","by 999",_G.Logo )

local Tab = Win:CraftTab('Main') -- Name

local Page = Tab:CraftPage('Main',1) -- Name,1 or 2

Page:Button('Button',function() --Name
    print("t")
end)

Page:Toggle('Test',nil,function(a) -- Toggle,Def,callback
    print(a)
end)

Page:Dropdown("Dropdown",{"1","2"},{""},function(v)
    print(v)
end)

Page:MultiDropdown("MultiDropdown",{"MultiDropdown","MultiDropdown2"},{""},function(v)
    print(v)
end)

local A = Page:Label('Label') --name
local B = Page:LabelLog('Label') --name

A:Refresh("A") -- name
B:Refresh("B") -- name
B:Color(Color3.fromRGB(255, 255, 255))  -- Color

Page:Slider("Slider",true,0,100,1,function(value)
    print(value)
end)

Page:Textbox("Test","",function(v)
	print(v)
end)
