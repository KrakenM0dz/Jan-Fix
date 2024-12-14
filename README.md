getgenv().scripttitle = "Name"
getgenv().FolderName = "Folder Name"
--New UI:
loadstring(game:HttpGet('https://raw.githubusercontent.com/Awakenchan/jan/main/JanModifiedSource'))()

--New Tab:
local Tab = library:AddTab("Tab"); 

--New Column: Creates a new side to put stuff on (2 max on a tab)
local Column = Tab:AddColumn();

--New Section:
local Section = Column:AddSection("Aim Assist")

--New Divider:
Section:AddDivider("Main");

--New Button:
Section:AddButton({text = "Button", flag = "Button",  callback = function()

end});

--New Toggle:
Section:AddToggle({text = "Toggle", flag = "Toggle", callback = function(value)

end, state = false})

--New Slider:
Section:AddSlider{text = "Slider", flag = "Slider", min = 0, max = 100, value = 100, suffix = "%", callback =  function(value)

end}

--New Dropdown:
Section:AddList({text = "Dropdown", flag = "Dropdown", value = "Head", values = {"Head", "Torso"}, callback =  function(value)

end});

--New TextBox:
Section:AddBox({text = "TextBox", flag = "TextBox", callback = function(value)

end});

--New KeyBind:
Section:AddBind({text = "Keybind", flag = "Keybind", nomouse = false, key = "End", callback = function()

end});

--New ColorPicker:
Section:AddColor({text = "ColorPicker", flag = "ColorPicker", color = Color3.new(0, 0, 0), callback = function(value)

end});

--Init:
library:Init();
