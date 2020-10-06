--[[ // CREDITS \\

    YESOK FOR DEVELOPMENT
https://v3rmillion.net/member.php?action=profile&uid=514695

    JAN FOR ESP
https://v3rmillion.net/member.php?action=profile&uid=557102

    CRISHOUX FOR STRUCID/NERF-FPS FUNCTIONS
https://v3rmillion.net/member.php?action=profile&uid=490270
--]]

warn("Loading...")

local Players = game:GetService("Players")
local UserInput = game:GetService("UserInputService")
local HTTP = game:GetService("HttpService")
local RunServ = game:GetService("RunService")
local CoreGui = game:GetService("CoreGui")

local ScreenGui = Instance.new("ScreenGui")
local Main = Instance.new("Frame")
local SelectLabel = Instance.new("TextLabel")
local CreditsLabel = Instance.new("TextLabel")
local RunButton = Instance.new("ImageButton")
local TextLabel = Instance.new("TextLabel")
local Border = Instance.new("Frame")
local Exit = Instance.new("ImageButton")
local SaveLabel = Instance.new("TextLabel")
local SaveButton = Instance.new("ImageButton")
local Droppable = Instance.new("Frame")
local TextButton = Instance.new("TextButton")
local Selected = Instance.new("TextLabel")
local DropDown = Instance.new("Frame")
local UIListLayout = Instance.new("UIListLayout")
local FindPartOnRay = Instance.new("TextButton")
local FindPartOnRayWithIgnoreList = Instance.new("TextButton")
local FindPartOnRayWithWhitelist = Instance.new("TextButton")
local ScreenPointToRay = Instance.new("TextButton")

local PlaceId = game.PlaceId
local LocalPlayer = Players.LocalPlayer
local CharacterAdded
local Camera = workspace.CurrentCamera
local PlayerGui = LocalPlayer:WaitForChild("PlayerGui")
PlayerGui:SetTopbarTransparency(1)
local Mouse = LocalPlayer:GetMouse()

ScreenGui.Parent = CoreGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
ScreenGui.DisplayOrder = 2147483647
ScreenGui.ResetOnSpawn = false

Main.Name = "Main"
Main.Parent = ScreenGui
Main.Active = true
Main.Draggable = true
Main.BackgroundColor3 = Color3.new(0.117647, 0.117647, 0.117647)
Main.BorderColor3 = Color3.new(1, 1, 1)
Main.Position = UDim2.new(0.40231362, 0, 0.41626215, 0)
Main.Size = UDim2.new(0, 304, 0, 137)

SelectLabel.Name = "SelectLabel"
SelectLabel.Parent = Main
SelectLabel.BackgroundColor3 = Color3.new(1, 1, 1)
SelectLabel.BackgroundTransparency = 1
SelectLabel.Position = UDim2.new(0.128999993, 0, 0.129999995, 0)
SelectLabel.Size = UDim2.new(0, 224, 0, 20)
SelectLabel.Font = Enum.Font.Code
SelectLabel.Text = "Please Select Your Ray Method."
SelectLabel.TextColor3 = Color3.new(1, 1, 1)
SelectLabel.TextSize = 14

CreditsLabel.Name = "CreditsLabel"
CreditsLabel.Parent = Main
CreditsLabel.BackgroundColor3 = Color3.new(1, 1, 1)
CreditsLabel.BackgroundTransparency = 1
CreditsLabel.Position = UDim2.new(0.428000088, 0, 0.893000005, 0)
CreditsLabel.Size = UDim2.new(0, 43, 0, 15)
CreditsLabel.Font = Enum.Font.Gotham
CreditsLabel.Text = "Celestial Silent Aim | yesok#3877"
CreditsLabel.TextColor3 = Color3.new(0.576471, 0.576471, 0.576471)
CreditsLabel.TextSize = 10

RunButton.Name = "RunButton"
RunButton.Parent = Main
RunButton.BackgroundTransparency = 1
RunButton.BorderSizePixel = 0
RunButton.Position = UDim2.new(0.300898075, 0, 0.730581724, 0)
RunButton.Size = UDim2.new(0, 118, 0, 19)
RunButton.Image = "rbxassetid://1307995459"
RunButton.ImageColor3 = Color3.new(0.505882, 0, 0)
RunButton.ScaleType = Enum.ScaleType.Slice
RunButton.SliceCenter = Rect.new(2, 2, 254, 254)

TextLabel.Parent = RunButton
TextLabel.AnchorPoint = Vector2.new(0, 0.5)
TextLabel.BackgroundTransparency = 1
TextLabel.Position = UDim2.new(0, 0, 0.491569102, 0)
TextLabel.Size = UDim2.new(1, 0, 1, 0)
TextLabel.Font = Enum.Font.Code
TextLabel.Text = "Submit"
TextLabel.TextColor3 = Color3.new(1, 1, 1)
TextLabel.TextSize = 14

Border.Name = "Border"
Border.Parent = Main
Border.BackgroundColor3 = Color3.new(0.505882, 0, 0)
Border.BorderSizePixel = 0
Border.Position = UDim2.new(0, 0, 0.00100000005, 0)
Border.Size = UDim2.new(0, 304, 0, 15)

Exit.Name = "Exit"
Exit.Parent = Border
Exit.BackgroundTransparency = 1
Exit.Position = UDim2.new(0.950657904, 0, 0, 0)
Exit.Size = UDim2.new(0, 15, 0, 15)
Exit.ZIndex = 2
Exit.Image = "rbxassetid://3926305904"
Exit.ImageRectOffset = Vector2.new(924, 724)
Exit.ImageRectSize = Vector2.new(36, 36)

SaveLabel.Name = "SaveLabel"
SaveLabel.Parent = Main
SaveLabel.AnchorPoint = Vector2.new(0, 0.5)
SaveLabel.BackgroundTransparency = 1
SaveLabel.Position = UDim2.new(0.299342096, 0, 0.584513516, 0)
SaveLabel.Size = UDim2.new(0.276315778, 0, 0.145235598, 0)
SaveLabel.Font = Enum.Font.Code
SaveLabel.Text = "Save Method"
SaveLabel.TextColor3 = Color3.new(1, 1, 1)
SaveLabel.TextSize = 14

SaveButton.Name = "SaveButton"
SaveButton.Parent = SaveLabel
SaveButton.BackgroundColor3 = Color3.new(0.505882, 0, 0)
SaveButton.BorderColor3 = Color3.new(1, 1, 1)
SaveButton.Position = UDim2.new(1.17900002, 0, 0.100000001, 0)
SaveButton.Size = UDim2.new(0, 19, 0, 19)
SaveButton.ZIndex = 2
SaveButton.ImageRectOffset = Vector2.new(644, 204)
SaveButton.ImageRectSize = Vector2.new(36, 36)

Droppable.Name = "Droppable"
Droppable.Parent = Main
Droppable.BackgroundColor3 = Color3.new(0.164706, 0.164706, 0.164706)
Droppable.BorderColor3 = Color3.new(1, 1, 1)
Droppable.ClipsDescendants = true
Droppable.Position = UDim2.new(0.178434879, 0, 0.324888349, 0)
Droppable.Size = UDim2.new(0, 192, 0, 17)

TextButton.Parent = Droppable
TextButton.BackgroundColor3 = Color3.new(0.164706, 0.164706, 0.164706)
TextButton.BorderColor3 = Color3.new(1, 1, 1)
TextButton.BorderSizePixel = 0
TextButton.Position = UDim2.new(0.00649298262, 0, -0.000401826575, 0)
TextButton.Size = UDim2.new(0, 190, 0, 17)
TextButton.AutoButtonColor = false
TextButton.Font = Enum.Font.Code
TextButton.Text = "v "
TextButton.TextColor3 = Color3.new(1, 1, 1)
TextButton.TextSize = 14
TextButton.TextXAlignment = Enum.TextXAlignment.Right

Selected.Name = "Selected"
Selected.Parent = TextButton
Selected.BackgroundColor3 = Color3.new(0.164706, 0.164706, 0.164706)
Selected.BorderSizePixel = 0
Selected.Position = UDim2.new(-0.000142950754, 0, 0.144445077, 0)
Selected.Size = UDim2.new(0, 175, 0, 14)
Selected.Font = Enum.Font.Code
Selected.Text = "FindPartOnRayWithIgnoreList"
Selected.TextColor3 = Color3.new(0.654902, 0.654902, 0.654902)
Selected.TextSize = 11
Selected.TextWrapped = true

DropDown.Name = "DropDown"
DropDown.Parent = TextButton
DropDown.BackgroundColor3 = Color3.new(0.164706, 0.164706, 0.164706)
DropDown.BorderColor3 = Color3.new(0.227451, 0.227451, 0.227451)
DropDown.Position = UDim2.new(0, 0, 1.35294116, 0)
DropDown.Size = UDim2.new(0, 190, 0, 77)

UIListLayout.Parent = DropDown
UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder

FindPartOnRay.Name = "FindPartOnRay"
FindPartOnRay.Parent = DropDown
FindPartOnRay.BackgroundColor3 = Color3.new(0.164706, 0.164706, 0.164706)
FindPartOnRay.BorderSizePixel = 0
FindPartOnRay.Size = UDim2.new(0, 190, 0, 18)
FindPartOnRay.Font = Enum.Font.Code
FindPartOnRay.Text = "FindPartOnRay"
FindPartOnRay.TextColor3 = Color3.new(0.654902, 0.654902, 0.654902)
FindPartOnRay.TextSize = 12

FindPartOnRayWithIgnoreList.Name = "FindPartOnRayWithIgnoreList"
FindPartOnRayWithIgnoreList.Parent = DropDown
FindPartOnRayWithIgnoreList.BackgroundColor3 = Color3.new(0.164706, 0.164706, 0.164706)
FindPartOnRayWithIgnoreList.BorderSizePixel = 0
FindPartOnRayWithIgnoreList.Size = UDim2.new(0, 190, 0, 18)
FindPartOnRayWithIgnoreList.Font = Enum.Font.Code
FindPartOnRayWithIgnoreList.Text = "FindPartOnRayWithIgnoreList"
FindPartOnRayWithIgnoreList.TextColor3 = Color3.new(0.654902, 0.654902, 0.654902)
FindPartOnRayWithIgnoreList.TextSize = 12

FindPartOnRayWithWhitelist.Name = "FindPartOnRayWithWhitelist"
FindPartOnRayWithWhitelist.Parent = DropDown
FindPartOnRayWithWhitelist.BackgroundColor3 = Color3.new(0.164706, 0.164706, 0.164706)
FindPartOnRayWithWhitelist.BorderSizePixel = 0
FindPartOnRayWithWhitelist.Size = UDim2.new(0, 190, 0, 18)
FindPartOnRayWithWhitelist.Font = Enum.Font.Code
FindPartOnRayWithWhitelist.Text = "FindPartOnRayWithWhitelist"
FindPartOnRayWithWhitelist.TextColor3 = Color3.new(0.654902, 0.654902, 0.654902)
FindPartOnRayWithWhitelist.TextSize = 12

local File = "RayMethod-DataSave.lua"
if not 
    pcall(function() 
        readfile(File) 
    end) 
then
    writefile(File, HTTP:JSONEncode({RayMethodSelected = 'FindPartOnRayWithIgnoreList', SaveRayMethod = false}))
end

Selected.Text = HTTP:JSONDecode(readfile(File)).RayMethodSelected
if HTTP:JSONDecode(readfile(File)).SaveRayMethod then
    getgenv().Save = true
    SaveButton.Image = "rbxassetid://3926305904"
else
    getgenv().Save = false
    SaveButton.Image = ""
end

Exit.MouseButton1Click:Connect(function()
    ScreenGui:Destroy()
end)

getgenv().Open = false
TextButton.MouseButton1Click:Connect(function()
    if getgenv().Open then
        Droppable.Size = UDim2.new(0, 192, 0, 81)
        TextButton.Text = "< "
        getgenv().Open = false
    else
        Droppable.Size = UDim2.new(0, 192, 0, 17)
        TextButton.Text = "v "
        getgenv().Open = true
    end
end)

function selectRay(selectedMethod)
    selectedMethod.MouseButton1Click:Connect(function()
        Selected.Text = selectedMethod.Text
        Droppable.Size = UDim2.new(0, 192, 0, 17)
        TextButton.Text = "v "
        getgenv().Open = true
    end)
end

selectRay(FindPartOnRay)
selectRay(FindPartOnRayWithIgnoreList)
selectRay(FindPartOnRayWithWhitelist)

SaveButton.MouseButton1Click:Connect(function()
    if SaveButton.Image == "" then
        getgenv().Save = true
        SaveButton.Image = "rbxassetid://3926305904"
    else
        getgenv().Save = false
        SaveButton.Image = ""
    end
end)

getgenv().Loaded = false
RunButton.MouseButton1Click:Connect(function()
    getgenv().RayMethodSelected = Selected.Text
    if getgenv().Save then
        writefile(File,HTTP:JSONEncode({RayMethodSelected = Selected.Text, SaveRayMethod = true}))
    else
        writefile(File,HTTP:JSONEncode({RayMethodSelected = 'FindPartOnRayWithIgnoreList', SaveRayMethod = false}))
    end
    getgenv().Loaded = true
    ScreenGui:Destroy()
    print("Ray Method: " .. getgenv().RayMethodSelected)
end)


local rigType = string.split(tostring(LocalPlayer.Character:WaitForChild("Humanoid").RigType), ".")[3]
local selected_teamType = "Regular"
local selected_rigType

local rigTypeR6 = {
	["Head"] = true,
	["Torso"] = true,
	["LowerTorso"] = true,
	["Left Arm"] = true,
	["Right Arm"] = true,
	["Left Leg"] = true,
	["Right Leg"] = true
}

local rigTypeR15 = {
    ["Head"] = true,
    ["UpperTorso"] = true,
    ["LowerTorso"] = true,
    ["LeftUpperArm"] = true,
    ["RightUpperArm"] = true,
    ["RightLowerArm"] = true,
    ["LeftLowerArm"] = true,
    ["LeftHand"] = true,
    ["RightHand"] = true,
    ["LeftUpperLeg"] = true,
    ["RightUpperLeg"] = true,
    ["LeftLowerLeg"] = true,
    ["RightLowerLeg"] = true,
    ["LeftFoot"] = true,
    ["RightFoot"] = true
}

local rigTypeStrucid = {
    ["LeftLowerArm"] = true,
    ["RightLowerArm"] = true,
    ["Head"] = true,
    ["LeftUpperLeg"] = true,
    ["LeftUpperLeg"] = true,
    ["RightLowerLeg"] = true,
    ["Neck"] = true,
    ["RightFoot"] = true,
    ["UpperTorso"] = true,
    ["LeftLowerLeg"] = true,
    ["LowerTorso"] = true,
    ["RightUpperLeg"] = true,
    ["LeftUpperArm"] = true,
    ["RightUpperArm"] = true
}

local rigTypeAceOfSpadez = {
	["Head"] = true,
	["LeftFoot"] = true,
	["LowerLeftArm"] = true,
	["LowerLeftLeg"] = true,
	["LowerRightArm"] = true,
	["LowerRightLeg"] = true,
	["LowerTorso"] = true,
	["RightFoot"] = true,
	["MidTorso"] = true,
	["UpperLeftArm"] = true,
	["UpperLeftLeg"] = true,
	["UpperRightArm"] = true,
	["UpperRightLeg"] = true,
	["UpperTorso"] = true,
	["LeftHandle"] = true,
	["RightHandle"] = true,
	["Shoulders"] = true,
	["Torso"] = true
}

local rigTypeStandardIssue = {
	["lowerrightleg"] = true,
	["leftforearm"] = true,
	["lowerleftleg"] = true,
	["waist"] = true,
	["Torso"] = true,
	["rightforearm"] = true,
	["Head"] = true,
}

local rigTypeRecoil = {
    ["Head"] = true,
	["LeftFoot"] = true,
	["RightFoot"] = true,
	["LeftLowerLeg"] = true,
	["LeftUpperLeg"] = true,
	["RightLowerLeg"] = true,
	["RightUpperLeg"] = true,
	["UpperTorso"] = true,
	["LowerTorso"] = true,
	["LeftUpperArm"] = true,
	["RightUpperArm"] = true,
	["LeftLowerArm"] = true,
	["RightLowerArm"] = true,
	["RightHand"] = true,
	["LeftHand"] = true
}

local rigTypePloyguns = {
    ["Head"] = true,
	["Right Forearm"] = true,
	["Right Leg"] = true,
	["Right Foreleg"] = true,
	["Left Arm"] = true,
	["Right Hand"] = true,
	["Right Foot"] = true,
	["Right Arm"] = true,
	["Left Hand"] = true,
	["Left Foreleg"] = true,
	["Left Leg"] = true,
	["Hips"] = true,
	["Torso"] = true,
	["Left Foot"] = true,
	["Mid"] = true
}

local rigTypeKineticCode = {
    ["UpperTorso"] = true,
	["Head"] = true,
	["Hips"] = true,
	["LeftArm"] = true,
	["LeftFoot"] = true,
    ["LeftHip"] = true,
    ["LeftKnuckles"] = true,
    ["LeftLeg"] = true,
    ["LeftPalm"] = true,
    ["LeftShoulder"] = true,
    ["LowerTorso"] = true,
    ["Neck"] = true,
    ["RightArm"] = true,
    ["RightFoot"] = true,
    ["RightHip"] = true,
    ["RightKnuckles"] = true,
    ["RightLeg"] = true,
    ["RightPalm"] = true,
    ["RightShoulder"] = true
}

if PlaceId == 2377868063 then
    selected_rigType = rigTypeStrucid
elseif PlaceId == 2555870920 then
    selected_rigType = rigTypeAceOfSpadez
elseif PlaceId == 388599755 then
    selected_rigType = rigTypePloyguns
elseif PlaceId == 1837257681 then
    selected_rigType = rigTypeStandardIssue
elseif PlaceId == 4651779470 then
    selected_rigType = rigTypeRecoil
    selected_teamType = "Recoil"
elseif PlaceId == 4738545896 then
    selected_rigType = rigTypeR15
    selected_teamType = "ShootOut"
elseif PlaceId == 3210442546 then
    selected_rigType = rigTypeR15
    selected_teamType = "IslandRoyale"
elseif PlaceId == 401356052 then
    selected_rigType = rigTypeKineticCode
elseif PlaceId == 983224898 then
    selected_teamType = "WildRevolvers"
    selected_rigType = rigTypeR15
elseif rigType == "R6" then
    selected_rigType = rigTypeR6
elseif rigType == "R15" then
    selected_rigType = rigTypeR15
end

print("Rig Type: " .. rigType)
print("Team Type: " .. selected_teamType)

local function teamType(player)
    if selected_teamType == "Recoil" then
        return player:FindFirstChild("GameStats").Team.Value
    elseif selected_teamType == "ShootOut" then
        if player == LocalPlayer then
            return tostring(BrickColor.new(0.172549, 0.329412, 1))
        else
            for _, Player in next, Players:GetPlayers() do
                if Player.Character then
                    if Player.Character:FindFirstChild("Head") then
                        if Player.Character == player.Character then
                            if Player.Character.Head:FindFirstChild("NameTag") then
                                NameTag = Player.Character.Head.NameTag.TextLabel
                                if string.find(tostring(BrickColor.new(NameTag.TextColor3)), "red") then
                                    return tostring(BrickColor.new(NameTag.TextColor3))
                                elseif string.find(tostring(BrickColor.new(NameTag.TextStrokeColor3)), "blue") then
                                    return tostring(BrickColor.new(NameTag.TextStrokeColor3))
                                end
                            end
                        end
                    end
                end
            end
        end
    elseif selected_teamType == "IslandRoyale" then
        return player:FindFirstChild("TeamName").Value
    elseif selected_teamType == "WildRevolvers" then
        if player == LocalPlayer then
            return tostring(BrickColor.new(0, 255, 0))
        else
            for _, Player in next, game.Players:GetPlayers() do
                if Player.Character then
                    if Player.Character:FindFirstChild("Head") then
                        if Player.Character == player.Character then
                            return tostring(BrickColor.new(Player.Character.Head.HeadTag.Label.TextColor3))
                        end
                    end
                end
            end
        end
    else
        if player.Team or player.TeamColor then
            local teamplayer = player.Team or player.TeamColor
            return teamplayer
        end
    end
end

local function characterType(player)
    playerName = player.Name
    if PlaceId == 401356052 then
        if workspace["Players"][playerName] or workspace["Players"]:WaitForChild(player) then
            local playerCharacter = workspace["Players"][playerName] or workspace["Players"]:WaitForChild(player)
            return playerCharacter
        end
    elseif player.Character or workspace:FindFirstChild(playerName) then
        local playerCharacter = player.Character or workspace:FindFirstChild(playerName)
        return playerCharacter
    end
end

local function FFA()
    sameTeam = 0
    for _, player in next, Players:GetPlayers() do
        if teamType(player) == teamType(LocalPlayer) then
            sameTeam = sameTeam + 1
        end
    end
    if sameTeam == #Players:GetChildren() then
        return true
    else
        return false
    end
end

local function returnVisibility(player)
    if getgenv().VisibiltyCheck then
        if characterType(player) then 
            if player.Character:FindFirstChild(getgenv().SelectedPart) then 
                CastPoint = {LocalPlayer.Character[getgenv().SelectedPart].Position, player.Character[getgenv().SelectedPart].Position}
                IgnoreList = {player.Character, LocalPlayer.Character}
                local castpointparts = workspace.CurrentCamera:GetPartsObscuringTarget(CastPoint, IgnoreList)
                if unpack(castpointparts) then
                    return false
                end
            end
        end
    end
    return true
end

local function returnRay(args, hit)
    if PlaceId == 2377868063 then
        args[3] = {workspace.IgnoreThese, LocalPlayer.Character, workspace.BuildStuff, workspace.Map}
        return args[3]
    elseif PlaceId == 625364452 then
        return hit, hit.Position, Vector3.new(0, 0, 0), hit.Material
    else
        CCF = Camera.CFrame.p
        args[2] = Ray.new(CCF, (hit.Position + Vector3.new(0,(CCF-hit.Position).Magnitude/getgenv().Distance,0) - CCF).unit * (getgenv().Distance * 10))
        return args[2]
    end
end

print("FFA: " .. tostring(FFA()))
print("Visibility Check: " .. tostring(getgenv().VisibiltyCheck))
print("Target ESP: " .. tostring(getgenv().VisibiltyCheck))

local function createBox(player)
	local lines = Instance.new("Frame")
	lines.Name = player.Name
	lines.BackgroundTransparency = 1
	lines.AnchorPoint = Vector2.new(0.5,0.5)
	
	local outlines = Instance.new("Folder", lines)
	outlines.Name = "outlines"
	local inlines = Instance.new("Folder", lines)
	inlines.Name = "inlines"
	
	local outline1 = Instance.new("Frame", outlines)
	outline1.Name = "left"
	outline1.BorderSizePixel = 0
	outline1.BackgroundColor3 = Color3.new(0,0,0)
	outline1.Size = UDim2.new(0,-1,1,0)
	
	local outline2 = Instance.new("Frame", outlines)
	outline2.Name = "right"
	outline2.BorderSizePixel = 0
	outline2.BackgroundColor3 = Color3.new(0,0,0)
	outline2.Position = UDim2.new(1,0,0,0)
	outline2.Size = UDim2.new(0,1,1,0)
	
	local outline3 = Instance.new("Frame", outlines)
	outline3.Name = "up"
	outline3.BorderSizePixel = 0
	outline3.BackgroundColor3 = Color3.new(0,0,0)
	outline3.Size = UDim2.new(1,0,0,-1)
	
	local outline4 = Instance.new("Frame", outlines)
	outline4.Name = "down"
	outline4.BorderSizePixel = 0
	outline4.BackgroundColor3 = Color3.new(0,0,0)
	outline4.Position = UDim2.new(0,0,1,0)
	outline4.Size = UDim2.new(1,0,0,1)
	
	local inline1 = Instance.new("Frame", inlines)
	inline1.Name = "left"
	inline1.BorderSizePixel = 0
	inline1.Size = UDim2.new(0,1,1,0)
	
	local inline2 = Instance.new("Frame", inlines)
	inline2.Name = "right"
	inline2.BorderSizePixel = 0
	inline2.Position = UDim2.new(1,0,0,0)
	inline2.Size = UDim2.new(0,-1,1,0)
	
	local inline3 = Instance.new("Frame", inlines)
	inline3.Name = "up"
	inline3.BorderSizePixel = 0
	inline3.Size = UDim2.new(1,0,0,1)
	
	local inline4 = Instance.new("Frame", inlines)
	inline4.Name = "down"
	inline4.BorderSizePixel = 0
	inline4.Position = UDim2.new(0,0,1,0)
	inline4.Size = UDim2.new(1,0,0,-1)
	
	local text = Instance.new("TextLabel")
	text.Name = "nametag"
	text.Position =  UDim2.new(0.5,0,0,-9)
	text.Size = UDim2.new(0,100,0,-20)
	text.AnchorPoint = Vector2.new(0.5,0.5)
	text.BackgroundTransparency = 1
	text.TextColor3 = Color3.new(1,1,1)
	text.Font = Enum.Font.Code
	text.TextSize = 16
	text.TextStrokeTransparency = 0
	
	for _,v in pairs(inlines:GetChildren()) do
		v.BackgroundColor3 = Color3.fromRGB(255, 74, 74)
	end
	
	return lines
end

local function updateEsp(player, folder)
    RunServ:BindToRenderStep("Get_Target_ESP", 1, function()
        local playerCharacter = characterType(player)
        local xMin = Camera.ViewportSize.X
        local yMin = Camera.ViewportSize.Y
        local xMax = 0
        local yMax = 0
        if returnVisibility(player) and teamType(player) ~= teamType(LocalPlayer) or FFA() and returnVisibility(player) then
            if player ~= LocalPlayer and player == getTarget() and playerCharacter and playerCharacter:FindFirstChild("Humanoid") and playerCharacter.Humanoid.Health > 0 then
                local box = folder
                local _, onScreen = Camera:WorldToScreenPoint(playerCharacter[getgenv().SelectedPart].Position)
                if onScreen and box then
                    box.Visible = true
                    local function getCorners(obj, size)
                        local corners = {
                            Vector3.new(obj.X+size.X/2, obj.Y+size.Y/2, obj.Z+size.Z/2);
                            Vector3.new(obj.X-size.X/2, obj.Y+size.Y/2, obj.Z+size.Z/2);
                            
                            Vector3.new(obj.X-size.X/2, obj.Y-size.Y/2, obj.Z-size.Z/2);
                            Vector3.new(obj.X+size.X/2, obj.Y-size.Y/2, obj.Z-size.Z/2);
                            
                            Vector3.new(obj.X-size.X/2, obj.Y+size.Y/2, obj.Z-size.Z/2);
                            Vector3.new(obj.X+size.X/2, obj.Y+size.Y/2, obj.Z-size.Z/2);
                            
                            Vector3.new(obj.X-size.X/2, obj.Y-size.Y/2, obj.Z+size.Z/2);
                            Vector3.new(obj.X+size.X/2, obj.Y-size.Y/2, obj.Z+size.Z/2);
                        }
                        return corners
                    end
                    local cornerCount = 1
                    local allCorners = {}
                    for _, bodyPart in next, playerCharacter:GetChildren() do
                        if selected_rigType[bodyPart.Name] then
                            local fetchCorners = getCorners(bodyPart.CFrame, bodyPart.Size)
                            for _, corner in next, fetchCorners do
                                table.insert(allCorners, cornerCount, corner)
                                cornerCount = cornerCount + 1
                            end
                        end
                    end
                    for _, corner in next, allCorners do
                        local pos = Camera:WorldToScreenPoint(corner)
                        if pos.X > xMax then
                            xMax = pos.X
                        end
                        if pos.X < xMin then
                            xMin = pos.X
                        end
                        if pos.Y > yMax then
                            yMax = pos.Y
                        end
                        if pos.Y < yMin then
                            yMin = pos.Y
                        end
                    end
                    local xSize = xMax - xMin
                    local ySize = yMax - yMin
                    box.Position = UDim2.new(0,xMin+(Vector2.new(xMax,0)-Vector2.new(xMin,0)).magnitude/2,0,yMin+(Vector2.new(0,yMax)-Vector2.new(0,yMin)).magnitude/2)
                    box.Size = UDim2.new(0,xSize,0,ySize)
                end
            end
        end
    end)
end

spawn(function()
    repeat
        for Hue = 0,1,0.003 do
            getgenv().Rainbow = Color3.fromHSV(Hue,1,1)
            wait()
        end
    until false
end)

spawn(function()
    local Circle = Drawing.new('Circle')
    Circle.Transparency = 1
    Circle.Thickness = 1.5
    Circle.Visible = false
    Circle.Color = Color3.fromRGB(255,0,0)
    Circle.Filled = false
    Circle.Radius = getgenv().FOV

    local TargetText = Drawing.new("Text")
    getgenv().SelectedTarget = ""
    TargetText.Text = ""
    TargetText.Size = 17
    TargetText.Center = true
    TargetText.Visible = false
    TargetText.Color = Color3.fromRGB(255,0,0)
    TargetText.Font = Drawing.Fonts.Monospace

    local lineX = Drawing.new("Line")
    lineX.Transparency = 1
    lineX.Thickness = 1.5
    lineX.Visible = false
    lineX.Color = Color3.fromRGB(255,0,0)

    local lineY = Drawing.new("Line")
    lineX.Transparency = 1
    lineY.Thickness = 1.5
    lineY.Visible = false
    lineY.Color = Color3.fromRGB(255,0,0)

    RunServ:BindToRenderStep("Get_Fov",1,function()
        if getgenv().Loaded then
            local Length = 10
            local Middle = 37
            Circle.Visible = getgenv().CircleVisibility
            TargetText.Visible = getgenv().CircleVisibility
            lineX.Visible = getgenv().CircleVisibility
            lineY.Visible = getgenv().CircleVisibility 
            Circle.Color = getgenv().Rainbow
            lineX.Color = getgenv().Rainbow
            lineY.Color = getgenv().Rainbow
	    Circle.Radius = getgenv().FOV
            Circle.Position = Vector2.new(Mouse.X,Mouse.Y+Middle)
            TargetText.Position = Vector2.new(Mouse.X,Mouse.Y+Middle-180)
            lineX.From = Vector2.new((Mouse.X)+Length+1,Mouse.Y-0.5+Middle)
            lineX.To = Vector2.new(Mouse.X-Length,Mouse.Y-0.5+Middle)
            lineY.From = Vector2.new(Mouse.X,Mouse.Y+Length+Middle)
            lineY.To = Vector2.new(Mouse.X,Mouse.Y-Length+Middle)
            TargetText.Text = getgenv().SelectedTarget
        end
    end)
end)

function getTarget()
	local closestTarg = math.huge
	local Target = nil

	for _, Player in next, Players:GetPlayers() do
        if Player ~= LocalPlayer and returnVisibility(Player) and teamType(Player) ~= teamType(LocalPlayer) or FFA() and Player ~= LocalPlayer and returnVisibility(Player) then
            local playerCharacter = characterType(Player)
            if playerCharacter then
                local playerHumanoid = playerCharacter:FindFirstChild("Humanoid")
                local playerPart = playerCharacter:FindFirstChild(getgenv().SelectedPart)
                if playerPart and playerHumanoid then
                    local hitVector, onScreen = Camera:WorldToScreenPoint(playerPart.Position)
                    if onScreen and playerHumanoid.Health > 0 then
                        local CCF = Camera.CFrame.p
                        if workspace:FindPartOnRayWithIgnoreList(Ray.new(CCF, (playerPart.Position-CCF).unit * getgenv().Distance),{Player}) then
                            local hitTargMagnitude = (Vector2.new(Mouse.X, Mouse.Y) - Vector2.new(hitVector.X, hitVector.Y)).magnitude
                            if hitTargMagnitude < closestTarg and hitTargMagnitude <= getgenv().FOV then
                                Target = Player
                                closestTarg = hitTargMagnitude
                            end
                        else
                        end
                    else
                    end
                end
            end
		end
	end
	return Target
end

local mt = getrawmetatable(game)
setreadonly(mt, false)
local index = mt.__index
local namecall = mt.__namecall
local hookfunc

mt.__namecall = newcclosure(function(...)
    local method = getnamecallmethod()
    local args = {...}
    if method == getgenv().RayMethodSelected then
        if Hit then
            returnRay(args, Hit)
            return namecall(unpack(args))
		end
	end
    return namecall(unpack(args))
end)

mt.__index = newcclosure(function(func, idx)
    if func == Mouse and tostring(idx) == "Hit" and Hit then
        return Hit.CFrame
    end
    return index(func, idx)
end)

hookfunc = hookfunction(workspace.FindPartOnRayWithIgnoreList, function(...)
    local args = {...}
    if Hit then
        if PlaceId == 625364452 then
            return returnRay(args, Hit)
        else
            returnRay(args, Hit)
        end
    end
    return hookfunc(unpack(args))
end)

fovVal = Instance.new("ObjectValue", game)
fovVal.Changed:Connect(function(player)
    if CoreGui:FindFirstChild("Get_ESP", true) then
        RunServ:UnbindFromRenderStep("Get_Target_ESP")
        CoreGui["Get_ESP"].Folder:ClearAllChildren()
    else
        local ScreenGui = Instance.new("ScreenGui", CoreGui) 
        ScreenGui.Name = "Get_ESP"
        Instance.new("Folder", ScreenGui)
    end
    for _, Player in next, Players:GetPlayers() do
        if Player == player and Player.Character.Humanoid.Health > 0 and getgenv().TargetESP then
            wait()
            espBox = createBox(Player)
            updateEsp(Player, espBox)
            espBox.Parent = CoreGui["Get_ESP"].Folder
        end
    end
end)

RunServ:BindToRenderStep("Get_Target",1,function()
    local Target = getTarget()
    if not Target then
        Hit = nil
        getgenv().SelectedTarget = ""
        fovVal.Value = nil
    elseif Target and getgenv().Loaded then
        getgenv().SelectedTarget = Target.Name .. "\n" .. math.floor((LocalPlayer.Character[getgenv().SelectedPart].Position - Target.Character[getgenv().SelectedPart].Position).magnitude) .. " Studs"
        fovVal.Value = Target
    end
    if UserInput:IsMouseButtonPressed(0) then
        if getgenv().Loaded and Target then
            Hit = Target.Character[getgenv().SelectedPart]
        end
    else
        Hit = nil
    end
end)

warn("Loaded!")
