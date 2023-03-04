repeat task.wait() until game:IsLoaded()

local lplr = game:GetService("Players").LocalPlayer
local TeamsService = game:GetService("Teams")
local RunService = game:GetService("RunService")
local UIS = game:GetService("UserInputService")
local GuiObjects = {}

if game.PlaceId ~= 6872265039 then
    game:GetService("StarterGui"):SetCoreGuiEnabled("PlayerList",  false)
end

local betterTeamColours = {
    Green = Color3.fromRGB(129, 253, 99)
}

local function CreateMainWindow()

    local BedWarsUI = Instance.new("ScreenGui")
    local Scoreboard = Instance.new("Frame")
    local wwweasygg = Instance.new("TextLabel")
    local MainObjects = Instance.new("Frame")
    local UIListLayout = Instance.new("UIListLayout")
    local BEDWARS = Instance.new("TextLabel")
    local GameInfoFrame = Instance.new("Frame")
    local Date = Instance.new("TextLabel")
    local Game = Instance.new("TextLabel")
    local NextEventFrame = Instance.new("Frame")
    local NextEventTimer = Instance.new("TextLabel")
    local NextEvent = Instance.new("TextLabel")

    local TabList = Instance.new("Frame")
    local UIListLayout_2 = Instance.new("UIListLayout")


    --Properties:

    BedWarsUI.Name = "BedWarsUI"
    BedWarsUI.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
    BedWarsUI.DisplayOrder = 999999999
    BedWarsUI.ResetOnSpawn = false

    if gethui and (not KRNL_LOADED) then
        BedWarsUI.Parent = gethui()
    elseif not is_sirhurt_closure and syn and syn.protect_gui then
        syn.protect_gui(BedWarsUI)
        BedWarsUI.Parent = game:GetService("CoreGui")
    else
        BedWarsUI.Parent = game:GetService("CoreGui")
    end

    TabList.Name = "TabList"
    TabList.Parent = BedWarsUI
    TabList.AnchorPoint = Vector2.new(0.5, 0)
    TabList.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    TabList.BackgroundTransparency = 1.000
    TabList.BorderSizePixel = 0
    TabList.Position = UDim2.new(0.5, 0, 0, 10)
    TabList.Size = UDim2.new(0, 540, 0, 30)
    TabList.Visible = false

    UIListLayout_2.Parent = TabList
    --UIListLayout_2.SortOrder = Enum.SortOrder.Name

    GuiObjects.BedWarsUI = BedWarsUI
    GuiObjects.TabList = TabList

    Scoreboard.Name = "Scoreboard"
    Scoreboard.Parent = BedWarsUI
    Scoreboard.AnchorPoint = Vector2.new(0.99000001, 0.5)
    Scoreboard.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
    Scoreboard.BackgroundTransparency = 0.600
    Scoreboard.BorderColor3 = Color3.fromRGB(27, 42, 53)
    Scoreboard.Position = UDim2.new(0.99000001, 0, 0.5, 0)
    Scoreboard.Size = UDim2.new(0, 234, 0, 157)

    wwweasygg.Name = "www.easy.gg"
    wwweasygg.Parent = Scoreboard
    wwweasygg.AnchorPoint = Vector2.new(0, 1)
    wwweasygg.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    wwweasygg.BackgroundTransparency = 1.000
    wwweasygg.BorderSizePixel = 0
    wwweasygg.Position = UDim2.new(0.051282052, 0, 1, 0)
    wwweasygg.Size = UDim2.new(0.948717952, 0, 0.119227365, 0)
    wwweasygg.Font = Enum.Font.SourceSans
    wwweasygg.Text = "www.easy.gg"
    wwweasygg.TextColor3 = Color3.fromRGB(252, 255, 75)
    wwweasygg.TextSize = 27.000
    wwweasygg.TextXAlignment = Enum.TextXAlignment.Left
    wwweasygg.TextYAlignment = Enum.TextYAlignment.Bottom

    MainObjects.Name = "MainObjects"
    MainObjects.Parent = Scoreboard
    MainObjects.AnchorPoint = Vector2.new(0.99000001, 0.5)
    MainObjects.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
    MainObjects.BackgroundTransparency = 1.000
    MainObjects.BorderColor3 = Color3.fromRGB(27, 42, 53)
    MainObjects.Position = UDim2.new(0.99000001, 0, 0.5, 0)
    MainObjects.Size = UDim2.new(1, 0, 1, 0)

    UIListLayout.Parent = MainObjects
    UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Right
    UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder

    BEDWARS.Name = "BEDWARS"
    BEDWARS.Parent = MainObjects
    BEDWARS.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    BEDWARS.BackgroundTransparency = 1.000
    BEDWARS.BorderSizePixel = 0
    BEDWARS.Size = UDim2.new(1, 0, 0.0746753216, 0)
    BEDWARS.Font = Enum.Font.SourceSans
    BEDWARS.Text = "BED WARS"
    BEDWARS.TextColor3 = Color3.fromRGB(252, 255, 75)
    BEDWARS.TextSize = 27.000

    GameInfoFrame.Name = "GameInfoFrame"
    GameInfoFrame.Parent = MainObjects
    GameInfoFrame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    GameInfoFrame.BackgroundTransparency = 1.000
    GameInfoFrame.Position = UDim2.new(0.051282052, 0, 0.0746752992, 0)
    GameInfoFrame.Size = UDim2.new(0, 222, 0, 26)

    Date.Name = "Date"
    Date.Parent = GameInfoFrame
    Date.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    Date.BackgroundTransparency = 1.000
    Date.Position = UDim2.new(0, 0, 0.0746753365, 0)
    Date.Size = UDim2.new(0.440171152, 0, 1, 0)
    Date.Font = Enum.Font.SourceSans
    Date.Text = "MM/DD/YY"
    Date.TextColor3 = Color3.fromRGB(173, 173, 173)
    Date.TextSize = 27.000
    Date.TextWrapped = true
    Date.TextXAlignment = Enum.TextXAlignment.Left

    Game.Name = "Game"
    Game.Parent = GameInfoFrame
    Game.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    Game.BackgroundTransparency = 1.000
    Game.Position = UDim2.new(0.440171093, 0, 0.0746753365, 0)
    Game.Size = UDim2.new(0.47863245, 0, 1, 0)
    Game.Font = Enum.Font.SourceSans
    Game.Text = "m451P"
    Game.TextColor3 = Color3.fromRGB(152, 152, 152)
    Game.TextSize = 27.000
    Game.TextWrapped = true
    Game.TextXAlignment = Enum.TextXAlignment.Left

    NextEventFrame.Name = "NextEventFrame"
    NextEventFrame.Parent = MainObjects
    NextEventFrame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    NextEventFrame.BackgroundTransparency = 1.000
    NextEventFrame.Position = UDim2.new(0.051282052, 0, 0.168538123, 0)
    NextEventFrame.Size = UDim2.new(0, 222, 0, 41)

    NextEventTimer.Name = "NextEventTimer"
    NextEventTimer.Parent = NextEventFrame
    NextEventTimer.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    NextEventTimer.BackgroundTransparency = 1.000
    NextEventTimer.Position = UDim2.new(0.266, 0,0, 0)
    NextEventTimer.Size = UDim2.new(0.135, 0,1, 0)
    NextEventTimer.Font = Enum.Font.SourceSans
    NextEventTimer.Text = "00:00"
    NextEventTimer.TextColor3 = Color3.fromRGB(63, 255, 53)
    NextEventTimer.TextSize = 27.000
    NextEventTimer.TextXAlignment = Enum.TextXAlignment.Left
    NextEventTimer.TextYAlignment = Enum.TextYAlignment.Bottom
    NextEventTimer.AutomaticSize = Enum.AutomaticSize.X

    NextEvent.Name = "NextEvent"
    NextEvent.Parent = NextEventFrame
    NextEvent.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    NextEvent.BackgroundTransparency = 1.000
    NextEvent.Size = UDim2.new(0, 1, 1, 0)
    NextEvent.Font = Enum.Font.SourceSans
    NextEvent.Text = "Time : "
    NextEvent.TextColor3 = Color3.fromRGB(255, 255, 255)
    NextEvent.TextSize = 27.000
    NextEvent.TextXAlignment = Enum.TextXAlignment.Left
    NextEvent.TextYAlignment = Enum.TextYAlignment.Bottom
    NextEvent.AutomaticSize = Enum.AutomaticSize.X
end

local function CreateTeamsFrame()
    local Teams = Instance.new("Frame")
    local TeamContainer = Instance.new("Frame")
    local UIListLayout = Instance.new("UIListLayout")

    Teams.Name = "Teams"
    Teams.Parent = game:GetService("CoreGui").BedWarsUI.Scoreboard or nil
    Teams.AnchorPoint = Vector2.new(0, 0.5)
    Teams.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    Teams.BackgroundTransparency = 1.000
    Teams.BorderSizePixel = 0
    Teams.Position = UDim2.new(0.051282052, 0, 0.5, 0)
    Teams.Size = UDim2.new(0, 222, 1, 0)

    GuiObjects.Teams = Teams

    TeamContainer.Name = "TeamContainer"
    TeamContainer.Parent = Teams
    TeamContainer.AnchorPoint = Vector2.new(0, 0.5)
    TeamContainer.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    TeamContainer.BackgroundTransparency = 1.000
    TeamContainer.Position = UDim2.new(0, 0, 0.600000024, 0)
    TeamContainer.Size = UDim2.new(1, 0, 0.41155234, 0)

    UIListLayout.Parent = TeamContainer
    UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
    UIListLayout.VerticalAlignment = Enum.VerticalAlignment.Center
end

local function CreateTeam(name, team)
    -- Instances:

    local Red = Instance.new("Frame")
    local YOU = Instance.new("TextLabel")
    local Players = Instance.new("TextLabel")
    local Label = Instance.new("TextLabel")
    local OneLetterLabel = Instance.new("TextLabel")
    local UIListLayout = Instance.new("UIListLayout")

    --Properties:

    Red.Name = name
    Red.Parent = GuiObjects.Teams.TeamContainer
    Red.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    Red.BackgroundTransparency = 1.000
    Red.BorderSizePixel = 0
    Red.Position = UDim2.new(0, 0, 0, 26)
    Red.Size = UDim2.new(0, 222, 0, 26)

    UIListLayout.Name = "UIListLayout"
    UIListLayout.Parent = Red
    UIListLayout.FillDirection = Enum.FillDirection.Horizontal
    UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Left
    UIListLayout.SortOrder = Enum.SortOrder.Name

    OneLetterLabel.Name = "!!!!OneLetterLabel"
    OneLetterLabel.Parent = Red
    OneLetterLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    OneLetterLabel.BackgroundTransparency = 1.000
    OneLetterLabel.BorderSizePixel = 0
    OneLetterLabel.Size = UDim2.new(0, 18, 0, 26)
    OneLetterLabel.Font = Enum.Font.SourceSans
    OneLetterLabel.Text = string.sub(name, 1, 1)
    OneLetterLabel.TextColor3 = team.TeamColor.Color
    OneLetterLabel.TextSize = 27.000
    OneLetterLabel.TextXAlignment = Enum.TextXAlignment.Left
    OneLetterLabel.LayoutOrder = 1
    --OneLetterLabel.AutomaticSize = Enum.AutomaticSize.X

    --// better team colours

    for i, v in pairs(betterTeamColours) do
        if name == i then
            OneLetterLabel.TextColor3 = v
        end
    end

    Label.Name = "!!!Label"
    Label.Parent = Red
    Label.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    Label.BackgroundTransparency = 1.000
    Label.BorderSizePixel = 0
    --Label.Position = UDim2.new(0, Label.Size.X.Offset, 0, 0)
    Label.Size = UDim2.new(0, 46, 0, 26)
    Label.Font = Enum.Font.SourceSans
    Label.Text = name .. ":"
    Label.TextColor3 = Color3.fromRGB(255, 255, 255)
    Label.TextSize = 27.000
    Label.TextXAlignment = Enum.TextXAlignment.Left
    Label.AutomaticSize = Enum.AutomaticSize.X
    Label.LayoutOrder = 2

    Players.Name = "!!Players"
    Players.Parent = Red
    Players.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    Players.BackgroundTransparency = 1.000
    Players.BorderSizePixel = 0
    --Players.Position = UDim2.new(0, Label.Size.X.Offset, 0, 0) + UDim2.new(0, OneLetterLabel.Size.X.Offset, 0, 0) + UDim2.new(0, 5, 0, 0)
    Players.Size = UDim2.new(0, 18, 0, 26)
    Players.Font = Enum.Font.SourceSans
    Players.Text = "✓"
    Players.TextColor3 = Color3.fromRGB(63, 255, 53)
    Players.TextSize = 27.000
    Players.TextXAlignment = Enum.TextXAlignment.Left
    Players.LayoutOrder = 3
    Players.AutomaticSize = Enum.AutomaticSize.X
    if Label.Text ~= "Red:" then
        Players.Text = " ✓"
    end

    YOU.Name = "!YOU"
    YOU.Parent = Red
    YOU.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    YOU.BackgroundTransparency = 1.000
    YOU.BorderSizePixel = 0
    --YOU.Position = UDim2.new(0, Label.Size.X.Offset, 0, 0) + UDim2.new(0, OneLetterLabel.Size.X.Offset, 0, 0) + UDim2.new(0, YOU.Size.X.Offset, 0, 0) + UDim2.new(0, 3, 0, 0)
    YOU.Size = UDim2.new(0, 47, 0, 26)
    YOU.Visible = false
    YOU.Font = Enum.Font.SourceSans
    YOU.Text = "YOU"
    YOU.TextColor3 = Color3.fromRGB(173, 173, 173)
    YOU.TextSize = 27.000
    YOU.LayoutOrder = 4

    GuiObjects.BedWarsUI.Scoreboard.Size = GuiObjects.BedWarsUI.Scoreboard.Size + UDim2.new(0, 0, 0, 26)

    task.spawn(function()
        local function updateBoard()
            if lplr.TeamColor.Color == OneLetterLabel.TextColor3 then
                YOU.Visible = true
            else
                YOU.Visible = false
            end

            local teamplrs = 0
            local teamnobed = 0
    
            for _, player in pairs(game:GetService("Players"):GetPlayers()) do
                if player.Team == team then
                    teamplrs += 1
                    
                    if player:FindFirstChild("leaderstats") then
                        if player.leaderstats.Bed.Value == "❌" then
                            teamnobed += 1
                        end
                    end
                end
            end
    
            if teamplrs ~= 0 and teamnobed ~= 0 then
                Players.Text = teamplrs
                if Label.Text ~= "Red:" then
                    Players.Text = " " .. teamplrs
                end
                Players.TextColor3 = Color3.fromRGB(255, 255, 0)
            elseif teamplrs ~= 0 and teamnobed == 0 then
                Players.Text = "✓"
                if Label.Text ~= "Red:" then
                    Players.Text = " ✓"
                end
                Players.TextColor3 = Color3.fromRGB(63, 255, 53)
            elseif teamplrs == 0 then
                Players.Text = "x"
                if Label.Text ~= "Red:" then
                    Players.Text = " x"
                end
                Players.TextColor3 = Color3.fromRGB(255, 0, 0)
            end
        end
    
        RunService.RenderStepped:Connect(updateBoard)
    end)
end

CreateMainWindow()
CreateTeamsFrame()

print(GuiObjects.TabList.Name)

local function addPlayer(player)
    local Player = Instance.new("Frame")
    local ImageLabel = Instance.new("ImageLabel")
    local OneLetterLabel = Instance.new("TextLabel")
    local Name = Instance.new("TextLabel")
    local BedStatus = Instance.new("TextLabel")
    local UIListLayout = Instance.new("UIListLayout")

    UIListLayout.Parent = Player
    UIListLayout.SortOrder = Enum.SortOrder.Name
    UIListLayout.FillDirection = Enum.FillDirection.Horizontal
    
    Player.Name = player.Name
    Player.Parent = GuiObjects.TabList
    Player.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
    Player.BackgroundTransparency = 0.500
    Player.BorderSizePixel = 0
    Player.Size = UDim2.new(1, 0, 0, 30)

    ImageLabel.Parent = Player
    ImageLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    ImageLabel.BackgroundTransparency = 1.000
    ImageLabel.BorderSizePixel = 0
    ImageLabel.Size = UDim2.new(-0.0166666675, 39, 1, 0)
    ImageLabel.Image = game:GetService("Players"):GetUserThumbnailAsync(player.UserId, Enum.ThumbnailType.HeadShot, Enum.ThumbnailSize.Size420x420)
    ImageLabel.Name = "!!!!ImageLabel"

    OneLetterLabel.Name = "!!!OneLetterLabel"
    OneLetterLabel.Parent = Player
    OneLetterLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    OneLetterLabel.BackgroundTransparency = 1.000
    OneLetterLabel.Position = UDim2.new(0.055555556, 0, 0, 0)
    OneLetterLabel.Size = UDim2.new(-0.0166666675, 39, 1, 0)
    OneLetterLabel.Font = Enum.Font.SourceSans
    OneLetterLabel.TextSize = 31.000
    --OneLetterLabel.AutomaticSize = Enum.AutomaticSize.X

    Name.Name = "!!" .. player.DisplayName
    Name.Parent = Player
    Name.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    Name.BackgroundTransparency = 1.000
    Name.Position = UDim2.new(0.111111112, 0, 0, 0)
    Name.Size = UDim2.new(0, 1, 1, 0)
    Name.Font = Enum.Font.SourceSans
    Name.Text = player.DisplayName
    Name.TextColor3 = Color3.fromRGB(255, 255, 255)
    Name.TextSize = 31.000
    Name.AutomaticSize = Enum.AutomaticSize.X
    Name.TextXAlignment = Enum.TextXAlignment.Left

    BedStatus.Name = "!Bedstats"
    BedStatus.Parent = Player
    BedStatus.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    BedStatus.BackgroundTransparency = 1.000
    BedStatus.Position = UDim2.new(0.111111112, 0, 0, 0)
    BedStatus.Size = UDim2.new(0.142592594, 39, 1, 0)
    BedStatus.Font = Enum.Font.SourceSans
    BedStatus.Text = ""
    BedStatus.TextColor3 = Color3.fromRGB(63, 255, 53)
    BedStatus.TextSize = 31.000
    BedStatus.AutomaticSize = Enum.AutomaticSize.X
    BedStatus.TextXAlignment = Enum.TextXAlignment.Left

    task.spawn(function()
        while true do
            if player == nil then
                Player:Destroy()
                break
            end
            if player:FindFirstChild("leaderstats") and player.leaderstats:FindFirstChild("Bed") then
                if player.leaderstats.Bed.Value == "❌" then
                    if player.Team and player.Team.Name == "Spectators" then
                        OneLetterLabel.Text = ""
                        BedStatus.Text = ""
                    else
                        BedStatus.Text = " x"
                        BedStatus.TextColor3 = Color3.fromRGB(255, 0, 0)
                    end
                else
                    BedStatus.Text = " ✓"
                    BedStatus.TextColor3 = Color3.fromRGB(63, 255, 53)
                end
            end

            if player.Team and player.Team.Name ~= "Spectators" then
                OneLetterLabel.Text = string.sub(player.Team.Name, 1, 1)
                OneLetterLabel.TextColor3 = player.TeamColor.Color
            elseif (player.Team and player.Team.Name == "Spectators") or (player.Team == nil) then
                OneLetterLabel.Text = ""
                BedStatus.Text = ""
                if game.PlaceId ~= 6872265039 and player:FindFirstChild("leaderstats") then
                    if player.leaderstats.Bed.Value == "❌" then
                        Player:Destroy()
                        break
                    end
                end
            else
                OneLetterLabel.Text = ""
                Player.LayoutOrder = 999999999
            end

            task.wait()
        end
    end)
end

local function removePlayer(player)
    for i, v in pairs(GuiObjects.TabList:GetChildren()) do
        if v:IsA("Frame") then
            if v.Name == player.Name then
                v:Destroy()
            end
        end
    end
end

_G.DeleteUI = function()
	GuiObjects.BedWarsUI:Destroy()
end

local dt = DateTime.now()
local DateLabel = GuiObjects.BedWarsUI.Scoreboard.MainObjects.GameInfoFrame.Date
DateLabel.Text = dt:FormatLocalTime("L", "en-us")
DateLabel.Text = string.sub(DateLabel.Text, 1, string.len(DateLabel.Text) -2)

for i, v in ipairs(TeamsService:GetTeams()) do
    if v.Name ~= "Spectators" and v.Name ~= "Neutral" then
        CreateTeam(v.Name, v)
    end

    for i2, v2 in pairs(v:GetPlayers()) do
        addPlayer(v2)
    end
end

task.spawn(function() --timer

    pcall(function()
        if not lplr.Character then
            repeat task.wait() until lplr.Character
        end
        repeat task.wait() until lplr.Character.PrimaryPart.Position.Y <= 140 or game.Workspace:FindFirstChild("spawn_cage")

        local eventTimer = GuiObjects.BedWarsUI.Scoreboard.MainObjects.NextEventFrame.NextEventTimer

        local minutes = 0
        local seconds = 0

        while true do
            task.wait(1)
            seconds += 1
            if seconds == 60 then
                seconds = 0
                minutes += 1
            end
            if string.len(tostring(minutes)) <= 1 then
                if string.len(tostring(seconds)) <= 1 then
                    eventTimer.Text = "0" .. tostring(minutes) .. ":0".. tostring(seconds)
                else
                    eventTimer.Text = "0" .. tostring(minutes) .. ":".. tostring(seconds)
                end
            else
                if string.len(tostring(seconds)) <= 1 then
                    eventTimer.Text = tostring(minutes) .. ":0".. tostring(seconds)
                else
                    eventTimer.Text = tostring(minutes) .. ":".. tostring(seconds)
                end
            end
        end
    end)
end)

GuiObjects.TabList:GetPropertyChangedSignal("Visible"):Connect(function()
    if GuiObjects.TabList.Visible == true then
        for i, v in pairs(game:GetService("Players"):GetPlayers()) do
            if not GuiObjects.TabList:FindFirstChild(v.Name) then
                addPlayer(v)
            end
        end
    end
end)

game:GetService("Players").PlayerRemoving:Connect(function(player)
    removePlayer(player)
end)

UIS.InputBegan:Connect(function(input, gameProcessedEvent)
    if gameProcessedEvent then return end
    if input.KeyCode == Enum.KeyCode.Tab then
        GuiObjects.BedWarsUI.TabList.Visible = true
    end
end)

UIS.InputEnded:Connect(function(input, gameProcessedEvent)
    if gameProcessedEvent then return end
    if input.KeyCode == Enum.KeyCode.Tab then
        GuiObjects.BedWarsUI.TabList.Visible = false
    end
end)
