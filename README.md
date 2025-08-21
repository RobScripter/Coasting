# Coasting UI Library

**Coasting** is a customizable Roblox UI library that provides a modern interface with tabs, sections, and interactive elements. Built using Roblox's built-in services, this library allows developers to easily add polished UIs to their games or scripts.

---

## ✨ Features

- 🎨 **Custom Theme Support** (colors, fonts, easing styles, toggle key)  
- 📑 **Tabs & Sections** for organized UI layouts  
- 🔘 **Buttons** with ripple effects  
- ✅ **Toggles** with smooth animations  
- 📊 **Sliders** with numeric input support  
- 🎨 **Color Pickers** (including rainbow/auto cycle mode)  
- ⬇️ **Dropdown Menus** with refreshable options  
- ⌨️ **Keybinds** with customizable behavior  
- 📋 **Labels** for static or dynamic text  

---

## 🚀 Getting Started

### 1. Load the Library
```lua
local Coasting = loadstring(game:HttpGet("https://raw.githubusercontent.com/RobScripter/Coasting/refs/heads/main/Source"))()
```

### 2. Create a Tab
```lua
local tab = Coasting:CreateTab("TabName")
```

### 3. Create a section within the tab
```lua
local section = tab:CreateSection("SectionName")
```

### 4. Add a Label
```lua
local label = section:CreateLabel("NameLabel", "ContentsDisplayed")
```

### 5. Add a Button
```lua
section:CreateButton("NameButton", function()
    print("button pressed")
end)
```

### 6. Add a Toggle (On/Off switch)
```lua
local toggle = section:CreateToggle("ToggleName", function()
    -- toggled = true/false
end)
```

### 7. Add a Slider (integer or decimal, set preciseValue to true for decimal)
```lua
local slider = section:CreateSlider("Volume", 0, 100, 25, false, function()
    print("Slider value:", value)
end)
-- Change value from script
slider:SetSliderValue(50) 
```

### 8. Color Picker
```lua
section:CreateColorPicker("Pick a Color", Color3.fromRGB(0, 255, 0), function()
    print("Selected color:", color)
end)
```

### 9. Add a Dropdown menu
```lua
dropdown:Refresh({"New 1", "New 2"}, 1, function()
    print("Dropdown refreshed selected:", newVal)
end)
```

### 10. Add a Keybind (keyboard or mouse)
```lua
section:CreateKeybind("MyKeybind", Enum.KeyCode.F, false, false, function()
    print("Keybind triggered!")
end
```






