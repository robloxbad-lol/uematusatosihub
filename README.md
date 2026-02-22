--[[
 .____                  ________ ___.    _____                           __                
 |    |    __ _______   \_____  \\_ |___/ ____\_ __  ______ ____ _____ _/  |_  ___________ 
 |    |   |  |  \__  \   /   |   \| __ \   __\  |  \/  ___// ___\\__  \\   __\/  _ \_  __ \
 |    |___|  |  // __ \_/    |    \ \_\ \  | |  |  /\___ \\  \___ / __ \|  | (  <_> )  | \/
 |_______ \____/(____  /\_______  /___  /__| |____//____  >\___  >____  /__|  \____/|__|   
         \/          \/         \/    \/                \/     \/     \/                   
          \_Welcome to LuaObfuscator.com   (Alpha 0.10.9) ~  Much Love, Ferib 

]]--

local v0 = game.CoreGui:FindFirstChild("植松聖HUB");
if v0 then
	v0:Destroy();
end
local v1 = game.Players.LocalPlayer;
local v2 = game:GetService("UserInputService");
local v3 = Instance.new("ScreenGui");
v3.Name = "植松聖HUB";
v3.Parent = game.CoreGui;
v3.ZIndexBehavior = Enum.ZIndexBehavior.Sibling;
_G.NebulaSettings = _G.NebulaSettings or {WalkSpeed=16,InfiniteJump=false,SavedPos=nil,AutoAim=false,FovAim=false};
local v9 = _G.NebulaSettings;
local v10 = false;
local function v11(v354)
	local v355 = 0 - 0;
	local v356;
	while true do
		if (v355 == (3 - 2)) then
			v356.Volume = 6 - 4;
			v356.Parent = game:GetService("SoundService");
			v355 = 362 - (151 + 209);
		end
		if (v355 == (0 + 0)) then
			v356 = Instance.new("Sound");
			v356.SoundId = "rbxassetid://" .. v354;
			v355 = 1481 - (641 + 839);
		end
		if (v355 == (915 - (910 + 3))) then
			v356.PlayOnRemove = true;
			v356:Destroy();
			break;
		end
	end
end
local function v12(v357)
	local v358 = 0 - 0;
	local v359;
	local v360;
	while true do
		if (v358 == (1685 - (1466 + 218))) then
			v359.BackgroundColor3 = Color3.fromRGB(14 + 16, 0, 1148 - (556 + 592));
			Instance.new("UICorner", v359);
			Instance.new("UIStroke", v359).Color = Color3.fromRGB(91 + 164, 0, 808 - (329 + 479));
			v358 = 856 - (174 + 680);
		end
		if (v358 == 2) then
			v360 = Instance.new("TextLabel", v359);
			v360.Size = UDim2.new(3 - 2, 0, 1 - 0, 0 + 0);
			v360.Text = v357;
			v358 = 742 - (396 + 343);
		end
		if ((0 + 0) == v358) then
			local v1012 = 1477 - (29 + 1448);
			while true do
				if (v1012 == (1390 - (135 + 1254))) then
					v359.Position = UDim2.new(1.1, 0, 0.9 - 0, 0 - 0);
					v358 = 1 + 0;
					break;
				end
				if (v1012 == (1527 - (389 + 1138))) then
					v359 = Instance.new("Frame", v3);
					v359.Size = UDim2.new(574 - (102 + 472), 208 + 12, 0 + 0, 47 + 3);
					v1012 = 1;
				end
			end
		end
		if (v358 == (1550 - (320 + 1225))) then
			task.delay(2 - 0, function()
				if (v359 and v359.Parent) then
					local v1316 = 0 + 0;
					local v1317;
					while true do
						if (v1316 == (1464 - (157 + 1307))) then
							v1317 = 1859 - (821 + 1038);
							while true do
								if (v1317 == (0 - 0)) then
									v359:TweenPosition(UDim2.new(1.1, 0, 0.9, 0 + 0), "In", "Quart", 0.3);
									task.wait(0.4 - 0);
									v1317 = 1 + 0;
								end
								if (v1317 == (2 - 1)) then
									v359:Destroy();
									break;
								end
							end
							break;
						end
					end
				end
			end);
			break;
		end
		if (v358 == 3) then
			v360.TextColor3 = Color3.fromRGB(1281 - (834 + 192), 17 + 238, 255);
			v360.Font = Enum.Font.SourceSansBold;
			v360.TextSize = 14;
			v358 = 4;
		end
		if (v358 == (2 + 2)) then
			v360.BackgroundTransparency = 1 + 0;
			v11("6518811702");
			v359:TweenPosition(UDim2.new(1 - 0, -(534 - (300 + 4)), 0.9, 0), "Out", "Quart", 0.3 + 0);
			v358 = 13 - 8;
		end
	end
end
local v13 = v2.JumpRequest:Connect(function()
	if v9.InfiniteJump then
		local v920 = 362 - (112 + 250);
		local v921;
		local v922;
		local v923;
		while true do
			if (v920 == (1 + 0)) then
				v923 = nil;
				while true do
					if ((2 - 1) == v921) then
						if v923 then
							v923:ChangeState(Enum.HumanoidStateType.Jumping);
						end
						break;
					end
					if (0 == v921) then
						v922 = v1.Character;
						v923 = v922 and v922:FindFirstChildOfClass("Humanoid");
						v921 = 1;
					end
				end
				break;
			end
			if ((0 + 0) == v920) then
				v921 = 0 + 0;
				v922 = nil;
				v920 = 1 + 0;
			end
		end
	end
end);
task.spawn(function()
	while task.wait(1 + 0) do
		local v814 = 0 + 0;
		local v815;
		while true do
			if (v814 == (1414 - (1001 + 413))) then
				v815 = v1.Character and v1.Character:FindFirstChildOfClass("Humanoid");
				if (v815 and (v815.WalkSpeed ~= v9.WalkSpeed)) then
					v815.WalkSpeed = v9.WalkSpeed;
				end
				break;
			end
		end
	end
end);
local function v14(v361)
	local v362 = 0 - 0;
	local v363;
	local v364;
	local v365;
	while true do
		if (v362 == (883 - (244 + 638))) then
			v2.InputChanged:Connect(function(v1129)
				if (v363 and (v1129.UserInputType == Enum.UserInputType.MouseMovement)) then
					local v1320 = v1129.Position - v364;
					v361.Position = UDim2.new(v365.X.Scale, v365.X.Offset + v1320.X, v365.Y.Scale, v365.Y.Offset + v1320.Y);
				end
			end);
			v2.InputEnded:Connect(function(v1130)
				if (v1130.UserInputType == Enum.UserInputType.MouseButton1) then
					v363 = false;
				end
			end);
			break;
		end
		if ((693 - (627 + 66)) == v362) then
			v363, v364, v365 = nil;
			v361.InputBegan:Connect(function(v1131)
				if (not v10 and (v1131.UserInputType == Enum.UserInputType.MouseButton1)) then
					local v1322 = 0;
					while true do
						if (v1322 == (0 - 0)) then
							v363 = true;
							v364 = v1131.Position;
							v1322 = 1;
						end
						if (v1322 == 1) then
							v365 = v361.Position;
							break;
						end
					end
				end
			end);
			v362 = 603 - (512 + 90);
		end
	end
end
local v15 = Instance.new("Frame", v3);
v15.Size = UDim2.new(1906 - (1665 + 241), 1267 - (373 + 344), 0 + 0, 350);
v15.Position = UDim2.new(0.5 + 0, -275, 0.5, -(461 - 286));
v15.BackgroundColor3 = Color3.fromRGB(10, 0 - 0, 1099 - (35 + 1064));
v14(v15);
Instance.new("UICorner", v15);
Instance.new("UIStroke", v15).Color = Color3.fromRGB(255, 37 + 13, 0 - 0);
local v20 = Instance.new("TextLabel", v15);
v20.Size = UDim2.new(0, 200, 0 + 0, 1276 - (298 + 938));
v20.Position = UDim2.new(1259 - (233 + 1026), 1806 - (636 + 1030), 0 + 0, 0);
v20.Text = "植松聖HUB";
v20.TextColor3 = Color3.fromRGB(250 + 5, 50, 0 + 0);
v20.Font = Enum.Font.SourceSansItalic;
v20.TextSize = 2 + 20;
v20.TextXAlignment = Enum.TextXAlignment.Left;
v20.BackgroundTransparency = 222 - (55 + 166);
local v31 = Instance.new("TextButton", v15);
v31.Size = UDim2.new(0, 6 + 24, 0, 4 + 26);
v31.Position = UDim2.new(3 - 2, -35, 0, 302 - (36 + 261));
v31.BackgroundColor3 = Color3.fromRGB(262 - 112, 1368 - (34 + 1334), 0 + 0);
v31.Text = "×";
v31.TextColor3 = Color3.fromRGB(199 + 56, 1538 - (1035 + 248), 276 - (20 + 1));
Instance.new("UICorner", v31);
local v37 = Instance.new("Frame", v3);
v37.Size = UDim2.new(0, 131 + 119, 319 - (134 + 185), 1253 - (549 + 584));
v37.Position = UDim2.new(685.5 - (314 + 371), -125, 0.5 - 0, -60);
v37.BackgroundColor3 = Color3.fromRGB(20, 968 - (478 + 490), 0);
v37.Visible = false;
v37.ZIndex = 1060 + 940;
Instance.new("UICorner", v37);
Instance.new("UIStroke", v37).Color = Color3.fromRGB(1427 - (786 + 386), 0, 0);
local v44 = Instance.new("TextLabel", v37);
v44.Size = UDim2.new(3 - 2, 0, 1379 - (1055 + 324), 1390 - (1093 + 247));
v44.Text = "完全に終了しますか？";
v44.TextColor3 = Color3.fromRGB(227 + 28, 27 + 228, 1012 - 757);
v44.BackgroundTransparency = 1;
local v49 = Instance.new("TextButton", v37);
v49.Size = UDim2.new(0 - 0, 284 - 184, 0, 40);
v49.Position = UDim2.new(0 - 0, 20, 0 + 0, 231 - 171);
v49.BackgroundColor3 = Color3.fromRGB(344 - 244, 0 + 0, 0);
v49.Text = "はい";
v49.TextColor3 = Color3.fromRGB(652 - 397, 943 - (364 + 324), 255);
Instance.new("UICorner", v49);
local v55 = Instance.new("TextButton", v37);
v55.Size = UDim2.new(0 - 0, 239 - 139, 0, 40);
v55.Position = UDim2.new(1, -(40 + 80), 0 - 0, 60);
v55.BackgroundColor3 = Color3.fromRGB(80 - 30, 151 - 101, 1318 - (1249 + 19));
v55.Text = "いいえ";
v55.TextColor3 = Color3.fromRGB(231 + 24, 992 - 737, 1341 - (686 + 400));
Instance.new("UICorner", v55);
v49.MouseButton1Click:Connect(function()
	local v366 = 0;
	local v367;
	while true do
		if ((0 + 0) == v366) then
			v9.InfiniteJump = false;
			v13:Disconnect();
			v366 = 1;
		end
		if ((230 - (73 + 156)) == v366) then
			v367 = v1.Character and v1.Character:FindFirstChildOfClass("Humanoid");
			if v367 then
				v367.WalkSpeed = 1 + 15;
			end
			v366 = 813 - (721 + 90);
		end
		if (v366 == (1 + 1)) then
			v3:Destroy();
			break;
		end
	end
end);
v55.MouseButton1Click:Connect(function()
	v37.Visible = false;
end);
v31.MouseButton1Click:Connect(function()
	v37.Visible = true;
end);
local v61 = Instance.new("ImageButton", v3);
v61.Size = UDim2.new(0 - 0, 530 - (224 + 246), 0 - 0, 110 - 50);
v61.Position = UDim2.new(0, 4 + 16, 0.5 + 0, -(23 + 7));
v61.BackgroundColor3 = Color3.fromRGB(39 - 19, 0 - 0, 0);
v61.Image = "rbxassetid://94535192599903";
v14(v61);
Instance.new("UICorner", v61);
Instance.new("UIStroke", v61).Color = Color3.fromRGB(255, 513 - (203 + 310), 1993 - (1238 + 755));
v2.InputBegan:Connect(function(v370, v371)
	if (not v371 and (v370.KeyCode == Enum.KeyCode.K)) then
		local v924 = 0 + 0;
		while true do
			if (v924 == (1534 - (709 + 825))) then
				v11("6895079853");
				v15.Visible = not v15.Visible;
				break;
			end
		end
	end
end);
v61.MouseButton1Click:Connect(function()
	local v372 = 0;
	while true do
		if (v372 == (0 - 0)) then
			v11("6895079853");
			v15.Visible = not v15.Visible;
			break;
		end
	end
end);
local v67 = Instance.new("ScrollingFrame", v15);
v67.Size = UDim2.new(0 - 0, 130, 865 - (196 + 668), -10);
v67.Position = UDim2.new(0 - 0, 0 - 0, 833 - (171 + 662), 5);
v67.BackgroundColor3 = Color3.fromRGB(108 - (4 + 89), 0 - 0, 0 + 0);
v67.BorderSizePixel = 0 - 0;
v67.ScrollBarThickness = 2;
v67.AutomaticCanvasSize = Enum.AutomaticSize.Y;
v67.CanvasSize = UDim2.new(0 + 0, 1486 - (35 + 1451), 1453 - (28 + 1425), 1993 - (941 + 1052));
local v76 = Instance.new("Frame", v15);
v76.Size = UDim2.new(1, -(135 + 5), 1, -(1564 - (822 + 692)));
v76.Position = UDim2.new(0 - 0, 66 + 74, 297 - (45 + 252), 50);
v76.BackgroundTransparency = 1 + 0;
local v80 = Instance.new("ImageLabel", v67);
v80.Size = UDim2.new(0 + 0, 121 - 71, 433 - (114 + 319), 50);
v80.Position = UDim2.new(0.5 - 0, -25, 0 - 0, 10 + 5);
v80.Image = game.Players:GetUserThumbnailAsync(v1.UserId, Enum.ThumbnailType.HeadShot, Enum.ThumbnailSize.Size100x100);
Instance.new("UICorner", v80).CornerRadius = UDim.new(1, 0 - 0);
local v85 = Instance.new("TextLabel", v67);
v85.Size = UDim2.new(1, 0 - 0, 1963 - (556 + 1407), 20);
v85.Position = UDim2.new(0, 0, 1206 - (741 + 465), 535 - (170 + 295));
v85.Text = v1.DisplayName;
v85.TextColor3 = Color3.fromRGB(135 + 120, 255, 235 + 20);
v85.Font = Enum.Font.SourceSansBold;
v85.TextSize = 34 - 20;
v85.BackgroundTransparency = 1 + 0;
local v95 = Instance.new("UIListLayout", v67);
v95.Padding = UDim.new(0 + 0, 5 + 3);
v95.HorizontalAlignment = Enum.HorizontalAlignment.Center;
local v99 = Instance.new("Frame", v67);
v99.Size = UDim2.new(1230 - (957 + 273), 0 + 0, 0 + 0, 95);
v99.BackgroundTransparency = 1;
local function v102(v373)
	local v374 = Instance.new("ScrollingFrame", v76);
	v374.Size = UDim2.new(3 - 2, 0 - 0, 2 - 1, 0 - 0);
	v374.BackgroundTransparency = 1781 - (389 + 1391);
	v374.Visible = false;
	v374.ScrollBarThickness = 3 + 1;
	v374.BorderSizePixel = 0;
	v374.ClipsDescendants = true;
	local v381 = Instance.new("UIListLayout", v374);
	v381.Padding = UDim.new(0 + 0, 26 - 14);
	v381.SortOrder = Enum.SortOrder.LayoutOrder;
	v381:GetPropertyChangedSignal("AbsoluteContentSize"):Connect(function()
		v374.CanvasSize = UDim2.new(0, 951 - (783 + 168), 0, v381.AbsoluteContentSize.Y + 50);
	end);
	local v385 = Instance.new("TextButton", v67);
	v385.Size = UDim2.new(0, 115, 0 - 0, 40);
	v385.BackgroundColor3 = Color3.fromRGB(35 + 0, 0, 0);
	v385.Text = v373:upper();
	v385.TextColor3 = Color3.fromRGB(255, 566 - (309 + 2), 255);
	v385.Font = Enum.Font.SourceSansBold;
	v385.TextSize = 55 - 37;
	Instance.new("UICorner", v385);
	v385.MouseButton1Click:Connect(function()
		local v817 = 0;
		while true do
			if (v817 == (1212 - (1090 + 122))) then
				v11("6895079853");
				for v1232, v1233 in pairs(v76:GetChildren()) do
					if v1233:IsA("ScrollingFrame") then
						v1233.Visible = false;
					end
				end
				v817 = 1 + 0;
			end
			if (v817 == (3 - 2)) then
				v374.Visible = true;
				v374.CanvasSize = UDim2.new(0 + 0, 1118 - (628 + 490), 0, v381.AbsoluteContentSize.Y + 50);
				break;
			end
		end
	end);
	return v374;
end
local function v103(v393, v394, v395, v396)
	local v397 = 0 + 0;
	local v398;
	local v399;
	local v400;
	local v401;
	local v402;
	while true do
		if (v397 == (0 - 0)) then
			v398 = Instance.new("TextButton", v393);
			v398.Size = UDim2.new(4 - 3, -10, 774 - (431 + 343), 90 - 45);
			v398.BackgroundColor3 = Color3.fromRGB(25, 0 - 0, 0 + 0);
			v398.Text = "";
			v397 = 1 + 0;
		end
		if (v397 == (1700 - (556 + 1139))) then
			v401.Size = UDim2.new(0, 16, 15 - (6 + 9), 16);
			v401.Position = (v395 and UDim2.new(1 + 0, -18, 0.5 + 0, -8)) or UDim2.new(169 - (28 + 141), 1 + 1, 0.5 - 0, -(6 + 2));
			v401.BackgroundColor3 = Color3.fromRGB(1572 - (486 + 831), 663 - 408, 897 - 642);
			Instance.new("UICorner", v401).CornerRadius = UDim.new(1 + 0, 0 - 0);
			v397 = 1269 - (668 + 595);
		end
		if (v397 == (4 + 0)) then
			v400.Position = UDim2.new(1 + 0, -(136 - 86), 290.5 - (23 + 267), -10);
			v400.BackgroundColor3 = (v395 and Color3.fromRGB(2199 - (1129 + 815), 0, 0)) or Color3.fromRGB(437 - (371 + 16), 1750 - (1326 + 424), 0 - 0);
			Instance.new("UICorner", v400).CornerRadius = UDim.new(3 - 2, 0);
			v401 = Instance.new("Frame", v400);
			v397 = 123 - (88 + 30);
		end
		if (v397 == (774 - (720 + 51))) then
			v399.BackgroundTransparency = 2 - 1;
			v399.TextXAlignment = Enum.TextXAlignment.Left;
			v400 = Instance.new("Frame", v398);
			v400.Size = UDim2.new(1776 - (421 + 1355), 40, 0 - 0, 10 + 10);
			v397 = 1087 - (286 + 797);
		end
		if (v397 == (3 - 2)) then
			Instance.new("UICorner", v398);
			v399 = Instance.new("TextLabel", v398);
			v399.Size = UDim2.new(1 - 0, -60, 440 - (397 + 42), 0 + 0);
			v399.Position = UDim2.new(800 - (24 + 776), 10, 0, 0 - 0);
			v397 = 787 - (222 + 563);
		end
		if (v397 == 6) then
			v402 = v395;
			v398.MouseButton1Click:Connect(function()
				local v1134 = 0 - 0;
				while true do
					if (v1134 == (1 + 0)) then
						v400.BackgroundColor3 = (v402 and Color3.fromRGB(445 - (23 + 167), 1798 - (690 + 1108), 0 + 0)) or Color3.fromRGB(50, 0 + 0, 848 - (40 + 808));
						v401:TweenPosition((v402 and UDim2.new(1 + 0, -(68 - 50), 0.5 + 0, -(5 + 3))) or UDim2.new(0, 2, 0.5, -(5 + 3)), "Out", "Quart", 571.2 - (47 + 524));
						v1134 = 2 + 0;
					end
					if ((0 - 0) == v1134) then
						v402 = not v402;
						v11("6895079853");
						v1134 = 1;
					end
					if (v1134 == (2 - 0)) then
						v396(v402);
						v12(v394 .. ((v402 and ": ON") or ": OFF"));
						break;
					end
				end
			end);
			break;
		end
		if (v397 == (4 - 2)) then
			v399.Text = v394;
			v399.TextColor3 = Color3.fromRGB(1981 - (1165 + 561), 255, 8 + 247);
			v399.Font = Enum.Font.SourceSansBold;
			v399.TextSize = 49 - 33;
			v397 = 3;
		end
	end
end
local function v104(v403, v404, v405, v406, v407, v408)
	local v409 = 0 + 0;
	local v410;
	local v411;
	local v412;
	local v413;
	local v414;
	local v415;
	while true do
		if ((485 - (341 + 138)) == v409) then
			function v415()
				local v1135 = 0 + 0;
				local v1136;
				local v1137;
				local v1138;
				while true do
					if (v1135 == (1 - 0)) then
						v1138 = nil;
						while true do
							if (v1136 == (328 - (89 + 237))) then
								v408(v1138);
								break;
							end
							if ((0 - 0) == v1136) then
								local v1618 = 0;
								while true do
									if (v1618 == (0 - 0)) then
										v1137 = math.clamp((v2:GetMouseLocation().X - v412.AbsolutePosition.X) / v412.AbsoluteSize.X, 0, 882 - (581 + 300));
										v413.Size = UDim2.new(v1137, 1220 - (855 + 365), 2 - 1, 0 + 0);
										v1618 = 1;
									end
									if (v1618 == (1236 - (1030 + 205))) then
										v1136 = 1 + 0;
										break;
									end
								end
							end
							if (v1136 == 1) then
								v1138 = math.floor(v405 + ((v406 - v405) * v1137));
								v411.Text = v404 .. " : " .. v1138;
								v1136 = 2 + 0;
							end
						end
						break;
					end
					if (v1135 == (286 - (156 + 130))) then
						v1136 = 0 - 0;
						v1137 = nil;
						v1135 = 1;
					end
				end
			end
			v412.InputBegan:Connect(function(v1139)
				if (v1139.UserInputType == Enum.UserInputType.MouseButton1) then
					local v1323 = 0;
					while true do
						if (v1323 == 0) then
							v414 = true;
							v10 = true;
							break;
						end
					end
				end
			end);
			v2.InputEnded:Connect(function(v1140)
				if ((v1140.UserInputType == Enum.UserInputType.MouseButton1) and v414) then
					local v1324 = 0 - 0;
					while true do
						if (v1324 == (0 - 0)) then
							v414 = false;
							v10 = false;
							v1324 = 1;
						end
						if (v1324 == 1) then
							v12(v404 .. "を保存");
							break;
						end
					end
				end
			end);
			v2.InputChanged:Connect(function(v1141)
				if (v414 and (v1141.UserInputType == Enum.UserInputType.MouseMovement)) then
					v415();
				end
			end);
			break;
		end
		if (v409 == 1) then
			v411 = Instance.new("TextLabel", v410);
			v411.Size = UDim2.new(1 + 0, -10, 0 + 0, 89 - (10 + 59));
			v411.Position = UDim2.new(0 + 0, 10, 0 - 0, 1168 - (671 + 492));
			v411.Text = v404 .. " : " .. v407;
			v409 = 2;
		end
		if (v409 == 5) then
			v413.BackgroundColor3 = Color3.fromRGB(203 + 52, 1215 - (369 + 846), 0 + 0);
			Instance.new("UICorner", v413);
			v414 = false;
			v415 = nil;
			v409 = 6 + 0;
		end
		if (2 == v409) then
			v411.TextColor3 = Color3.fromRGB(2200 - (1036 + 909), 255, 203 + 52);
			v411.Font = Enum.Font.SourceSansBold;
			v411.TextSize = 15;
			v411.BackgroundTransparency = 1 - 0;
			v409 = 206 - (11 + 192);
		end
		if (v409 == (3 + 1)) then
			v412.BackgroundColor3 = Color3.fromRGB(50, 175 - (135 + 40), 0 - 0);
			Instance.new("UICorner", v412);
			v413 = Instance.new("Frame", v412);
			v413.Size = UDim2.new((v407 - v405) / (v406 - v405), 0, 1, 0 + 0);
			v409 = 5;
		end
		if ((6 - 3) == v409) then
			v411.TextXAlignment = Enum.TextXAlignment.Left;
			v412 = Instance.new("Frame", v410);
			v412.Size = UDim2.new(1 - 0, -(196 - (50 + 126)), 0 - 0, 2 + 6);
			v412.Position = UDim2.new(1413 - (1233 + 180), 10, 969 - (522 + 447), 35);
			v409 = 4;
		end
		if (v409 == (1421 - (107 + 1314))) then
			v410 = Instance.new("Frame", v403);
			v410.Size = UDim2.new(1 + 0, -10, 0, 167 - 112);
			v410.BackgroundColor3 = Color3.fromRGB(11 + 14, 0 - 0, 0 - 0);
			Instance.new("UICorner", v410);
			v409 = 1911 - (716 + 1194);
		end
	end
end
local function v105(v416, v417, v418)
	local v419 = 0 + 0;
	local v420;
	while true do
		if (v419 == 2) then
			v420.TextColor3 = Color3.fromRGB(255, 28 + 227, 758 - (74 + 429));
			v420.Font = Enum.Font.SourceSansBold;
			v419 = 5 - 2;
		end
		if (v419 == (0 + 0)) then
			local v1061 = 0 - 0;
			while true do
				if (v1061 == 0) then
					v420 = Instance.new("TextButton", v416);
					v420.Size = UDim2.new(1 + 0, -(30 - 20), 0, 111 - 66);
					v1061 = 1;
				end
				if (v1061 == (434 - (279 + 154))) then
					v419 = 779 - (454 + 324);
					break;
				end
			end
		end
		if (v419 == 1) then
			v420.BackgroundColor3 = Color3.fromRGB(35, 0 + 0, 0);
			v420.Text = v417;
			v419 = 19 - (12 + 5);
		end
		if (v419 == (2 + 1)) then
			v420.TextSize = 40 - 24;
			Instance.new("UICorner", v420);
			v419 = 2 + 2;
		end
		if (v419 == 4) then
			v420.MouseButton1Click:Connect(function()
				local v1142 = 0;
				while true do
					if (v1142 == (1093 - (277 + 816))) then
						v11("6895079853");
						v418();
						break;
					end
				end
			end);
			break;
		end
	end
end
local v106 = v102("Main");
local v107 = v102("Player");
local v108 = v102("BloxFruits");
v106.Visible = true;
v103(v106, "無限ジャンプ", v9.InfiniteJump, function(v421)
	v9.InfiniteJump = v421;
end);
v105(v106, "現在の場所を保存", function()
	local v423 = 0 - 0;
	local v424;
	while true do
		if (v423 == (1183 - (1058 + 125))) then
			v424 = v1.Character and v1.Character:FindFirstChild("HumanoidRootPart");
			if v424 then
				local v1234 = 0 + 0;
				local v1235;
				while true do
					if (v1234 == 0) then
						v1235 = 975 - (815 + 160);
						while true do
							if (v1235 == (0 - 0)) then
								v9.SavedPos = v424.Position;
								v12("位置を保存しました");
								break;
							end
						end
						break;
					end
				end
			end
			break;
		end
	end
end);
v105(v106, "保存地点へテレポート", function()
	local v425 = v1.Character and v1.Character:FindFirstChild("HumanoidRootPart");
	if (v9.SavedPos and v425) then
		local v925 = 0;
		while true do
			if (v925 == (0 - 0)) then
				v425.CFrame = CFrame.new(v9.SavedPos);
				v12("移動しました");
				break;
			end
		end
	end
end);
v104(v107, "移動速度", 4 + 12, 250, v9.WalkSpeed, function(v426)
	v9.WalkSpeed = v426;
	local v428 = v1.Character and v1.Character:FindFirstChildOfClass("Humanoid");
	if v428 then
		v428.WalkSpeed = v426;
	end
end);
local v110 = false;
local v111 = workspace.CurrentCamera;
v103(v106, "オートエイム", v9.AutoAim, function(v429)
	v9.AutoAim = v429;
end);
v2.InputBegan:Connect(function(v431)
	if (v431.UserInputType == Enum.UserInputType.MouseButton2) then
		v110 = true;
	end
end);
v2.InputEnded:Connect(function(v432)
	if (v432.UserInputType == Enum.UserInputType.MouseButton2) then
		v110 = false;
	end
end);
game:GetService("RunService").RenderStepped:Connect(function()
	if (v9.AutoAim and v110) then
		local v927 = nil;
		local v928 = math.huge;
		for v1065, v1066 in pairs(game.Players:GetPlayers()) do
			if ((v1066 ~= v1) and v1066.Character and v1066.Character:FindFirstChild("Head")) then
				local v1237 = 0 - 0;
				local v1238;
				while true do
					if (v1237 == 0) then
						v1238 = v1066.Character:FindFirstChildOfClass("Humanoid");
						if (v1238 and (v1238.Health > (1898 - (41 + 1857)))) then
							local v1620 = v1066.Character.Head;
							local v1621 = (v1620.Position - v111.CFrame.Position).Magnitude;
							if (v1621 < v928) then
								local v1712 = 1893 - (1222 + 671);
								while true do
									if (v1712 == 0) then
										v928 = v1621;
										v927 = v1066;
										break;
									end
								end
							end
						end
						break;
					end
				end
			end
		end
		if (v927 and v927.Character and v927.Character:FindFirstChild("Head")) then
			v111.CFrame = CFrame.new(v111.CFrame.Position, v927.Character.Head.Position);
		end
	end
end);
v105(v106, "Fly", function()
	local v433 = 0;
	local v434;
	while true do
		if (v433 == (0 - 0)) then
			v434 = 0 - 0;
			while true do
				if (v434 == (1182 - (229 + 953))) then
					loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))();
					v12("Flyスクリプトを実行しました");
					break;
				end
			end
			break;
		end
	end
end);
local v112 = false;
local v113 = 1974 - (1111 + 663);
local v114 = Vector2.new();
local v115 = Drawing.new("Circle");
v115.Radius = v113;
v115.Color = Color3.fromRGB(1834 - (874 + 705), 36 + 219, 174 + 81);
v115.Thickness = 1;
v115.Transparency = 0.5 - 0;
v115.Visible = false;
v115.Filled = false;
v103(v106, "オートエイム（FOV）", v9.FovAim, function(v435)
	v9.FovAim = v435;
	v115.Visible = v435;
end);
v2.InputBegan:Connect(function(v438)
	if (v438.UserInputType == Enum.UserInputType.MouseButton2) then
		v112 = true;
	elseif (v438.UserInputType == Enum.UserInputType.MouseMovement) then
		v114 = Vector2.new(v438.Position.X, v438.Position.Y);
	end
end);
v2.InputChanged:Connect(function(v439)
	if (v439.UserInputType == Enum.UserInputType.MouseMovement) then
		v114 = Vector2.new(v439.Position.X, v439.Position.Y);
	end
end);
v2.InputEnded:Connect(function(v440)
	if (v440.UserInputType == Enum.UserInputType.MouseButton2) then
		v112 = false;
	end
end);
game:GetService("RunService").RenderStepped:Connect(function()
	local v441 = 0 + 0;
	while true do
		if (v441 == (679 - (642 + 37))) then
			v115.Position = v114;
			if (v9.FovAim and v112) then
				local v1239 = nil;
				local v1240 = math.huge;
				for v1326, v1327 in pairs(game.Players:GetPlayers()) do
					if ((v1327 ~= v1) and v1327.Character and v1327.Character:FindFirstChild("Head")) then
						local v1470 = 0 + 0;
						local v1471;
						local v1472;
						local v1473;
						while true do
							if (v1470 == (1 + 0)) then
								v1473 = nil;
								while true do
									if (1 == v1471) then
										if (v1473 and (v1473.Health > 0)) then
											local v1796, v1797 = v111:WorldToViewportPoint(v1472.Position);
											if v1797 then
												local v1818 = 0;
												local v1819;
												while true do
													if (v1818 == (0 - 0)) then
														v1819 = (Vector2.new(v1796.X, v1796.Y) - v114).Magnitude;
														if (v1819 <= v113) then
															local v1834 = 454 - (233 + 221);
															local v1835;
															while true do
																if (v1834 == (0 - 0)) then
																	v1835 = (v1472.Position - v111.CFrame.Position).Magnitude;
																	if (v1835 < v1240) then
																		local v1841 = 0 + 0;
																		local v1842;
																		while true do
																			if (v1841 == (1541 - (718 + 823))) then
																				v1842 = 0 + 0;
																				while true do
																					if (v1842 == (805 - (266 + 539))) then
																						v1240 = v1835;
																						v1239 = v1327;
																						break;
																					end
																				end
																				break;
																			end
																		end
																	end
																	break;
																end
															end
														end
														break;
													end
												end
											end
										end
										break;
									end
									if (v1471 == (0 - 0)) then
										v1472 = v1327.Character.Head;
										v1473 = v1327.Character:FindFirstChildOfClass("Humanoid");
										v1471 = 1;
									end
								end
								break;
							end
							if (v1470 == 0) then
								v1471 = 1225 - (636 + 589);
								v1472 = nil;
								v1470 = 2 - 1;
							end
						end
					end
				end
				if (v1239 and v1239.Character:FindFirstChild("Head")) then
					v111.CFrame = CFrame.new(v111.CFrame.Position, v1239.Character.Head.Position);
				end
			end
			break;
		end
	end
end);
task.spawn(function()
	local v442 = 0 - 0;
	local v443;
	local v444;
	while true do
		if (v442 == (0 + 0)) then
			if not _G.Settings then
				_G.Settings = {};
			end
			_G.Settings.DisableHit = true;
			v442 = 1 + 0;
		end
		if (v442 == 2) then
			local v1068 = 1015 - (657 + 358);
			while true do
				if (v1068 == (2 - 1)) then
					v442 = 6 - 3;
					break;
				end
				if (v1068 == 0) then
					v444 = nil;
					function v444(v1399)
						local v1400 = 0;
						local v1401;
						local v1402;
						while true do
							if (v1400 == (1187 - (1151 + 36))) then
								local v1622 = 0 + 0;
								while true do
									if (v1622 == 1) then
										v1400 = 1 + 0;
										break;
									end
									if (v1622 == (0 - 0)) then
										v1401 = 1832 - (1552 + 280);
										v1402 = game.Players.LocalPlayer.Character;
										v1622 = 1;
									end
								end
							end
							if (1 == v1400) then
								for v1686, v1687 in ipairs(workspace:GetDescendants()) do
									if v1687:IsA("BasePart") then
										pcall(function()
											if (not v1402 or not v1687:IsDescendantOf(v1402)) then
												v1687.CanTouch = not v1399;
											end
										end);
									end
									v1401 = v1401 + 1;
									if ((v1401 % 1000) == (834 - (64 + 770))) then
										task.wait();
									end
								end
								break;
							end
						end
					end
					v1068 = 1 + 0;
				end
			end
		end
		if (v442 == (6 - 3)) then
			task.spawn(function()
				v444(_G.Settings.DisableHit);
			end);
			workspace.DescendantAdded:Connect(function(v1144)
				if (_G.Settings.DisableHit and v1144:IsA("BasePart")) then
					pcall(function()
						local v1403 = 0 + 0;
						local v1404;
						while true do
							if (0 == v1403) then
								v1404 = game.Players.LocalPlayer.Character;
								if (not v1404 or not v1144:IsDescendantOf(v1404)) then
									v1144.CanTouch = false;
								end
								break;
							end
						end
					end);
				end
			end);
			v442 = 1247 - (157 + 1086);
		end
		if (v442 == (1 - 0)) then
			v443 = v106;
			if (not v443 and Window) then
				for v1328, v1329 in pairs(Window) do
					if ((type(v1329) == "table") and ((v1329.Name == "Main") or (v1329.Title == "Main"))) then
						v443 = v1329;
						break;
					end
				end
			end
			v442 = 8 - 6;
		end
		if (v442 == 4) then
			if v443 then
				pcall(function()
					v103(v443, "オブジェクトダメージ無効化", _G.Settings.DisableHit, function(v1405)
						local v1406 = 0;
						while true do
							if (v1406 == (0 - 0)) then
								_G.Settings.DisableHit = v1405;
								task.spawn(function()
									v444(v1405);
								end);
								v1406 = 1 - 0;
							end
							if (v1406 == (820 - (599 + 220))) then
								v12("ダメージ無効化: " .. ((v1405 and "ON") or "OFF"));
								break;
							end
						end
					end);
				end);
			else
				warn("MainTabが見つかりませんでした。");
			end
			break;
		end
	end
end);
local v122 = false;
local v123 = nil;
local v124 = workspace.CurrentCamera;
local v125 = Instance.new("Frame", v108);
v125.Size = UDim2.new(1 - 0, -10, 0, 2111 - (1813 + 118));
v125.BackgroundColor3 = Color3.fromRGB(20, 0 + 0, 1217 - (841 + 376));
Instance.new("UICorner", v125);
local v128 = Instance.new("TextLabel", v125);
v128.Size = UDim2.new(1 - 0, 0 + 0, 0 - 0, 889 - (464 + 395));
v128.Text = " 👥 観戦プレイヤーを選択 (自動更新)";
v128.TextColor3 = Color3.fromRGB(654 - 399, 123 + 132, 1092 - (467 + 370));
v128.Font = Enum.Font.SourceSansBold;
v128.TextSize = 28 - 14;
v128.BackgroundTransparency = 1;
v128.TextXAlignment = Enum.TextXAlignment.Left;
local v136 = Instance.new("ScrollingFrame", v125);
v136.Size = UDim2.new(1 + 0, -(34 - 24), 1 + 0, -(93 - 53));
v136.Position = UDim2.new(520 - (150 + 370), 1287 - (74 + 1208), 0 - 0, 165 - 130);
v136.BackgroundTransparency = 1;
v136.CanvasSize = UDim2.new(0 + 0, 0, 390 - (14 + 376), 0);
v136.ScrollBarThickness = 6 - 2;
local v142 = Instance.new("UIListLayout", v136);
v142.Padding = UDim.new(0 + 0, 5);
local function v144()
	for v818, v819 in pairs(v136:GetChildren()) do
		if v819:IsA("TextButton") then
			v819:Destroy();
		end
	end
	for v820, v821 in pairs(game.Players:GetPlayers()) do
		if (v821 ~= v1) then
			local v1069 = 0 + 0;
			local v1070;
			while true do
				if (v1069 == (3 + 0)) then
					v1070.TextSize = 40 - 26;
					Instance.new("UICorner", v1070);
					v1069 = 4;
				end
				if (1 == v1069) then
					v1070.BackgroundColor3 = Color3.fromRGB(40, 0 + 0, 78 - (23 + 55));
					v1070.Text = v821.DisplayName .. " (@" .. v821.Name .. ")";
					v1069 = 4 - 2;
				end
				if (v1069 == (3 + 1)) then
					v1070.MouseButton1Click:Connect(function()
						local v1407 = 0 + 0;
						while true do
							if (v1407 == 0) then
								v123 = v821.Name;
								v12("対象: " .. v821.DisplayName);
								v1407 = 1 - 0;
							end
							if ((1 + 0) == v1407) then
								v128.Text = " 👁️ 観戦中: " .. v821.DisplayName;
								break;
							end
						end
					end);
					break;
				end
				if (v1069 == (903 - (652 + 249))) then
					v1070.TextColor3 = Color3.fromRGB(255, 682 - 427, 255);
					v1070.Font = Enum.Font.SourceSans;
					v1069 = 1871 - (708 + 1160);
				end
				if (v1069 == 0) then
					v1070 = Instance.new("TextButton", v136);
					v1070.Size = UDim2.new(2 - 1, -(18 - 8), 27 - (10 + 17), 8 + 27);
					v1069 = 1733 - (1400 + 332);
				end
			end
		end
	end
	v136.CanvasSize = UDim2.new(0 - 0, 0, 1908 - (242 + 1666), v142.AbsoluteContentSize.Y);
end
game.Players.PlayerAdded:Connect(v144);
game.Players.PlayerRemoving:Connect(v144);
v144();
v103(v108, "スペクテイト有効化", false, function(v446)
	local v447 = 0 + 0;
	while true do
		if (v447 == (0 + 0)) then
			v122 = v446;
			if not v446 then
				v124.CameraSubject = v1.Character:FindFirstChildOfClass("Humanoid");
			end
			break;
		end
	end
end);
game:GetService("RunService").RenderStepped:Connect(function()
	if (v122 and v123) then
		local v929 = game.Players:FindFirstChild(v123);
		if (v929 and v929.Character and v929.Character:FindFirstChildOfClass("Humanoid")) then
			v124.CameraSubject = v929.Character:FindFirstChildOfClass("Humanoid");
		else
			local v1146 = 0 + 0;
			while true do
				if (v1146 == 0) then
					v124.CameraSubject = v1.Character:FindFirstChildOfClass("Humanoid");
					if v123 then
						v123 = nil;
						v128.Text = " 👥 観戦対象を選択";
						v12("対象がいなくなったため解除しました");
					end
					break;
				end
			end
		end
	end
end);
local v145 = false;
local v146 = 1140 - (850 + 90);
local v147 = game:GetService("RunService");
local function v148()
	local v448 = 0;
	local v449;
	while true do
		if (v448 == (0 - 0)) then
			if v145 then
				return;
			end
			if not v123 then
				v12("まず観戦リストからターゲットを選んでください");
				return;
			end
			v448 = 1;
		end
		if (1 == v448) then
			v145 = true;
			v12(v123 .. " への追従を開始 (Custom TP)");
			v448 = 1392 - (360 + 1030);
		end
		if (v448 == (3 + 0)) then
			task.spawn(function()
				local v1147;
				v1147 = v147.RenderStepped:Connect(function(v1242)
					local v1243 = 0;
					local v1244;
					local v1245;
					local v1246;
					while true do
						if (v1243 == (2 - 1)) then
							v1245 = v1.Character;
							v1246 = v1245 and v1245:FindFirstChild("HumanoidRootPart");
							v1243 = 2;
						end
						if (v1243 == (0 - 0)) then
							if not v145 then
								local v1626 = 1661 - (909 + 752);
								while true do
									if (0 == v1626) then
										v1147:Disconnect();
										return;
									end
								end
							end
							v1244 = game.Players:FindFirstChild(v123);
							v1243 = 1;
						end
						if (v1243 == 2) then
							if (v1244 and v1244.Character and v1244.Character:FindFirstChild("HumanoidRootPart") and v1246) then
								local v1627 = 1223 - (109 + 1114);
								local v1628;
								local v1629;
								local v1630;
								local v1631;
								local v1632;
								local v1633;
								local v1634;
								while true do
									if (v1627 == 3) then
										local v1741 = 0 - 0;
										while true do
											if (v1741 == 0) then
												v1633 = v1632.Magnitude;
												v1634 = v146 * v1242;
												v1741 = 1;
											end
											if ((1 + 0) == v1741) then
												v1627 = 246 - (6 + 236);
												break;
											end
										end
									end
									if (v1627 == (2 + 0)) then
										local v1742 = 0 + 0;
										while true do
											if (v1742 == (0 - 0)) then
												v1631 = v1246.Position;
												v1632 = v1630 - v1631;
												v1742 = 1 - 0;
											end
											if (v1742 == (1134 - (1076 + 57))) then
												v1627 = 1 + 2;
												break;
											end
										end
									end
									if (v1627 == (690 - (579 + 110))) then
										v1629 = v1628.CFrame * CFrame.new(0, 5, 1 + 2);
										v1630 = v1629.Position;
										v1627 = 2 + 0;
									end
									if (v1627 == (3 + 1)) then
										if (v1633 > 0.5) then
											if (v1633 < v1634) then
												v1246.CFrame = v1629;
											else
												local v1808 = v1631 + (v1632.Unit * v1634);
												v1246.CFrame = CFrame.lookAt(v1808, v1630);
											end
											v1246.Velocity = Vector3.zero;
											v1246.AssemblyLinearVelocity = Vector3.zero;
										end
										break;
									end
									if (v1627 == (407 - (174 + 233))) then
										v1628 = v1244.Character.HumanoidRootPart;
										v449();
										v1627 = 2 - 1;
									end
								end
							else
								local v1635 = 0 - 0;
								while true do
									if (v1635 == 0) then
										v145 = false;
										v1147:Disconnect();
										v1635 = 1 + 0;
									end
									if ((1175 - (663 + 511)) == v1635) then
										v12("ターゲットロスト / 停止");
										break;
									end
								end
							end
							break;
						end
					end
				end);
			end);
			break;
		end
		if (v448 == (2 + 0)) then
			local v1071 = 0 + 0;
			while true do
				if (v1071 == 0) then
					v449 = nil;
					function v449()
						if v1.Character then
							for v1636, v1637 in pairs(v1.Character:GetDescendants()) do
								if (v1637:IsA("BasePart") and (v1637.CanCollide == true)) then
									v1637.CanCollide = false;
								end
							end
						end
					end
					v1071 = 1;
				end
				if (v1071 == (2 - 1)) then
					v448 = 2 + 1;
					break;
				end
			end
		end
	end
end
local v149 = Instance.new("Frame", v108);
v149.Size = UDim2.new(2 - 1, -(24 - 14), 0 + 0, 194 - 94);
v149.BackgroundTransparency = 1;
local v152 = Instance.new("TextButton", v149);
v152.Size = UDim2.new(0.48, 0 + 0, 0 + 0, 40);
v152.BackgroundColor3 = Color3.fromRGB(0, 80, 722 - (478 + 244));
v152.Text = "疑似Tween開始";
v152.TextColor3 = Color3.fromRGB(255, 772 - (440 + 77), 116 + 139);
Instance.new("UICorner", v152);
local v157 = Instance.new("TextButton", v149);
v157.Size = UDim2.new(0.48, 0 - 0, 1556 - (655 + 901), 8 + 32);
v157.Position = UDim2.new(0.52 + 0, 0 + 0, 0 - 0, 0);
v157.BackgroundColor3 = Color3.fromRGB(1525 - (695 + 750), 0 - 0, 0);
v157.Text = "停止";
v157.TextColor3 = Color3.fromRGB(255, 393 - 138, 255);
Instance.new("UICorner", v157);
local v163 = Instance.new("Frame", v149);
v163.Size = UDim2.new(3 - 2, 351 - (285 + 66), 0 - 0, 1360 - (682 + 628));
v163.Position = UDim2.new(0 + 0, 0, 299 - (176 + 123), 19 + 26);
v163.BackgroundTransparency = 1 + 0;
v104(v163, "追従スピード", 369 - (239 + 30), 96 + 254, v146, function(v450)
	v146 = v450;
end);
v152.MouseButton1Click:Connect(function()
	v148();
end);
v157.MouseButton1Click:Connect(function()
	local v451 = 0;
	while true do
		if (v451 == 0) then
			v145 = false;
			v12("追従を停止しました");
			break;
		end
	end
end);
v9.SpeedMultiplier = 1 + 0;
game:GetService("RunService").Heartbeat:Connect(function()
	local v452 = 0 - 0;
	local v453;
	while true do
		if ((0 - 0) == v452) then
			v453 = v1.Character;
			if v453 then
				v453:SetAttribute("SpeedMultiplier", v9.SpeedMultiplier);
			end
			break;
		end
	end
end);
v104(v108, "スピード", 316 - (306 + 9), 3489 - 2489, v9.SpeedMultiplier, function(v454)
	local v455 = 0 + 0;
	local v456;
	while true do
		if (v455 == (1 + 0)) then
			if v456 then
				v456:SetAttribute("SpeedMultiplier", v454);
			end
			break;
		end
		if (v455 == (0 + 0)) then
			v9.SpeedMultiplier = v454;
			v456 = v1.Character;
			v455 = 2 - 1;
		end
	end
end);
v9.DashLength = 10;
game:GetService("RunService").Heartbeat:Connect(function()
	local v457 = v1.Character;
	if v457 then
		v457:SetAttribute("DashLength", v9.DashLength);
	end
end);
v104(v108, "ダッシュ", 10, 1000, v9.DashLength, function(v458)
	local v459 = 0;
	local v460;
	while true do
		if ((1375 - (1140 + 235)) == v459) then
			v9.DashLength = v458;
			v460 = v1.Character;
			v459 = 1;
		end
		if (v459 == 1) then
			if v460 then
				v460:SetAttribute("DashLength", v458);
			end
			break;
		end
	end
end);
_G.JumpHeightValue = 32 + 18;
_G.AutoJumpEnabled = true;
game:GetService("RunService").Heartbeat:Connect(function()
	if _G.AutoJumpEnabled then
		pcall(function()
			local v1077 = game.Players.LocalPlayer.Character;
			local v1078 = v1077 and v1077:FindFirstChildOfClass("Humanoid");
			if v1078 then
				v1078.UseJumpPower = true;
				v1078.JumpPower = _G.JumpHeightValue;
			end
		end);
	end
end);
v104(v108, "ジャンプ力", 46 + 4, 129 + 371, _G.JumpHeightValue, function(v461)
	local v462 = 0;
	while true do
		if (v462 == (53 - (33 + 19))) then
			pcall(function()
				local v1148 = 0 + 0;
				local v1149;
				while true do
					if (v1148 == (0 - 0)) then
						v1149 = game.Players.LocalPlayer.Character:FindFirstChildOfClass("Humanoid");
						if v1149 then
							local v1540 = 0 + 0;
							local v1541;
							while true do
								if (v1540 == (0 - 0)) then
									v1541 = 0 + 0;
									while true do
										if (v1541 == (689 - (586 + 103))) then
											v1149.UseJumpPower = true;
											v1149.JumpPower = v461;
											break;
										end
									end
									break;
								end
							end
						end
						break;
					end
				end
			end);
			break;
		end
		if (v462 == (0 + 0)) then
			_G.JumpHeightValue = v461;
			_G.AutoJumpEnabled = true;
			v462 = 2 - 1;
		end
	end
end);
v9.BangKey = "G";
v9.TpKey = "U";
v9.BangEnabled = false;
v9.TpEnabled = false;
local v173 = false;
local v174 = tick();
local v175 = nil;
local v124 = workspace.CurrentCamera;
local v176 = v1:GetMouse();
local function v177(v463)
	local v464, v465 = pcall(function()
		return Enum.KeyCode[v463:upper()];
	end);
	return (v464 and v465) or nil;
end
local function v178(v466, v467, v468, v469)
	local v470 = Instance.new("Frame", v466);
	v470.Size = UDim2.new(1, -10, 1488 - (1309 + 179), 45);
	v470.BackgroundColor3 = Color3.fromRGB(25, 0 - 0, 0 + 0);
	Instance.new("UICorner", v470);
	local v473 = Instance.new("TextLabel", v470);
	v473.Size = UDim2.new(0 - 0, 114 + 36, 1 - 0, 0 - 0);
	v473.Position = UDim2.new(609 - (295 + 314), 10, 0 - 0, 1962 - (1300 + 662));
	v473.Text = v467;
	v473.TextColor3 = Color3.fromRGB(800 - 545, 2010 - (1178 + 577), 133 + 122);
	v473.Font = Enum.Font.SourceSansBold;
	v473.TextSize = 16;
	v473.BackgroundTransparency = 2 - 1;
	v473.TextXAlignment = Enum.TextXAlignment.Left;
	local v484 = Instance.new("TextBox", v470);
	v484.Size = UDim2.new(0, 1455 - (851 + 554), 0, 27 + 3);
	v484.Position = UDim2.new(2 - 1, -(130 - 70), 302.5 - (115 + 187), -15);
	v484.BackgroundColor3 = Color3.fromRGB(40, 0, 0 + 0);
	v484.Text = v468;
	v484.TextColor3 = Color3.fromRGB(242 + 13, 1004 - 749, 1416 - (160 + 1001));
	v484.Font = Enum.Font.SourceSansBold;
	v484.TextSize = 16;
	Instance.new("UICorner", v484);
	v484.FocusLost:Connect(function()
		local v822 = 0 + 0;
		while true do
			if ((0 + 0) == v822) then
				v469(v484.Text);
				v12(v467 .. "を [" .. v484.Text:upper() .. "] に設定");
				break;
			end
		end
	end);
end
v178(v106, "BANG起動キー設定", v9.BangKey, function(v492)
	v9.BangKey = v492:upper();
end);
v178(v106, "クリックTPキー設定", v9.TpKey, function(v494)
	v9.TpKey = v494:upper();
end);
v103(v106, "BANG機能 有効化", false, function(v496)
	local v497 = 0 - 0;
	while true do
		if (v497 == 0) then
			v9.BangEnabled = v496;
			if not v496 then
				v173 = false;
			end
			break;
		end
	end
end);
v2.InputBegan:Connect(function(v498, v499)
	if v499 then
		return;
	end
	if ((v498.UserInputType == Enum.UserInputType.MouseButton1) and v2:IsKeyDown(Enum.KeyCode.LeftControl)) then
		local v930 = 358 - (237 + 121);
		local v931;
		local v932;
		local v933;
		while true do
			if (v930 == (898 - (525 + 372))) then
				for v1337, v1338 in pairs(game.Players:GetPlayers()) do
					if ((v1338 ~= v1) and v1338.Character and v1338.Character:FindFirstChild("HumanoidRootPart")) then
						local v1475, v1476 = v124:WorldToViewportPoint(v1338.Character.HumanoidRootPart.Position);
						if v1476 then
							local v1638 = 0;
							local v1639;
							while true do
								if (v1638 == (0 - 0)) then
									v1639 = (Vector2.new(v1475.X, v1475.Y) - v931).Magnitude;
									if (v1639 < v933) then
										local v1781 = 0;
										while true do
											if ((0 - 0) == v1781) then
												v933 = v1639;
												v932 = v1338;
												break;
											end
										end
									end
									break;
								end
							end
						end
					end
				end
				if v932 then
					local v1409 = 0;
					local v1410;
					while true do
						if (v1409 == (142 - (96 + 46))) then
							v1410 = 0;
							while true do
								if ((777 - (643 + 134)) == v1410) then
									v175 = v932;
									v12("ターゲット確定: " .. v932.DisplayName);
									break;
								end
							end
							break;
						end
					end
				else
					v12("近くにプレイヤーがいません");
				end
				break;
			end
			if (v930 == (0 + 0)) then
				v931 = v2:GetMouseLocation();
				v932, v933 = nil, 250;
				v930 = 2 - 1;
			end
		end
	end
	local v500 = v177(v9.BangKey);
	local v501 = v177(v9.TpKey);
	if (v500 and (v498.KeyCode == v500)) then
		local v934 = 0;
		while true do
			if (v934 == (0 - 0)) then
				v9.BangEnabled = not v9.BangEnabled;
				v12("BANG: " .. ((v9.BangEnabled and "ON") or "OFF"));
				break;
			end
		end
	elseif (v501 and (v498.KeyCode == v501)) then
		local v1150 = 0 + 0;
		while true do
			if ((0 - 0) == v1150) then
				v9.TpEnabled = not v9.TpEnabled;
				v12("クリックTP: " .. ((v9.TpEnabled and "ON") or "OFF"));
				break;
			end
		end
	end
end);
game:GetService("RunService").Heartbeat:Connect(function()
	if (v9.BangEnabled and v175 and v175.Character) then
		local v935 = 0 - 0;
		local v936;
		local v937;
		local v938;
		while true do
			if (1 == v935) then
				v938 = nil;
				while true do
					if (v936 == (720 - (316 + 403))) then
						if (v937 and v938 and ((tick() - v174) >= 0.2)) then
							v937.CFrame = v938.CFrame * CFrame.new(0 + 0, 0 - 0, 3);
						end
						break;
					end
					if (v936 == (0 + 0)) then
						v937 = v1.Character and v1.Character:FindFirstChild("HumanoidRootPart");
						v938 = v175.Character:FindFirstChild("HumanoidRootPart");
						v936 = 2 - 1;
					end
				end
				break;
			end
			if (v935 == (0 + 0)) then
				v936 = 0 + 0;
				v937 = nil;
				v935 = 3 - 2;
			end
		end
	end
end);
v176.Button1Down:Connect(function()
	if (v9.BangEnabled and v9.TpEnabled and v175) then
		local v939 = v175.Character and v175.Character:FindFirstChild("HumanoidRootPart");
		if v939 then
			local v1151 = 0;
			local v1152;
			local v1153;
			while true do
				if (v1151 == (4 - 3)) then
					v1.Character.HumanoidRootPart.CFrame = CFrame.new(v939.Position + v1153);
					v174 = tick();
					break;
				end
				if (v1151 == 0) then
					local v1413 = 0 - 0;
					while true do
						if (v1413 == 1) then
							v1151 = 1 + 0;
							break;
						end
						if (v1413 == (0 - 0)) then
							v1152 = math.random() * (1 + 1) * math.pi;
							v1153 = Vector3.new(math.cos(v1152) * 300, 14 - 9, math.sin(v1152) * 300);
							v1413 = 18 - (12 + 5);
						end
					end
				end
			end
		end
	end
end);
local v179 = {};
local v180 = workspace:FindFirstChild("Boats");
local function v181()
	local v502 = 0 - 0;
	local v503;
	local v504;
	local v505;
	local v506;
	while true do
		if (v502 == 1) then
			if (not v504 or not v504.SeatPart or not v180) then
				return nil, {};
			end
			v505 = nil;
			v502 = 2;
		end
		if (v502 == 2) then
			for v1154, v1155 in ipairs(v180:GetChildren()) do
				if v504.SeatPart:IsDescendantOf(v1155) then
					v505 = v1155;
					break;
				end
			end
			v506 = {};
			v502 = 3;
		end
		if (v502 == (5 - 2)) then
			if v505 then
				for v1339, v1340 in ipairs(v505:GetDescendants()) do
					if ((v1340:IsA("Seat") or v1340:IsA("VehicleSeat")) and (v1340 ~= v504.SeatPart) and (v1340.Occupant == nil)) then
						table.insert(v506, v1340);
					end
				end
			end
			return v505, v506;
		end
		if (v502 == 0) then
			v503 = v1.Character;
			v504 = v503 and v503:FindFirstChildOfClass("Humanoid");
			v502 = 1;
		end
	end
end
local v182 = Instance.new("Frame", v108);
v182.Size = UDim2.new(1 - 0, -(24 - 14), 0, 41 + 159);
v182.BackgroundColor3 = Color3.fromRGB(1993 - (1656 + 317), 20, 23 + 2);
Instance.new("UICorner", v182);
local v185 = Instance.new("TextLabel", v182);
v185.Size = UDim2.new(1, 0, 0 + 0, 79 - 49);
v185.Text = " 🚢 Target Slots (ボート空き枠)";
v185.TextColor3 = Color3.fromRGB(255, 255, 1254 - 999);
v185.Font = Enum.Font.SourceSansBold;
v185.TextSize = 14;
v185.BackgroundTransparency = 1;
v185.TextXAlignment = Enum.TextXAlignment.Left;
local v193 = Instance.new("ScrollingFrame", v182);
v193.Size = UDim2.new(355 - (5 + 349), -(47 - 37), 1272 - (266 + 1005), -75);
v193.Position = UDim2.new(0, 4 + 1, 0 - 0, 46 - 11);
v193.BackgroundTransparency = 1697 - (561 + 1135);
v193.ScrollBarThickness = 5 - 1;
local v198 = Instance.new("UIListLayout", v193);
v198.Padding = UDim.new(0, 16 - 11);
local function v200()
	local v507 = 0;
	local v508;
	local v509;
	local v510;
	while true do
		if (v507 == (1068 - (507 + 559))) then
			for v1156, v1157 in ipairs(game.Players:GetPlayers()) do
				if (v1157 ~= v1) then
					local v1341 = 0 - 0;
					local v1342;
					local v1343;
					while true do
						if (v1341 == 1) then
							v1343.Size = UDim2.new(3 - 2, -(398 - (212 + 176)), 905 - (250 + 655), 30);
							v1343.Text = v1157.DisplayName;
							v1341 = 2;
						end
						if (v1341 == (5 - 3)) then
							v1343.TextColor3 = Color3.fromRGB(255, 445 - 190, 398 - 143);
							v1343.BackgroundColor3 = (v1342 and Color3.fromRGB(2106 - (1869 + 87), 0 - 0, 1901 - (484 + 1417))) or Color3.fromRGB(85 - 45, 67 - 27, 813 - (48 + 725));
							v1341 = 4 - 1;
						end
						if ((0 - 0) == v1341) then
							v1342 = table.find(v179, v1157);
							v1343 = Instance.new("TextButton", v193);
							v1341 = 1 + 0;
						end
						if (v1341 == (7 - 4)) then
							Instance.new("UICorner", v1343);
							v1343.MouseButton1Click:Connect(function()
								local v1641 = 0 + 0;
								local v1642;
								while true do
									if (v1641 == (1 + 0)) then
										v200();
										break;
									end
									if (v1641 == (853 - (152 + 701))) then
										v1642 = table.find(v179, v1157);
										if v1642 then
											table.remove(v179, v1642);
										elseif (#v179 < v510) then
											table.insert(v179, v1157);
										else
											v12("空き席が足りません！");
										end
										v1641 = 1;
									end
								end
							end);
							break;
						end
					end
				end
			end
			v193.CanvasSize = UDim2.new(0, 1311 - (430 + 881), 0 + 0, v198.AbsoluteContentSize.Y);
			break;
		end
		if (v507 == 1) then
			v185.Text = " 🚢 Target Slots: " .. #v179 .. " / " .. v510;
			for v1158, v1159 in ipairs(v193:GetChildren()) do
				if v1159:IsA("TextButton") then
					v1159:Destroy();
				end
			end
			v507 = 2;
		end
		if (v507 == 0) then
			v508, v509 = v181();
			v510 = #v509;
			v507 = 896 - (557 + 338);
		end
	end
end
local v201 = Instance.new("TextButton", v182);
v201.Size = UDim2.new(0.9, 0 + 0, 0 - 0, 122 - 87);
v201.Position = UDim2.new(0.05 - 0, 0 - 0, 802 - (499 + 302), -40);
v201.BackgroundColor3 = Color3.fromRGB(866 - (39 + 827), 276 - 176, 0 - 0);
v201.Text = "ボートハメ込みTP開始";
v201.TextColor3 = Color3.fromRGB(1012 - 757, 255, 255);
Instance.new("UICorner", v201);
v201.MouseButton1Click:Connect(function()
	local v511 = 0;
	local v512;
	local v513;
	while true do
		if (v511 == 1) then
			v12("テレポートを開始します...");
			for v1160, v1161 in ipairs(v179) do
				local v1162 = v513[v1160];
				local v1163 = v1161.Character and v1161.Character:FindFirstChild("HumanoidRootPart");
				if (v1162 and v1163) then
					local v1344 = 0 - 0;
					local v1345;
					local v1346;
					local v1347;
					while true do
						if (v1344 == (0 + 0)) then
							v1345 = 0 - 0;
							v1346 = nil;
							v1344 = 1 + 0;
						end
						if (v1344 == (1 - 0)) then
							v1347 = nil;
							while true do
								if (v1345 == 1) then
									v512:PivotTo(v1347);
									task.wait(104.3 - (103 + 1));
									break;
								end
								if (v1345 == (554 - (475 + 79))) then
									v1346 = v512:GetPivot():Inverse() * v1162.CFrame;
									v1347 = v1163.CFrame * v1346:Inverse();
									v1345 = 1;
								end
							end
							break;
						end
					end
				end
			end
			v511 = 4 - 2;
		end
		if (v511 == (9 - 6)) then
			v12("全ターゲットの処理が完了しました");
			break;
		end
		if (v511 == (1 + 1)) then
			v179 = {};
			v200();
			v511 = 3 + 0;
		end
		if (v511 == (1503 - (1395 + 108))) then
			v512, v513 = v181();
			if (not v512 or (#v179 == (0 - 0))) then
				local v1250 = 1204 - (7 + 1197);
				while true do
					if (v1250 == (0 + 0)) then
						v12("ボートに乗っていないか、対象を選んでいません");
						return;
					end
				end
			end
			v511 = 1 + 0;
		end
	end
end);
game.Players.PlayerAdded:Connect(v200);
game.Players.PlayerRemoving:Connect(v200);
v200();
local function v207(v514)
	local v515 = 319 - (27 + 292);
	local v516;
	local v517;
	while true do
		if ((2 - 1) == v515) then
			if v516 then
				v516:Destroy();
			end
			v517 = v514:WaitForChild("Humanoid", 6 - 1);
			v515 = 8 - 6;
		end
		if (v515 == (0 - 0)) then
			if not v514 then
				return;
			end
			v516 = v514:WaitForChild("Animate", 5);
			v515 = 1 - 0;
		end
		if (v515 == (141 - (43 + 96))) then
			if v517 then
				local v1251 = 0 - 0;
				while true do
					if (v1251 == (0 - 0)) then
						for v1547, v1548 in pairs(v517:GetPlayingAnimationTracks()) do
							v1548:Stop(0);
						end
						v517.AnimationPlayed:Connect(function(v1549)
							v1549:Stop(0);
						end);
						break;
					end
				end
			end
			break;
		end
	end
end
v105(v106, "アニメーション無効化", function()
	local v518 = 0 + 0;
	while true do
		if (v518 == 0) then
			if v1.Character then
				v207(v1.Character);
			end
			v1.CharacterAdded:Connect(v207);
			v518 = 1;
		end
		if (1 == v518) then
			v12("アニメーションを完全に削除しました");
			break;
		end
	end
end);
local function v208()
	local v519 = game:GetService("Lighting");
	local v520 = game:GetService("Workspace");
	local function v521(v823)
		local v824 = 0 + 0;
		while true do
			if (v824 == (0 - 0)) then
				if (v823:IsA("Sound") or v823:IsA("SoundGroup")) then
					return;
				end
				pcall(function()
					if (v823:IsA("ParticleEmitter") or v823:IsA("Smoke") or v823:IsA("Fire") or v823:IsA("Sparkles")) then
						local v1414 = 0 + 0;
						local v1415;
						while true do
							if (v1414 == (0 - 0)) then
								v1415 = 0;
								while true do
									if (v1415 == (0 + 0)) then
										v823.Transparency = NumberSequence.new(0.99 + 0);
										if v823:IsA("ParticleEmitter") then
											v823.Rate = v823.Rate * (1751.01 - (1414 + 337));
										end
										break;
									end
								end
								break;
							end
						end
					elseif (v823:IsA("Trail") or v823:IsA("Beam")) then
						v823.Transparency = 1940.99 - (1642 + 298);
					elseif (v823:IsA("Decal") or v823:IsA("Texture")) then
						if (v823.Name ~= "face") then
							v823.Transparency = 0.98 - 0;
						end
					elseif (v823:IsA("PostEffect") or v823:IsA("ColorCorrectionEffect") or v823:IsA("BloomEffect") or v823:IsA("BlurEffect") or v823:IsA("SunRaysEffect")) then
						v823.Enabled = false;
					elseif (v823:IsA("BasePart") or v823:IsA("MeshPart")) then
						local v1783 = 0;
						local v1784;
						while true do
							if (v1783 == (0 - 0)) then
								v1784 = 0 - 0;
								while true do
									if (v1784 == (0 + 0)) then
										v823.CastShadow = false;
										v823.Reflectance = 0 + 0;
										v1784 = 1;
									end
									if (v1784 == 1) then
										v823.Material = Enum.Material.SmoothPlastic;
										break;
									end
								end
								break;
							end
						end
					end
				end);
				break;
			end
		end
	end
	for v825, v826 in pairs(game:GetDescendants()) do
		v521(v826);
	end
	v520.DescendantAdded:Connect(v521);
	v519.GlobalShadows = false;
	v519.FogEnd = 9000000460 - (357 + 615);
	pcall(function()
		v9().Rendering.QualityLevel = Enum.QualityLevel.Level01;
	end);
	v12("FPS Boost有効");
end
v105(v106, "FPS Boost", function()
	v208();
end);
local function v209()
	local v524 = game:GetService("Lighting");
	local v525 = game:GetService("Workspace");
	local v526 = v525.Terrain;
	local v527 = game:GetService("RunService");
	v524.GlobalShadows = true;
	v524.ShadowSoftness = 0;
	v524.Brightness = 1.8;
	v524.EnvironmentDiffuseScale = 1;
	v524.EnvironmentSpecularScale = 1 + 0;
	v524.ExposureCompensation = 0.1;
	local v534 = v526:FindFirstChildOfClass("Clouds") or Instance.new("Clouds", v526);
	v534.Enabled = true;
	v534.Cover = 0.62 - 0;
	v534.Density = 0.75;
	pcall(function()
		v527:UnbindFromRenderStep("ZenithCloudDrift");
	end);
	local v538 = 0;
	v527:BindToRenderStep("ZenithCloudDrift", Enum.RenderPriority.Last.Value, function(v829)
		local v830 = 0 + 0;
		while true do
			if (0 == v830) then
				v538 = v538 + v829;
				v534.Cover = (0.62 - 0) + (math.sin(v538 * 0.15) * 0.015);
				break;
			end
		end
	end);
	for v831, v832 in pairs(v525:GetDescendants()) do
		pcall(function()
			if (v832:IsA("BasePart") or v832:IsA("MeshPart")) then
				local v1165 = 0;
				while true do
					if ((0 + 0) == v1165) then
						v832.CastShadow = true;
						if (v832.Reflectance < 0.15) then
							v832.Reflectance = 0.22 + 0;
						end
						v1165 = 1 + 0;
					end
					if (v1165 == (1302 - (384 + 917))) then
						if ((v832.Material == Enum.Material.SmoothPlastic) or (v832.Material == Enum.Material.Glass)) then
							v832.Reflectance = 0.35;
						end
						break;
					end
				end
			end
		end);
	end
	local function v539(v833)
		if v833:IsA("BloomEffect") then
			local v1083 = 0;
			while true do
				if ((698 - (128 + 569)) == v1083) then
					v833.Threshold = 0.9;
					break;
				end
				if (v1083 == (1543 - (1407 + 136))) then
					v833.Intensity = 1887.35 - (687 + 1200);
					v833.Size = 1734 - (556 + 1154);
					v1083 = 1;
				end
			end
		elseif v833:IsA("SunRaysEffect") then
			v833.Intensity = 0.06;
		elseif v833:IsA("Atmosphere") then
			local v1417 = 0;
			while true do
				if (v1417 == (3 - 2)) then
					v833.Haze = 95.8 - (9 + 86);
					break;
				end
				if (v1417 == 0) then
					v833.Density = 421.28 - (275 + 146);
					v833.Glare = 0.4 + 0;
					v1417 = 65 - (29 + 35);
				end
			end
		end
	end
	for v834, v835 in pairs(v524:GetChildren()) do
		v539(v835);
	end
	v524.ChildAdded:Connect(v539);
	if not v524:FindFirstChildOfClass("Atmosphere") then
		local v940 = Instance.new("Atmosphere", v524);
		v940.Density = 0.28;
		v940.Glare = 0.4;
		v940.Haze = 0.8 - 0;
	end
	local v540 = v524:FindFirstChild("ZenithBlurV2") or Instance.new("BlurEffect", v524);
	v540.Name = "ZenithBlurV2";
	local v542 = v525.CurrentCamera.CFrame;
	pcall(function()
		v527:UnbindFromRenderStep("ZenithDynamicBlur");
	end);
	v527:BindToRenderStep("ZenithDynamicBlur", Enum.RenderPriority.Camera.Value + (2 - 1), function()
		local v836 = v525.CurrentCamera;
		local v837 = (v836.CFrame.Position - v542.Position).Magnitude;
		local v838 = (v836.CFrame.LookVector - v542.LookVector).Magnitude;
		local v839 = math.min((v837 * 2) + (v838 * 40), 10);
		v540.Size = v540.Size + ((v839 - v540.Size) * 0.2);
		v542 = v836.CFrame;
	end);
	v12("RTX適用完了");
end
v105(v106, "RTX", function()
	v209();
end);
local v210 = game:GetService("Players");
local v147 = game:GetService("RunService");
local v211 = v210.LocalPlayer;
local v212 = workspace.CurrentCamera;
if _G.ESPConnection then
	_G.ESPConnection:Disconnect();
end
if _G.ESPObjects then
	for v944, v945 in pairs(_G.ESPObjects) do
		for v1084, v1085 in pairs(v945) do
			pcall(function()
				v1085:Remove();
			end);
		end
	end
end
_G.ESPObjects = {};
_G.ESPEnabled = false;
local function v213(v543)
	local v544 = v543.Character;
	local v545 = v544 and v544:FindFirstChild("HumanoidRootPart");
	if not v545 then
		return false;
	end
	local v546 = workspace:FindFirstChild("_WorldOrigin") and workspace._WorldOrigin:FindFirstChild("SafeZones");
	if not v546 then
		return false;
	end
	for v842, v843 in pairs(v546:GetChildren()) do
		if v843:IsA("BasePart") then
			local v1086 = 0 - 0;
			local v1087;
			local v1088;
			local v1089;
			local v1090;
			while true do
				if ((1 + 0) == v1086) then
					if v1089 then
						v1088 = v1088 * v1089.Scale;
					end
					v1090 = v545.Position;
					v1086 = 2;
				end
				if (v1086 == 2) then
					if ((v1090.X >= (v1087.X - (v1088.X / 2))) and (v1090.X <= (v1087.X + (v1088.X / 2))) and (v1090.Z >= (v1087.Z - (v1088.Z / 2))) and (v1090.Z <= (v1087.Z + (v1088.Z / (1014 - (53 + 959)))))) then
						return true;
					end
					break;
				end
				if ((408 - (312 + 96)) == v1086) then
					local v1352 = 0 - 0;
					while true do
						if (v1352 == 1) then
							v1086 = 1;
							break;
						end
						if (v1352 == (285 - (147 + 138))) then
							v1087, v1088 = v843.Position, v843.Size;
							v1089 = v843:FindFirstChildOfClass("SpecialMesh");
							v1352 = 900 - (813 + 86);
						end
					end
				end
			end
		end
	end
	return false;
end
local function v214(v547)
	return (v547:GetAttribute("KenActive") == true) or (v547:FindFirstChild("KenActive", true) and (v547:FindFirstChild("KenActive", true).Value == true));
end
local function v215(v548)
	if (not v548 or (type(v548) ~= "number")) then
		return "0";
	end
	if (v548 >= 1000000) then
		return string.format("%.1fM", v548 / 1000000);
	elseif (v548 >= (904 + 96)) then
		return string.format("%.1fk", v548 / (1852 - 852));
	else
		return tostring(v548);
	end
end
local function v216(v549)
	local v550 = 0;
	local v551;
	while true do
		if (v550 == (493 - (18 + 474))) then
			function v551(v1166, v1167)
				local v1168 = 0;
				local v1169;
				while true do
					if (v1168 == (2 + 1)) then
						return v1169;
					end
					if (v1168 == (3 - 2)) then
						v1169.Color = v1167;
						v1169.Center = true;
						v1168 = 1088 - (860 + 226);
					end
					if (v1168 == (305 - (121 + 182))) then
						v1169.Outline = true;
						v1169.Visible = false;
						v1168 = 1 + 2;
					end
					if (v1168 == 0) then
						v1169 = Drawing.new("Text");
						v1169.Size = v1166;
						v1168 = 1;
					end
				end
			end
			_G.ESPObjects[v549] = {Line=Drawing.new("Line"),NameText=v551(1256 - (988 + 252), Color3.new(1, 1 + 0, 1 + 0)),PvpText=v551(1984 - (49 + 1921), Color3.new(891 - (223 + 667), 53 - (51 + 1), 1)),KenText=v551(23 - 9, Color3.new(1 - 0, 0, 1126 - (146 + 979))),StatText=v551(4 + 9, Color3.new(606 - (311 + 294), 0.8, 0)),HPText=v551(13, Color3.new(0, 2 - 1, 0 + 0))};
			break;
		end
		if ((1443 - (496 + 947)) == v550) then
			if (v549 == v211) then
				return;
			end
			v551 = nil;
			v550 = 1359 - (1233 + 125);
		end
	end
end
for v552, v553 in ipairs(v210:GetPlayers()) do
	v216(v553);
end
v210.PlayerAdded:Connect(v216);
_G.ESPConnection = v147.RenderStepped:Connect(function()
	for v844, v845 in pairs(_G.ESPObjects) do
		if not _G.ESPEnabled then
			for v1170, v1171 in pairs(v845) do
				v1171.Visible = false;
			end
			continue;
		end
		local v846 = v844.Character;
		local v847 = v846 and v846:FindFirstChild("HumanoidRootPart");
		local v848 = v846 and v846:FindFirstChildOfClass("Humanoid");
		if (v847 and v848) then
			local v1091, v1092 = v212:WorldToViewportPoint(v847.Position);
			if v1092 then
				local v1253 = 0 + 0;
				local v1254;
				local v1255;
				local v1256;
				local v1257;
				local v1258;
				local v1259;
				local v1260;
				while true do
					if (v1253 == (3 + 0)) then
						v1260 = (v1256 and "PvP: OFF") or "PvP: ON";
						if v1255 then
							local v1646 = 0 + 0;
							local v1647;
							while true do
								if (v1646 == 0) then
									v1647 = 1645 - (963 + 682);
									while true do
										if (v1647 == (0 + 0)) then
											v1260 = v1260 .. " (SAFE)";
											v845.PvpText.Color = Color3.new(1504 - (504 + 1000), 1 + 0, 1 + 0);
											break;
										end
									end
									break;
								end
							end
						else
							v845.PvpText.Color = (v1256 and Color3.new(0.7 + 0, 0.7, 0.7 - 0)) or Color3.new(1 + 0, 0, 0 + 0);
						end
						v845.PvpText.Text = v1260;
						v845.PvpText.Position = Vector2.new(v1091.X, v1091.Y - 65);
						v1253 = 186 - (156 + 26);
					end
					if (1 == v1253) then
						v1258 = v844:FindFirstChild("leaderstats");
						v1259 = v1258 and v1258:FindFirstChild("Bounty/Honor");
						v845.Line.From = Vector2.new(v212.ViewportSize.X / (2 + 0), v212.ViewportSize.Y);
						v845.Line.To = Vector2.new(v1091.X, v1091.Y);
						v1253 = 2 - 0;
					end
					if (v1253 == (168 - (149 + 15))) then
						v845.PvpText.Visible = true;
						v845.KenText.Text = (v1257 and "● 見聞あり ●") or "○ 見聞なし ○";
						v845.KenText.Position = Vector2.new(v1091.X, v1091.Y - (1010 - (890 + 70)));
						v845.KenText.Visible = true;
						v1253 = 122 - (39 + 78);
					end
					if ((487 - (14 + 468)) == v1253) then
						v845.StatText.Text = (v1259 and ("Bounty: " .. v215(v1259.Value))) or "";
						v845.StatText.Position = Vector2.new(v1091.X, v1091.Y - 35);
						v845.StatText.Visible = true;
						v845.HPText.Text = "HP: " .. math.floor(v848.Health);
						v1253 = 13 - 7;
					end
					if (v1253 == (16 - 10)) then
						v845.HPText.Position = Vector2.new(v1091.X, v1091.Y - (11 + 9));
						v845.HPText.Visible = true;
						break;
					end
					if ((2 + 0) == v1253) then
						v845.Line.Visible = true;
						v845.NameText.Text = string.format("%s [%dm]", v844.DisplayName, v1254);
						v845.NameText.Position = Vector2.new(v1091.X, v1091.Y - 80);
						v845.NameText.Visible = true;
						v1253 = 1 + 2;
					end
					if (v1253 == 0) then
						v1254 = math.floor((v847.Position - v212.CFrame.Position).Magnitude);
						v1255 = v213(v844);
						v1256 = v844:GetAttribute("PvpDisabled");
						v1257 = v214(v844);
						v1253 = 1;
					end
				end
			else
				for v1353, v1354 in pairs(v845) do
					v1354.Visible = false;
				end
			end
		else
			for v1173, v1174 in pairs(v845) do
				v1174.Visible = false;
			end
		end
	end
end);
v103(v106, "ESP", false, function(v554)
	_G.ESPEnabled = v554;
end);
task.spawn(function()
	local v555 = Vector3.new(439.4629 + 531, 67.02590000000001 + 185, 32872.1875);
	local v556 = Vector3.new(-(545.2947082519531 - 260), 302.8865966796875 + 3, 2073.4352416992188 - 1483);
	if not _G.NebulaSettings then
		_G.NebulaSettings = {};
	end
	_G.NebulaSettings.GhostShipKey = _G.NebulaSettings.GhostShipKey or "H";
	_G.NebulaSettings.MansionKey = _G.NebulaSettings.MansionKey or "V";
	local v557 = false;
	local v558 = false;
	local function v559(v849, v850)
		local v851 = game.Players.LocalPlayer.Character;
		local v852 = v851 and v851:FindFirstChild("HumanoidRootPart");
		if v852 then
			v852.CFrame = CFrame.new(v849);
			v12(v850 .. " へテレポートしました");
		else
			v12("キャラクターが見つかりません");
		end
	end
	game:GetService("UserInputService").InputBegan:Connect(function(v853, v854)
		local v855 = 0;
		while true do
			if (v855 == 0) then
				if v854 then
					return;
				end
				if v557 then
					local v1356 = 0 + 0;
					while true do
						if (v1356 == 0) then
							_G.NebulaSettings.GhostShipKey = v853.KeyCode.Name;
							v557 = false;
							v1356 = 52 - (12 + 39);
						end
						if (1 == v1356) then
							local v1556 = 0;
							while true do
								if (v1556 == 0) then
									v12("幽霊船キーを " .. v853.KeyCode.Name .. " に設定しました");
									return;
								end
							end
						end
					end
				end
				v855 = 1 + 0;
			end
			if (v855 == (2 - 1)) then
				if v558 then
					local v1357 = 0;
					while true do
						if (v1357 == 0) then
							_G.NebulaSettings.MansionKey = v853.KeyCode.Name;
							v558 = false;
							v1357 = 3 - 2;
						end
						if (v1357 == (1 + 0)) then
							v12("マンションキーを " .. v853.KeyCode.Name .. " に設定しました");
							return;
						end
					end
				end
				if (v853.KeyCode.Name == _G.NebulaSettings.GhostShipKey) then
					v559(v555, "幽霊船");
				elseif (v853.KeyCode.Name == _G.NebulaSettings.MansionKey) then
					v559(v556, "マンション");
				end
				break;
			end
		end
	end);
	if v108 then
		local v946 = Instance.new("Frame", v108);
		v946.Size = UDim2.new(1 + 0, -10, 0 - 0, 30 + 15);
		v946.BackgroundTransparency = 1;
		local v949 = Instance.new("TextButton", v946);
		v949.Size = UDim2.new(0.65 - 0, 0, 1710 - (1596 + 114), 40);
		v949.BackgroundColor3 = Color3.fromRGB(104 - 64, 753 - (164 + 549), 80);
		v949.Text = "幽霊船へTP";
		v949.TextColor3 = Color3.new(1, 1439 - (1059 + 379), 1 - 0);
		Instance.new("UICorner", v949);
		v949.MouseButton1Click:Connect(function()
			v559(v555, "幽霊船");
		end);
		local v954 = Instance.new("TextButton", v946);
		v954.Size = UDim2.new(0.3, 0 + 0, 0 + 0, 432 - (145 + 247));
		v954.Position = UDim2.new(0.7 + 0, 0 + 0, 0 - 0, 0 + 0);
		v954.BackgroundColor3 = Color3.fromRGB(18 + 2, 32 - 12, 740 - (254 + 466));
		v954.Text = "[" .. _G.NebulaSettings.GhostShipKey .. "]";
		v954.TextColor3 = Color3.new(561 - (544 + 16), 0.8 - 0, 628 - (294 + 334));
		Instance.new("UICorner", v954);
		v954.MouseButton1Click:Connect(function()
			local v1094 = 253 - (236 + 17);
			while true do
				if (v1094 == 1) then
					task.spawn(function()
						local v1423 = 0 + 0;
						local v1424;
						while true do
							if (v1423 == (0 + 0)) then
								v1424 = 0 - 0;
								while true do
									if ((0 - 0) == v1424) then
										while v557 do
											task.wait();
										end
										v954.Text = "[" .. _G.NebulaSettings.GhostShipKey .. "]";
										break;
									end
								end
								break;
							end
						end
					end);
					break;
				end
				if (v1094 == (0 + 0)) then
					v954.Text = "入力待機...";
					v557 = true;
					v1094 = 1;
				end
			end
		end);
		local v960 = Instance.new("Frame", v108);
		v960.Size = UDim2.new(1, -10, 0 + 0, 839 - (413 + 381));
		v960.BackgroundTransparency = 1;
		local v963 = Instance.new("TextButton", v960);
		v963.Size = UDim2.new(0.65, 0, 0 + 0, 40);
		v963.BackgroundColor3 = Color3.fromRGB(80, 85 - 45, 103 - 63);
		v963.Text = "マンションへTP";
		v963.TextColor3 = Color3.new(1971 - (582 + 1388), 1 - 0, 1 + 0);
		Instance.new("UICorner", v963);
		v963.MouseButton1Click:Connect(function()
			v559(v556, "マンション");
		end);
		local v968 = Instance.new("TextButton", v960);
		v968.Size = UDim2.new(0.3, 0, 364 - (326 + 38), 118 - 78);
		v968.Position = UDim2.new(0.7 - 0, 620 - (47 + 573), 0, 0 + 0);
		v968.BackgroundColor3 = Color3.fromRGB(84 - 64, 32 - 12, 1684 - (1269 + 395));
		v968.Text = "[" .. _G.NebulaSettings.MansionKey .. "]";
		v968.TextColor3 = Color3.new(493 - (76 + 416), 0.8, 443 - (319 + 124));
		Instance.new("UICorner", v968);
		v968.MouseButton1Click:Connect(function()
			local v1095 = 0 - 0;
			local v1096;
			while true do
				if ((1007 - (564 + 443)) == v1095) then
					v1096 = 0 - 0;
					while true do
						if (v1096 == 0) then
							v968.Text = "入力待機...";
							v558 = true;
							v1096 = 1;
						end
						if (v1096 == (459 - (337 + 121))) then
							task.spawn(function()
								local v1649 = 0;
								while true do
									if (v1649 == (0 - 0)) then
										while v558 do
											task.wait();
										end
										v968.Text = "[" .. _G.NebulaSettings.MansionKey .. "]";
										break;
									end
								end
							end);
							break;
						end
					end
					break;
				end
			end
		end);
	end
end);
if not _G.NebulaSettings then
	_G.NebulaSettings = {};
end
_G.NebulaSettings.InvFlyEnabled = false;
_G.NebulaSettings.InvFlyKey = _G.NebulaSettings.InvFlyKey or "B";
_G.NebulaSettings.InvFlySpeed = 999 - 699;
local v217 = -(201907.48 - (1261 + 650));
local v218, v219, v220, v221;
local v222 = false;
local v2 = game:GetService("UserInputService");
local v147 = game:GetService("RunService");
local function v223(v560)
	local v561 = 0 + 0;
	local v562;
	local v563;
	local v564;
	while true do
		if ((2 - 0) == v561) then
			if v560 then
				local v1261 = 1817 - (772 + 1045);
				while true do
					if (v1261 == (0 + 0)) then
						if v218 then
							v218:Destroy();
						end
						v562.Archivable = true;
						v218 = v562:Clone();
						v218.Parent = workspace;
						v1261 = 145 - (102 + 42);
					end
					if (v1261 == 2) then
						v219.Velocity = Vector3.zero;
						v220 = Instance.new("BodyGyro", v218.HumanoidRootPart);
						v220.MaxTorque = Vector3.new(1001844 - (1524 + 320), 1001270 - (1049 + 221), 1000156 - (18 + 138));
						v220.CFrame = v218.HumanoidRootPart.CFrame;
						v1261 = 7 - 4;
					end
					if (v1261 == (1105 - (67 + 1035))) then
						task.spawn(function()
							while _G.NebulaSettings.InvFlyEnabled and v563 do
								local v1650 = 348 - (136 + 212);
								while true do
									if (v1650 == 1) then
										task.wait();
										break;
									end
									if (v1650 == (0 - 0)) then
										v563.CFrame = CFrame.new(v563.Position.X, v217, v563.Position.Z);
										v563.AssemblyLinearVelocity = Vector3.zero;
										v1650 = 1 + 0;
									end
								end
							end
						end);
						v221 = v147.RenderStepped:Connect(function()
							if not v218 then
								return;
							end
							local v1559 = workspace.CurrentCamera;
							local v1560 = v564.MoveDirection;
							local v1561 = Vector3.zero;
							if (v1560.Magnitude > 0) then
								v1561 = (v1559.CFrame.LookVector * -v1560.Z) + (v1559.CFrame.RightVector * v1560.X);
							end
							if v2:IsKeyDown(Enum.KeyCode.Space) then
								v1561 += Vector3.new(0 + 0, 1, 1604 - (240 + 1364))
							elseif v2:IsKeyDown(Enum.KeyCode.LeftShift) then
								v1561 += Vector3.new(1082 - (1050 + 32), -(3 - 2), 0 + 0)
							end
							v219.Velocity = v1561.Unit * _G.NebulaSettings.InvFlySpeed;
							if (v1561.Magnitude == 0) then
								v219.Velocity = Vector3.zero;
							end
							v220.CFrame = v1559.CFrame;
						end);
						v12("Inv-Fly: 有効 (Speed:" .. _G.NebulaSettings.InvFlySpeed .. ")");
						break;
					end
					if (v1261 == (1056 - (331 + 724))) then
						for v1565, v1566 in ipairs(v218:GetDescendants()) do
							if v1566:IsA("BasePart") then
								local v1690 = 0 + 0;
								while true do
									if (v1690 == (644 - (269 + 375))) then
										v1566.CanCollide = false;
										v1566.Transparency = 0.5;
										break;
									end
								end
							end
						end
						workspace.CurrentCamera.CameraSubject = v218.Humanoid;
						v219 = Instance.new("BodyVelocity", v218.HumanoidRootPart);
						v219.MaxForce = Vector3.new(1000000, 1000725 - (267 + 458), 310961 + 689039);
						v1261 = 3 - 1;
					end
				end
			else
				local v1262 = 0;
				while true do
					if ((818 - (667 + 151)) == v1262) then
						if v221 then
							v221:Disconnect();
						end
						if (v218 and v563) then
							local v1651 = 1497 - (1410 + 87);
							while true do
								if (v1651 == (1898 - (1504 + 393))) then
									v218 = nil;
									break;
								end
								if (v1651 == (0 - 0)) then
									v563.CFrame = v218.HumanoidRootPart.CFrame;
									v218:Destroy();
									v1651 = 1;
								end
							end
						end
						v1262 = 1;
					end
					if (v1262 == 1) then
						workspace.CurrentCamera.CameraSubject = v564;
						v12("Inv-Fly: 解除しました");
						break;
					end
				end
			end
			break;
		end
		if (v561 == (0 - 0)) then
			_G.NebulaSettings.InvFlyEnabled = v560;
			v562 = game.Players.LocalPlayer.Character;
			v561 = 1;
		end
		if (v561 == (797 - (461 + 335))) then
			v563 = v562 and v562:FindFirstChild("HumanoidRootPart");
			v564 = v562 and v562:FindFirstChild("Humanoid");
			v561 = 2;
		end
	end
end
v2.InputBegan:Connect(function(v565, v566)
	local v567 = 0 + 0;
	while true do
		if (v567 == (1761 - (1730 + 31))) then
			if v566 then
				return;
			end
			if v222 then
				local v1263 = 0;
				local v1264;
				while true do
					if ((1667 - (728 + 939)) == v1263) then
						v1264 = 0 - 0;
						while true do
							if (v1264 == (1 - 0)) then
								v12("Flyキーを " .. v565.KeyCode.Name .. " に変更");
								return;
							end
							if (v1264 == (0 - 0)) then
								_G.NebulaSettings.InvFlyKey = v565.KeyCode.Name;
								v222 = false;
								v1264 = 1069 - (138 + 930);
							end
						end
						break;
					end
				end
			end
			v567 = 1 + 0;
		end
		if (v567 == (1 + 0)) then
			if (v565.KeyCode.Name == _G.NebulaSettings.InvFlyKey) then
				_G.NebulaSettings.InvFlyEnabled = not _G.NebulaSettings.InvFlyEnabled;
				v223(_G.NebulaSettings.InvFlyEnabled);
			end
			break;
		end
	end
end);
if v106 then
	local v856 = 0 + 0;
	local v857;
	while true do
		if (v856 == (0 - 0)) then
			v103(v106, "Invisible & Fly", false, function(v1265)
				v223(v1265);
			end);
			v104(v106, "Flyスピード", 10, 2566 - (459 + 1307), 2170 - (474 + 1396), function(v1266)
				_G.NebulaSettings.InvFlySpeed = v1266;
			end);
			v857 = Instance.new("TextButton", v106);
			v857.Size = UDim2.new(1, -10, 0 - 0, 40);
			v856 = 1;
		end
		if (v856 == (1 + 0)) then
			v857.BackgroundColor3 = Color3.fromRGB(1 + 44, 128 - 83, 45);
			v857.Text = "オンオフキー: [" .. _G.NebulaSettings.InvFlyKey .. "]";
			v857.TextColor3 = Color3.new(1, 1, 1 + 0);
			v857.Font = Enum.Font.SourceSansBold;
			v856 = 2;
		end
		if (v856 == 2) then
			v857.TextSize = 53 - 37;
			Instance.new("UICorner", v857);
			v857.MouseButton1Click:Connect(function()
				local v1267 = 0 - 0;
				while true do
					if (v1267 == 0) then
						v857.Text = "キー入力待機...";
						v222 = true;
						v1267 = 1;
					end
					if (v1267 == (592 - (562 + 29))) then
						task.spawn(function()
							local v1567 = 0 + 0;
							local v1568;
							while true do
								if (v1567 == (1419 - (374 + 1045))) then
									v1568 = 0 + 0;
									while true do
										if (v1568 == 0) then
											while v222 do
												task.wait();
											end
											v857.Text = "オンオフキー: [" .. _G.NebulaSettings.InvFlyKey .. "]";
											break;
										end
									end
									break;
								end
							end
						end);
						break;
					end
				end
			end);
			break;
		end
	end
end
task.spawn(function()
	local v568 = (((typeof(v108) == "Instance") or (typeof(v108) == "userdata")) and v108) or v106;
	if not v568 then
		return;
	end
	local v569 = game:GetService("Players").LocalPlayer;
	local v570 = game:GetService("RunService");
	local v571 = game:GetService("ReplicatedStorage");
	local v572 = game:GetService("CollectionService");
	local v573 = v571:WaitForChild("Remotes"):WaitForChild("CommF_");
	_G.AutoBuso = false;
	v103(v568, "Auto Buso Haki", false, function(v858)
		_G.AutoBuso = v858;
	end);
	task.spawn(function()
		while true do
			local v974 = 0;
			while true do
				if (v974 == (0 - 0)) then
					task.wait(638.5 - (448 + 190));
					if _G.AutoBuso then
						pcall(function()
							local v1507 = 0 + 0;
							local v1508;
							while true do
								if (v1507 == 0) then
									v1508 = v569.Character;
									if (v1508 and v572:HasTag(v1508, "Buso") and not v1508:FindFirstChild("HasBuso")) then
										v573:InvokeServer("Buso");
									end
									break;
								end
							end
						end);
					end
					break;
				end
			end
		end
	end);
	task.spawn(function()
		local v859 = 0 + 0;
		local v860;
		local v861;
		local v862;
		local v863;
		local v864;
		local v865;
		local v866;
		local v867;
		local v868;
		local v869;
		local v870;
		while true do
			if (v859 == (2 + 1)) then
				v869 = nil;
				function v869()
					local v1268 = {};
					local v1269 = nil;
					local v1270 = v861.Character;
					local v1271 = v1270 and v1270:FindFirstChild("HumanoidRootPart");
					if not v1271 then
						return nil, {};
					end
					local function v1272(v1359)
						local v1360 = 0;
						while true do
							if (v1360 == (0 - 0)) then
								if not v1359 then
									return;
								end
								for v1652, v1653 in pairs(v1359:GetChildren()) do
									if (v1653 ~= v1270) then
										local v1715 = 0;
										local v1716;
										local v1717;
										while true do
											if (v1715 == (0 - 0)) then
												v1716 = v1653:FindFirstChild("Humanoid");
												v1717 = v1653:FindFirstChild("HumanoidRootPart") or v1653:FindFirstChild("Head");
												v1715 = 1;
											end
											if (v1715 == (1495 - (1307 + 187))) then
												if (v1716 and v1717 and (v1716.Health > (0 - 0))) then
													local v1810 = 0 - 0;
													local v1811;
													while true do
														if (v1810 == 0) then
															v1811 = (v1271.Position - v1717.Position).Magnitude;
															if (v1811 <= v868) then
																local v1833 = 0;
																while true do
																	if (v1833 == (0 - 0)) then
																		table.insert(v1268, {v1653,v1717});
																		v1269 = v1717;
																		break;
																	end
																end
															end
															break;
														end
													end
												end
												break;
											end
										end
									end
								end
								break;
							end
						end
					end
					v1272(workspace:FindFirstChild("Enemies"));
					v1272(workspace:FindFirstChild("Characters"));
					return v1269, v1268;
				end
				v103(v860, "Fast Attack", false, function(v1273)
					v866 = v1273;
				end);
				v859 = 4 + 0;
			end
			if (v859 == (564 - (510 + 54))) then
				v860 = v108;
				v861 = game:GetService("Players").LocalPlayer;
				v862 = game:GetService("ReplicatedStorage");
				v859 = 1 - 0;
			end
			if (v859 == (40 - (13 + 23))) then
				v870 = nil;
				function v870()
					local v1274 = v861.Character;
					local v1275 = v1274 and v1274:FindFirstChildOfClass("Tool");
					if (not v1275 or not ((v1275.ToolTip == "Melee") or (v1275.ToolTip == "Sword") or (v1275.ToolTip == "Blox Fruit"))) then
						return;
					end
					local v1276, v1277 = v869();
					v864:FireServer(v867);
					if (v1276 and (#v1277 > (0 - 0))) then
						v865:FireServer(v1276, v1277);
					end
					if v1275:FindFirstChild("LeftClickRemote") then
						local v1425 = 0 - 0;
						local v1426;
						while true do
							if (v1425 == 1) then
								v1275.LeftClickRemote:FireServer(v1426, 1 - 0);
								break;
							end
							if (v1425 == 0) then
								v1426 = nil;
								if v1276 then
									v1426 = (v1276.Position - v1274:GetPivot().Position).Unit;
								else
									v1426 = v1274.HumanoidRootPart.CFrame.LookVector;
								end
								v1425 = 1;
							end
						end
					end
				end
				task.spawn(function()
					while true do
						local v1361 = 0;
						while true do
							if (v1361 == (1088 - (830 + 258))) then
								if v866 then
									pcall(v870);
								end
								task.wait(v867);
								break;
							end
						end
					end
				end);
				break;
			end
			if (v859 == 2) then
				v866 = false;
				v867 = 0.01 - 0;
				v868 = 626 + 374;
				v859 = 3 + 0;
			end
			if (v859 == (1442 - (860 + 581))) then
				v863 = v862:WaitForChild("Modules"):WaitForChild("Net");
				v864 = v863["RE/RegisterAttack"];
				v865 = v863["RE/RegisterHit"];
				v859 = 7 - 5;
			end
		end
	end);
	_G.InfiniteEnergy = false;
	v103(v568, "Infinite Energy", false, function(v871)
		_G.InfiniteEnergy = v871;
	end);
	v570.Heartbeat:Connect(function()
		if _G.InfiniteEnergy then
			local v1098 = 0 + 0;
			local v1099;
			while true do
				if ((241 - (237 + 4)) == v1098) then
					v1099 = v569.Character;
					if (v1099 and v1099:FindFirstChild("Energy")) then
						v1099.Energy.Value = v1099.Energy.MaxValue;
					end
					break;
				end
			end
		end
	end);
end);
task.spawn(function()
	local v574 = v108;
	local v575 = game:GetService("Players").LocalPlayer;
	local v576 = game:GetService("ReplicatedStorage");
	v103(v574, "Fruit Sniper", false, function(v872)
		_G.FruitSniper = v872;
	end);
	task.spawn(function()
		while task.wait(2 - 1) do
			if _G.FruitSniper then
				pcall(function()
					for v1363, v1364 in pairs(workspace:GetChildren()) do
						if (v1364:IsA("Tool") and v1364:FindFirstChild("Handle")) then
							local v1511 = 0 - 0;
							local v1512;
							while true do
								if (v1511 == 0) then
									v1512 = v575.Character and v575.Character:FindFirstChild("HumanoidRootPart");
									if v1512 then
										local v1756 = 0 - 0;
										while true do
											if (v1756 == (0 + 0)) then
												v1512.CFrame = v1364.Handle.CFrame;
												task.wait(0.1 + 0);
												v1756 = 3 - 2;
											end
											if (1 == v1756) then
												firetouchinterest(v1512, v1364.Handle, 0);
												firetouchinterest(v1512, v1364.Handle, 1 + 0);
												break;
											end
										end
									end
									break;
								end
							end
						end
					end
				end);
			end
		end
	end);
	v103(v574, "Bring Mob (敵寄せ)", false, function(v873)
		_G.BringMob = v873;
	end);
	v103(v574, "Freeze Mob (敵固定)", false, function(v874)
		_G.FreezeMob = v874;
	end);
	task.spawn(function()
		while task.wait(0.5) do
			pcall(function()
				local v1100 = 0 + 0;
				while true do
					if (v1100 == 0) then
						if _G.BringMob then
							local v1513 = 1426 - (85 + 1341);
							local v1514;
							while true do
								if (v1513 == (0 - 0)) then
									v1514 = v575.Character.HumanoidRootPart;
									for v1720, v1721 in pairs(workspace.Enemies:GetChildren()) do
										if v1721:FindFirstChild("HumanoidRootPart") then
											local v1769 = 0;
											while true do
												if (v1769 == (0 - 0)) then
													v1721.HumanoidRootPart.CFrame = v1514.CFrame * CFrame.new(0, 0, -(377 - (45 + 327)));
													v1721.HumanoidRootPart.CanCollide = false;
													break;
												end
											end
										end
									end
									break;
								end
							end
						end
						if _G.FreezeMob then
							for v1569, v1570 in pairs(workspace.Enemies:GetChildren()) do
								if v1570:FindFirstChild("Humanoid") then
									local v1694 = 0;
									while true do
										if ((0 - 0) == v1694) then
											v1570.Humanoid.WalkSpeed = 502 - (444 + 58);
											if v1570:FindFirstChild("HumanoidRootPart") then
												v1570.HumanoidRootPart.Anchored = true;
											end
											break;
										end
									end
								end
							end
						end
						break;
					end
				end
			end);
		end
	end);
	_G.KillRange = 50;
	v103(v574, "Kill Aura", false, function(v875)
		_G.KillAura = v875;
	end);
	task.spawn(function()
		while task.wait() do
			if _G.KillAura then
				pcall(function()
					local v1278 = 0;
					local v1279;
					while true do
						if (v1278 == 0) then
							v1279 = v575.Character.HumanoidRootPart;
							for v1571, v1572 in pairs(workspace.Enemies:GetChildren()) do
								local v1573 = 0;
								local v1574;
								local v1575;
								while true do
									if (v1573 == (1 + 0)) then
										if (v1574 and v1575 and ((v1574.Position - v1279.Position).Magnitude < _G.KillRange)) then
											v1575.Health = 0 + 0;
										end
										break;
									end
									if (v1573 == (0 + 0)) then
										v1574 = v1572:FindFirstChild("HumanoidRootPart");
										v1575 = v1572:FindFirstChild("Humanoid");
										v1573 = 2 - 1;
									end
								end
							end
							break;
						end
					end
				end);
			end
		end
	end);
end);
task.spawn(function()
	local v577 = 0;
	local v578;
	local v579;
	while true do
		if (v577 == (1733 - (64 + 1668))) then
			v579 = game:GetService("Players").LocalPlayer;
			v103(v578, "Water Walking", false, function(v1186)
				local v1187 = 1973 - (1227 + 746);
				while true do
					if (v1187 == 0) then
						_G.WaterWalkingEnabled = v1186;
						if v1186 then
							task.spawn(function()
								while _G.WaterWalkingEnabled do
									local v1695 = v579.Name;
									local v1696 = game:GetService("Workspace").Characters:FindFirstChild(v1695);
									if v1696 then
										local v1757 = 0;
										local v1758;
										while true do
											if (v1757 == (2 - 1)) then
												v1758 = v1696:FindFirstChild("WaterWalking");
												if v1758 then
													pcall(function()
														v1758.Value = true;
													end);
												end
												break;
											end
											if (v1757 == (0 - 0)) then
												pcall(function()
													v1696.WaterWalking = true;
												end);
												pcall(function()
													v1696:SetAttribute("WaterWalking", true);
												end);
												v1757 = 1;
											end
										end
									end
									task.wait(494.5 - (415 + 79));
								end
							end);
						else
							pcall(function()
								local v1654 = 0 + 0;
								local v1655;
								local v1656;
								local v1657;
								while true do
									if ((491 - (142 + 349)) == v1654) then
										v1655 = 0;
										v1656 = nil;
										v1654 = 1;
									end
									if (v1654 == (1 + 0)) then
										v1657 = nil;
										while true do
											if (1 == v1655) then
												if v1657 then
													local v1820 = 0;
													local v1821;
													while true do
														if (v1820 == (1 - 0)) then
															v1821 = v1657:FindFirstChild("WaterWalking");
															if v1821 then
																v1821.Value = false;
															end
															break;
														end
														if (v1820 == 0) then
															v1657.WaterWalking = false;
															v1657:SetAttribute("WaterWalking", false);
															v1820 = 1;
														end
													end
												end
												break;
											end
											if (v1655 == (0 + 0)) then
												v1656 = v579.Name;
												v1657 = game:GetService("Workspace").Characters:FindFirstChild(v1656);
												v1655 = 1;
											end
										end
										break;
									end
								end
							end);
						end
						break;
					end
				end
			end);
			break;
		end
		if (v577 == (0 + 0)) then
			v578 = (((typeof(v108) == "Instance") or (typeof(v108) == "userdata")) and v108) or v106;
			if not v578 then
				return;
			end
			v577 = 1;
		end
	end
end);
task.spawn(function()
	local v580 = (((typeof(v108) == "Instance") or (typeof(v108) == "userdata")) and v108) or v106;
	if not v580 then
		return;
	end
	local v581 = game:GetService("Players").LocalPlayer;
	local v582 = game:GetService("RunService");
	_G.NPCBangEnabled = false;
	_G.NPCBangRange = 272 - 172;
	v103(v580, "NPC BANG", false, function(v876)
		_G.NPCBangEnabled = v876;
	end);
	v104(v580, "BANG 探索範囲", 10, 2864 - (1710 + 154), 418 - (200 + 118), function(v877)
		_G.NPCBangRange = v877;
	end);
	v582.Heartbeat:Connect(function()
		local v878 = 0;
		local v879;
		local v880;
		local v881;
		local v882;
		local v883;
		while true do
			if (v878 == (2 + 1)) then
				local v1188 = 0;
				while true do
					if (v1188 == (0 - 0)) then
						v883 = {workspace:FindFirstChild("Enemies"),workspace:FindFirstChild("NPCs"),workspace};
						for v1516, v1517 in pairs(v883) do
							if v1517 then
								for v1697, v1698 in pairs(v1517:GetChildren()) do
									if (v1698:IsA("Model") and v1698:FindFirstChild("Humanoid") and (v1698.Humanoid.Health > (0 + 0)) and v1698:FindFirstChild("HumanoidRootPart")) then
										local v1759 = 0;
										local v1760;
										local v1761;
										local v1762;
										while true do
											if (v1759 == (0 + 0)) then
												v1760 = 0;
												v1761 = nil;
												v1759 = 1;
											end
											if (v1759 == 1) then
												v1762 = nil;
												while true do
													if (v1760 == (0 - 0)) then
														v1761 = string.lower(v1698.Name);
														v1762 = string.lower(v1698.Humanoid.DisplayName);
														v1760 = 1;
													end
													if (v1760 == 1) then
														if (not string.find(v1761, "shadow") and not string.find(v1762, "shadow")) then
															if (v1698.Name ~= v581.Name) then
																local v1837 = 1250 - (363 + 887);
																local v1838;
																while true do
																	if (v1837 == (0 - 0)) then
																		v1838 = (v880.Position - v1698.HumanoidRootPart.Position).Magnitude;
																		if (v1838 < v882) then
																			local v1843 = 0 - 0;
																			while true do
																				if (v1843 == 0) then
																					v882 = v1838;
																					v881 = v1698;
																					break;
																				end
																			end
																		end
																		break;
																	end
																end
															end
														end
														break;
													end
												end
												break;
											end
										end
									end
								end
							end
							if v881 then
								break;
							end
						end
						v1188 = 1 + 0;
					end
					if (v1188 == (2 - 1)) then
						v878 = 3 + 1;
						break;
					end
				end
			end
			if (v878 == 2) then
				local v1189 = 0;
				while true do
					if (v1189 == 0) then
						v881 = nil;
						v882 = _G.NPCBangRange;
						v1189 = 1665 - (674 + 990);
					end
					if (v1189 == 1) then
						v878 = 1 + 2;
						break;
					end
				end
			end
			if (v878 == (2 + 2)) then
				if v881 then
					local v1365 = 0 - 0;
					while true do
						if (v1365 == 0) then
							v880.CFrame = v881.HumanoidRootPart.CFrame * CFrame.new(1055 - (507 + 548), 12, 837 - (289 + 548));
							v880.AssemblyLinearVelocity = Vector3.new(1818 - (821 + 997), 0, 255 - (195 + 60));
							break;
						end
					end
				end
				break;
			end
			if (v878 == 1) then
				local v1190 = 0;
				while true do
					if (v1190 == (0 + 0)) then
						v880 = v879 and v879:FindFirstChild("HumanoidRootPart");
						if not v880 then
							return;
						end
						v1190 = 1;
					end
					if (v1190 == (1502 - (251 + 1250))) then
						v878 = 5 - 3;
						break;
					end
				end
			end
			if (v878 == (0 + 0)) then
				if not _G.NPCBangEnabled then
					return;
				end
				v879 = v581.Character;
				v878 = 1033 - (809 + 223);
			end
		end
	end);
end);
task.spawn(function()
	local v583 = 0 - 0;
	local v584;
	local v585;
	local v586;
	local v587;
	local v588;
	local v589;
	local v590;
	while true do
		if (v583 == 0) then
			local v1102 = 0 - 0;
			while true do
				if (v1102 == (6 - 4)) then
					v583 = 1 + 0;
					break;
				end
				if (v1102 == (1 + 0)) then
					v585 = game:GetService("Players").LocalPlayer;
					v586 = game:GetService("ReplicatedStorage");
					v1102 = 2;
				end
				if (v1102 == (617 - (14 + 603))) then
					v584 = (((typeof(v108) == "Instance") or (typeof(v108) == "userdata")) and v108) or v106;
					if not v584 then
						return;
					end
					v1102 = 130 - (118 + 11);
				end
			end
		end
		if (v583 == (1 + 2)) then
			v103(v584, "Auto Race Ability (V3スキル連打)", false, function(v1192)
				_G.AutoRaceV3_Ability = v1192;
			end);
			v587.Heartbeat:Connect(function(v1193)
				local v1194 = v585.Character;
				if not v1194 then
					return;
				end
				pcall(function()
					local v1280 = 0 + 0;
					while true do
						if (v1280 == (0 - 0)) then
							if _G.AutoRaceV4_Force then
								local v1658 = v1194:FindFirstChild("RaceEnergy");
								if (v1658 and (v1658.Value >= (950 - (551 + 398)))) then
									local v1722 = 0 + 0;
									local v1723;
									local v1724;
									while true do
										if (v1722 == (1 + 0)) then
											v586.Remotes.CommE:FireServer("ActivateAbility");
											v1724 = v585.Backpack:FindFirstChild("Awakening") or v1194:FindFirstChild("Awakening");
											v1722 = 2 + 0;
										end
										if (v1722 == (0 - 0)) then
											local v1786 = 0;
											while true do
												if (v1786 == 1) then
													v1722 = 1;
													break;
												end
												if (v1786 == (0 - 0)) then
													v1723 = v1194:FindFirstChild("RaceTransformed");
													if v1723 then
														v1723.Value = false;
													end
													v1786 = 1 + 0;
												end
											end
										end
										if (v1722 == 2) then
											if (v1724 and v1724:FindFirstChild("RemoteFunction")) then
												v1724.RemoteFunction:InvokeServer(true);
											end
											break;
										end
									end
								end
							end
							if _G.AutoRaceV3_Ability then
								local v1659 = 0;
								local v1660;
								while true do
									if (v1659 == (0 - 0)) then
										v1660 = v1194:FindFirstChildOfClass("Humanoid");
										if (v1660 and (v1660.Health > 0) and v590()) then
											local v1787 = 0 + 0;
											while true do
												if (v1787 == (89 - (40 + 49))) then
													v588 = v588 - v1193;
													if (v588 <= 0) then
														local v1826 = 0 - 0;
														while true do
															if (v1826 == 0) then
																v586.Remotes.CommE:FireServer("ActivateAbility");
																v588 = 490.2 - (99 + 391);
																break;
															end
														end
													end
													break;
												end
											end
										end
										break;
									end
								end
							end
							break;
						end
					end
				end);
			end);
			break;
		end
		if (v583 == (2 + 0)) then
			v589 = {"Last Resort","Agility","Water Body","Heavenly Blood","Heightened Senses","Energy Core","Primordial Reign"};
			v590 = nil;
			function v590()
				local v1195 = 417 - (203 + 214);
				local v1196;
				while true do
					if (v1195 == (1818 - (568 + 1249))) then
						for v1518, v1519 in ipairs(v589) do
							if (v585.Backpack:FindFirstChild(v1519) or v1196:FindFirstChild(v1519)) then
								return true;
							end
						end
						return false;
					end
					if (v1195 == (0 + 0)) then
						v1196 = v585.Character;
						if not v1196 then
							return false;
						end
						v1195 = 1;
					end
				end
			end
			v103(v584, "Auto Race V4 (強制変身)", false, function(v1197)
				_G.AutoRaceV4_Force = v1197;
			end);
			v583 = 3;
		end
		if (v583 == (2 - 1)) then
			v587 = game:GetService("RunService");
			_G.AutoRaceV4_Force = false;
			_G.AutoRaceV3_Ability = false;
			v588 = 0 - 0;
			v583 = 1308 - (913 + 393);
		end
	end
end);
_G.BoatMaxSpeed = 100;
_G.AutoBoatSpeedEnabled = true;
task.spawn(function()
	while task.wait(2 - 1) do
		if _G.AutoBoatSpeedEnabled then
			pcall(function()
				local v1198 = 0;
				local v1199;
				while true do
					if (v1198 == 0) then
						v1199 = workspace:FindFirstChild("Boats");
						if v1199 then
							for v1661, v1662 in pairs(v1199:GetDescendants()) do
								if v1662:IsA("VehicleSeat") then
									if (v1662.MaxSpeed ~= _G.BoatMaxSpeed) then
										v1662.MaxSpeed = _G.BoatMaxSpeed;
									end
								end
							end
						end
						break;
					end
				end
			end);
		end
	end
end);
v104(v108, "ボートの速度", 141 - 41, 910 - (269 + 141), _G.BoatMaxSpeed, function(v591)
	local v592 = 0 - 0;
	while true do
		if (v592 == 0) then
			_G.BoatMaxSpeed = v591;
			_G.AutoBoatSpeedEnabled = true;
			v592 = 1;
		end
		if (v592 == (1982 - (362 + 1619))) then
			pcall(function()
				local v1200 = workspace:FindFirstChild("Boats");
				if v1200 then
					for v1428, v1429 in pairs(v1200:GetDescendants()) do
						if v1429:IsA("VehicleSeat") then
							v1429.MaxSpeed = v591;
						end
					end
				end
			end);
			break;
		end
	end
end);
task.spawn(function()
	local v593 = (((typeof(v108) == "Instance") or (typeof(v108) == "userdata")) and v108) or v106;
	if not v593 then
		return;
	end
	local v594 = game:GetService("Players").LocalPlayer;
	local v595 = game:GetService("ReplicatedStorage");
	local v596 = game:GetService("TweenService");
	local v597 = v595:WaitForChild("Remotes"):WaitForChild("CommF_");
	local v598 = {RaidAutoMove=false,AutoStartRaid=false,SelectRaid="Flame",TweenSpeed=(1875 - (950 + 675))};
	local v599 = {"Flame","Ice","Quake","Light","Dark","Spider","Rumble","Magma","Buddha","Sand"};
	local v600 = {"Rocket-Rocket","Spin-Spin","Chop-Chop","Spring-Spring","Bomb-Bomb","Smoke-Smoke"};
	local function v601(v884)
		local v885 = 0 - 0;
		local v886;
		local v887;
		local v888;
		while true do
			if ((7 - 5) == v885) then
				v888:Play();
				break;
			end
			if (v885 == (0 - 0)) then
				v886 = v594.Character and v594.Character:FindFirstChild("HumanoidRootPart");
				if not v886 then
					return;
				end
				v885 = 2 - 1;
			end
			if (v885 == (1 + 0)) then
				local v1201 = 529 - (318 + 211);
				while true do
					if (v1201 == 1) then
						v885 = 9 - 7;
						break;
					end
					if (v1201 == 0) then
						v887 = (v884.Position - v886.Position).Magnitude;
						v888 = v596:Create(v886, TweenInfo.new(v887 / v598.TweenSpeed, Enum.EasingStyle.Linear), {CFrame=v884});
						v1201 = 1588 - (963 + 624);
					end
				end
			end
		end
	end
	v105(v593, "--- Click Below to Select Raid ---", function()
	end);
	for v889, v890 in pairs(v599) do
		v105(v593, "Select: " .. v890, function()
			local v975 = 0 + 0;
			while true do
				if (v975 == (846 - (518 + 328))) then
					v598.SelectRaid = v890;
					pcall(function()
						game:GetService("StarterGui"):SetCore("SendNotification", {Title="Raid Selected",Text=("Target: " .. v890),Duration=2});
					end);
					break;
				end
			end
		end);
	end
	v105(v593, "----------------------------", function()
	end);
	v105(v593, "Get Low Fruit (実を出す)", function()
		for v976, v977 in pairs(v600) do
			if v597:InvokeServer("LoadFruit", v977) then
				break;
			end
		end
	end);
	v103(v593, "Raid Auto Move (250)", false, function(v891)
		v598.RaidAutoMove = v891;
	end);
	v103(v593, "Auto Start Raid", false, function(v893)
		v598.AutoStartRaid = v893;
	end);
	task.spawn(function()
		while task.wait(2.5 - 1) do
			if v598.AutoStartRaid then
				pcall(function()
					local v1282 = 0;
					local v1283;
					while true do
						if ((0 - 0) == v1282) then
							v1283 = v594.PlayerGui.Main:FindFirstChild("Timer");
							if not (v1283 and v1283.Visible) then
								local v1663 = 0;
								local v1664;
								while true do
									if (v1663 == 0) then
										v1664 = v594.Backpack:FindFirstChild("Special Microchip") or v594.Character:FindFirstChild("Special Microchip");
										if v1664 then
											local v1788 = 317 - (301 + 16);
											local v1789;
											local v1790;
											local v1791;
											while true do
												if (v1788 == 1) then
													v1791 = nil;
													while true do
														if (v1789 == 0) then
															v1790 = workspace.Map:FindFirstChild("CircleIsland") or workspace.Map:FindFirstChild("Boat Castle");
															v1791 = v1790 and v1790:FindFirstChild("RaidSummon2") and v1790.RaidSummon2.Button.Main;
															v1789 = 2 - 1;
														end
														if (v1789 == (2 - 1)) then
															if v1791 then
																v601(v1791.CFrame);
															end
															break;
														end
													end
													break;
												end
												if (v1788 == (0 - 0)) then
													v1789 = 0 + 0;
													v1790 = nil;
													v1788 = 1;
												end
											end
										else
											local v1792 = 0 + 0;
											while true do
												if (v1792 == 0) then
													v597:InvokeServer("RaidsNpc", "Select", v598.SelectRaid);
													v597:InvokeServer("RaidsNpc", "Buy");
													break;
												end
											end
										end
										break;
									end
								end
							end
							break;
						end
					end
				end);
			end
		end
	end);
	workspace:WaitForChild("Map"):WaitForChild("RaidMap").ChildAdded:Connect(function(v895)
		if (v598.RaidAutoMove and v895.Name:match("RaidIsland")) then
			local v1103 = 0 - 0;
			local v1104;
			while true do
				if (v1103 == 1) then
					v1104 = v895:FindFirstChildWhichIsA("BasePart") or (v895:IsA("Model") and v895.PrimaryPart);
					if v1104 then
						v601(v1104.CFrame + Vector3.new(0, 31 + 19, 0));
					end
					break;
				end
				if (v1103 == (0 + 0)) then
					if (v895.Name:match("RaidIsland1") and not v895.Name:match("RaidIsland1[0-9]")) then
						return;
					end
					task.wait(1);
					v1103 = 3 - 2;
				end
			end
		end
	end);
end);
v105(v106, "Fly", function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))();
	v12("Flyスクリプトを実行しました");
end);
v9.Noclip = false;
v103(v106, "Noclip（壁抜け）", v9.Noclip, function(v602)
	v9.Noclip = v602;
end);
game:GetService("RunService").Stepped:Connect(function()
	if v9.Noclip then
		local v978 = 0;
		local v979;
		while true do
			if (v978 == 0) then
				v979 = v1.Character;
				if v979 then
					for v1520, v1521 in pairs(v979:GetDescendants()) do
						if v1521:IsA("BasePart") then
							v1521.CanCollide = false;
						end
					end
				end
				break;
			end
		end
	end
end);
local v225 = v102("Player Information");
local v210 = game:GetService("Players");
local v226 = game:GetService("UserInputService");
local v227 = {["Summon Sea Beast"]=true,Awakening=true,Tool=true,["Last Resort"]=true,Agility=true,["Water Body"]=true,["Heavenly Blood"]=true,["Heightened Senses"]=true,["Energy Core"]=true,["Primordial Reign"]=true};
local v228 = {"Last Resort","Agility","Water Body","Heavenly Blood","Heightened Senses","Energy Core","Primordial Reign"};
local v229 = Instance.new("Frame");
v229.Size = UDim2.new(2 - 1, -(3 + 7), 0 + 0, 1669 - 1119);
v229.Position = UDim2.new(0, 5, 0 + 0, 618 - (520 + 93));
v229.BackgroundColor3 = Color3.fromRGB(286 - (259 + 17), 10, 1 + 9);
v229.Parent = v225;
Instance.new("UICorner", v229);
local v234 = Instance.new("Frame");
v234.Size = UDim2.new(1, 0 + 0, 0 - 0, 641 - (396 + 195));
v234.BackgroundColor3 = Color3.fromRGB(72 - 47, 1786 - (440 + 1321), 1854 - (1059 + 770));
v234.Parent = v229;
local v238 = Instance.new("TextLabel");
v238.Size = UDim2.new(1, 0, 1, 0);
v238.BackgroundTransparency = 4 - 3;
v238.Text = "  PLAYER INTELLIGENCE (v3.5)";
v238.TextColor3 = Color3.new(1, 546 - (424 + 121), 1 + 0);
v238.Font = Enum.Font.SourceSansBold;
v238.TextSize = 1365 - (641 + 706);
v238.TextXAlignment = Enum.TextXAlignment.Left;
v238.Parent = v234;
local v247 = Instance.new("ScrollingFrame");
v247.Size = UDim2.new(1 + 0, -(455 - (249 + 191)), 1, -65);
v247.Position = UDim2.new(0 - 0, 4 + 3, 0 - 0, 482 - (183 + 244));
v247.BackgroundTransparency = 1 + 0;
v247.CanvasSize = UDim2.new(0, 730 - (434 + 296), 0 - 0, 0);
v247.AutomaticCanvasSize = Enum.AutomaticSize.Y;
v247.ScrollBarThickness = 517 - (169 + 343);
v247.Parent = v229;
Instance.new("UIListLayout", v247).Padding = UDim.new(0, 8 + 0);
local function v256(v604, v605)
	local v606 = 0 - 0;
	local v607;
	local v608;
	local v609;
	local v610;
	local v611;
	while true do
		if (v606 == 1) then
			v609 = nil;
			v610 = nil;
			v606 = 2;
		end
		if (v606 == (0 - 0)) then
			v607 = 0 + 0;
			v608 = nil;
			v606 = 2 - 1;
		end
		if ((1125 - (651 + 472)) == v606) then
			v611 = nil;
			while true do
				if (v607 == (1 + 0)) then
					local v1367 = 0 + 0;
					while true do
						if ((1 - 0) == v1367) then
							v607 = 485 - (397 + 86);
							break;
						end
						if (v1367 == (876 - (423 + 453))) then
							v609, v610 = pcall(function()
								return v604[v605];
							end);
							if (v609 and (v610 ~= nil)) then
								return tostring(v610);
							end
							v1367 = 1 + 0;
						end
					end
				end
				if ((1 + 2) == v607) then
					return "Not Found";
				end
				if (2 == v607) then
					local v1368 = 0 + 0;
					while true do
						if (1 == v1368) then
							v607 = 3 + 0;
							break;
						end
						if (v1368 == (0 + 0)) then
							v611 = {v604:FindFirstChild("Data"),v604:FindFirstChild("leaderstats"),v604};
							for v1666, v1667 in pairs(v611) do
								if v1667 then
									local v1725 = 0;
									local v1726;
									while true do
										if (v1725 == (1190 - (50 + 1140))) then
											v1726 = v1667:FindFirstChild(v605);
											if (v1726 and v1726:IsA("ValueBase")) then
												return tostring(v1726.Value);
											end
											break;
										end
									end
								end
							end
							v1368 = 1 + 0;
						end
					end
				end
				if (v607 == (0 + 0)) then
					v608 = v604:GetAttribute(v605);
					if (v608 ~= nil) then
						return tostring(v608);
					end
					v607 = 1;
				end
			end
			break;
		end
	end
end
local function v257(v612, v613)
	local v614 = v612:FindFirstChild("Data");
	if (v614 and v614:FindFirstChild("Stats")) then
		local v980 = 0 + 0;
		local v981;
		while true do
			if (v980 == (0 - 0)) then
				v981 = v614.Stats:FindFirstChild(v613);
				if v981 then
					local v1431 = 0 + 0;
					local v1432;
					while true do
						if ((596 - (157 + 439)) == v1431) then
							local v1668 = 0;
							while true do
								if (v1668 == (0 - 0)) then
									v1432 = v981:FindFirstChild("Level");
									return (v1432 and tostring(v1432.Value)) or (v981:IsA("ValueBase") and tostring(v981.Value)) or "0";
								end
							end
						end
					end
				end
				break;
			end
		end
	end
	return "0";
end
local function v258(v615)
	local v616 = v615:FindFirstChild("Backpack");
	local v617 = v615.Character;
	local function v618(v896)
		return (v616 and v616:FindFirstChild(v896)) or (v617 and v617:FindFirstChild(v896));
	end
	if v618("Awakening") then
		return "v4";
	end
	for v897, v898 in ipairs(v228) do
		if v618(v898) then
			return "v3";
		end
	end
	return "v1/v2";
end
local function v259(v619)
	if v247:FindFirstChild(v619.Name) then
		return;
	end
	local v620 = Instance.new("Frame");
	v620.Name = v619.Name;
	v620.Size = UDim2.new(1, -(16 - 11), 0 - 0, 983 - (782 + 136));
	v620.BackgroundColor3 = Color3.fromRGB(35, 35, 890 - (112 + 743));
	v620.ClipsDescendants = true;
	v620.Parent = v247;
	Instance.new("UICorner", v620);
	local v627 = Instance.new("TextButton");
	v627.Size = UDim2.new(1, 1171 - (1026 + 145), 0, 12 + 53);
	v627.BackgroundTransparency = 719 - (493 + 225);
	v627.Text = "";
	v627.Parent = v620;
	local v632 = Instance.new("ImageLabel");
	v632.Size = UDim2.new(0, 202 - 147, 0 + 0, 147 - 92);
	v632.Position = UDim2.new(0, 1 + 4, 0, 14 - 9);
	v632.BackgroundTransparency = 1 + 0;
	v632.Parent = v627;
	task.spawn(function()
		v632.Image = v210:GetUserThumbnailAsync(v619.UserId, Enum.ThumbnailType.HeadShot, Enum.ThumbnailSize.Size100x100);
	end);
	local v637 = Instance.new("TextLabel");
	v637.Size = UDim2.new(1, -70, 0 - 0, 25);
	v637.Position = UDim2.new(0, 1665 - (210 + 1385), 1689 - (1201 + 488), 5);
	v637.BackgroundTransparency = 1 + 0;
	v637.Text = v619.DisplayName;
	v637.Font = Enum.Font.SourceSansBold;
	v637.TextSize = 28 - 12;
	v637.TextXAlignment = Enum.TextXAlignment.Left;
	v637.Parent = v627;
	local v649 = Instance.new("TextLabel");
	v649.Size = UDim2.new(1, -(125 - 55), 0, 20);
	v649.Position = UDim2.new(0, 655 - (352 + 233), 0, 72 - 42);
	v649.BackgroundTransparency = 1 + 0;
	v649.TextColor3 = Color3.fromRGB(0 - 0, 774 - (489 + 85), 1756 - (277 + 1224));
	v649.TextSize = 1506 - (663 + 830);
	v649.TextXAlignment = Enum.TextXAlignment.Left;
	v649.Font = Enum.Font.SourceSansBold;
	v649.Parent = v627;
	local v658 = Instance.new("TextLabel");
	v658.Size = UDim2.new(1 + 0, -(171 - 101), 875 - (461 + 414), 3 + 12);
	v658.Position = UDim2.new(0, 70, 0, 45);
	v658.BackgroundTransparency = 1 + 0;
	v658.TextColor3 = Color3.fromRGB(25 + 230, 85, 252 + 3);
	v658.TextSize = 12;
	v658.TextXAlignment = Enum.TextXAlignment.Left;
	v658.Font = Enum.Font.SourceSansBold;
	v658.Parent = v627;
	local v667 = Instance.new("ScrollingFrame");
	v667.Size = UDim2.new(251 - (172 + 78), -10, 0, 515 - 195);
	v667.Position = UDim2.new(0 + 0, 7 - 2, 0 + 0, 26 + 49);
	v667.BackgroundColor3 = Color3.fromRGB(33 - 13, 25 - 5, 20);
	v667.CanvasSize = UDim2.new(0 + 0, 0, 0 + 0, 0);
	v667.AutomaticCanvasSize = Enum.AutomaticSize.Y;
	v667.ScrollBarThickness = 2 + 1;
	v667.Parent = v620;
	Instance.new("UICorner", v667);
	Instance.new("UIListLayout", v667).Padding = UDim.new(0 - 0, 5);
	local v677 = Instance.new("TextLabel");
	v677.Size = UDim2.new(2 - 1, -20, 0 + 0, 15 + 10);
	v677.BackgroundTransparency = 448 - (133 + 314);
	v677.TextColor3 = Color3.fromRGB(0, 45 + 210, 150);
	v677.Font = Enum.Font.SourceSansBold;
	v677.TextSize = 229 - (199 + 14);
	v677.TextXAlignment = Enum.TextXAlignment.Left;
	v677.Parent = v667;
	local v685 = Instance.new("TextLabel");
	v685.Size = UDim2.new(1, -20, 0, 0 - 0);
	v685.AutomaticSize = Enum.AutomaticSize.Y;
	v685.BackgroundTransparency = 1550 - (647 + 902);
	v685.TextColor3 = Color3.fromRGB(766 - 511, 255, 100);
	v685.Font = Enum.Font.SourceSansItalic;
	v685.TextSize = 247 - (85 + 148);
	v685.TextXAlignment = Enum.TextXAlignment.Left;
	v685.Parent = v667;
	local v695 = Instance.new("TextLabel");
	v695.Size = UDim2.new(1290 - (426 + 863), -(93 - 73), 1654 - (873 + 781), 0 - 0);
	v695.AutomaticSize = Enum.AutomaticSize.Y;
	v695.BackgroundTransparency = 2 - 1;
	v695.TextColor3 = Color3.fromRGB(106 + 149, 609 - 444, 0 - 0);
	v695.Font = Enum.Font.Code;
	v695.TextSize = 41 - 27;
	v695.TextXAlignment = Enum.TextXAlignment.Left;
	v695.Parent = v667;
	local v705 = Instance.new("TextLabel");
	v705.Size = UDim2.new(1948 - (414 + 1533), -(18 + 2), 555 - (443 + 112), 1479 - (888 + 591));
	v705.AutomaticSize = Enum.AutomaticSize.Y;
	v705.BackgroundTransparency = 1;
	v705.TextColor3 = Color3.new(2 - 1, 1, 1);
	v705.TextSize = 1 + 13;
	v705.TextXAlignment = Enum.TextXAlignment.Left;
	v705.TextWrapped = true;
	v705.Font = Enum.Font.SourceSans;
	v705.Parent = v667;
	local v716 = false;
	v627.MouseButton1Click:Connect(function()
		local v900 = 0 - 0;
		local v901;
		while true do
			if (v900 == (0 + 0)) then
				v901 = 0;
				while true do
					if ((0 + 0) == v901) then
						v716 = not v716;
						v620:TweenSize(UDim2.new(1 + 0, -(9 - 4), 0 - 0, (v716 and (2078 - (136 + 1542))) or (213 - 148)), "Out", "Quad", 0.2, true);
						break;
					end
				end
				break;
			end
		end
	end);
	task.spawn(function()
		while v620.Parent do
			local v982 = 0 + 0;
			local v983;
			local v984;
			local v985;
			local v986;
			local v987;
			while true do
				if (v982 == 2) then
					v986 = v258(v619);
					v987 = v256(v619, "Fragments");
					v982 = 4 - 1;
				end
				if (v982 == (1 + 0)) then
					v984 = v256(v619, "Level");
					v985 = v256(v619, "Race");
					v982 = 2;
				end
				if (v982 == (490 - (68 + 418))) then
					if v716 then
						local v1433 = 0;
						local v1434;
						local v1435;
						local v1436;
						local v1437;
						local v1438;
						local v1439;
						local v1440;
						local v1441;
						local v1442;
						local v1443;
						local v1444;
						while true do
							if (v1433 == (4 - 2)) then
								v1440 = v257(v619, "Melee");
								v1441 = v257(v619, "Sword");
								v695.Text = string.format("  [ STATISTICS ]\n  Team: %s\n  Defense: %s\n  Fruit: %s\n  Gun: %s\n  Melee: %s\n  Sword: %s\n  Fragments: %s", v983, v1437, v1438, v1439, v1440, v1441, v987);
								v1442 = {};
								v1433 = 3;
							end
							if (v1433 == (0 - 0)) then
								v1434 = v619.Character;
								v677.Text = "  [ HEALTH ] : " .. ((v1434 and v1434:FindFirstChild("Humanoid") and math.floor(v1434.Humanoid.Health)) or "DEAD");
								v1435 = v256(v619, "ChatTagText");
								v1436 = v256(v619, "ExactLocation");
								v1433 = 1;
							end
							if (v1433 == (4 + 0)) then
								table.sort(v1442);
								v1444 = {"  [ INVENTORY ]"};
								for v1699, v1700 in ipairs(v1442) do
									table.insert(v1444, "  - " .. v1700);
								end
								v705.Text = ((#v1442 > 0) and table.concat(v1444, "\n")) or "  [ INVENTORY ]\n  (Empty)";
								break;
							end
							if (v1433 == 3) then
								v1443 = nil;
								function v1443(v1701)
									for v1727, v1728 in pairs(v1701:GetChildren()) do
										if (v1728:IsA("Tool") and not v227[v1728.Name]) then
											table.insert(v1442, v1728.Name);
										end
									end
								end
								if v1434 then
									v1443(v1434);
								end
								v1443(v619.Backpack);
								v1433 = 1 + 3;
							end
							if (v1433 == (1 + 0)) then
								v685.Text = string.format("  タイトル: %s\n  現在の場所: %s", v1435, v1436);
								v1437 = v257(v619, "Defense");
								v1438 = v257(v619, "Demon Fruit");
								v1439 = v257(v619, "Gun");
								v1433 = 2;
							end
						end
					end
					task.wait(0.6);
					break;
				end
				if (v982 == (0 + 0)) then
					v983 = (v619.Team and v619.Team.Name) or "None";
					if string.find(string.lower(v983), "pirate") then
						v637.TextColor3 = Color3.fromRGB(255, 71 - 21, 96 - 46);
					elseif string.find(string.lower(v983), "marine") then
						v637.TextColor3 = Color3.fromRGB(136 - 86, 551 - 401, 143 + 112);
					else
						v637.TextColor3 = Color3.fromRGB(255, 255, 255);
					end
					v982 = 1;
				end
				if (v982 == (4 - 1)) then
					v649.Text = "Lv: " .. v984 .. " | " .. v985 .. " (" .. v986 .. ")";
					v658.Text = "Fragments: " .. v987;
					v982 = 4;
				end
			end
		end
	end);
end
for v717, v718 in pairs(v210:GetPlayers()) do
	v259(v718);
end
v210.PlayerAdded:Connect(v259);
v210.PlayerRemoving:Connect(function(v719)
	if v247:FindFirstChild(v719.Name) then
		v247[v719.Name]:Destroy();
	end
end);
local v260 = v102("VFXカラー");
local v261 = nil;
local v262 = nil;
local v263 = nil;
local v264 = Color3.new(1 + 0, 1 + 0, 1 + 0);
local v265 = false;
local function v266(v720)
	if not v262 then
		return;
	end
	local v721 = v262:FindFirstChild("Shifted");
	if v721 then
		for v1105, v1106 in pairs(v721:GetAttributes()) do
			if string.find(v1105:lower(), "shifted_color") then
				v721:SetAttribute(v1105, v720);
			end
		end
		for v1107, v1108 in pairs(v721:GetChildren()) do
			if (string.find(v1108.Name:lower(), "shifted_color") and v1108:IsA("Color3Value")) then
				v1108.Value = v720;
			end
		end
	end
end
local v267 = Instance.new("Frame", v260);
v267.Size = UDim2.new(3 - 2, 0 - 0, 0 + 0, 0 - 0);
v267.AutomaticSize = Enum.AutomaticSize.Y;
v267.BackgroundTransparency = 3 - 2;
v267.LayoutOrder = -10;
local v272 = Instance.new("UIListLayout", v267);
v272.Padding = UDim.new(0, 3 + 2);
local function v274()
	for v902, v903 in pairs(v267:GetChildren()) do
		if not v903:IsA("UIListLayout") then
			v903:Destroy();
		end
	end
	for v904, v905 in pairs(game.Players.LocalPlayer:GetChildren()) do
		if v905.Name:find("VFXColor") then
			local v1109 = 0 - 0;
			local v1110;
			while true do
				if (v1109 == 0) then
					v1110 = v905.Name:gsub("VFXColor", "");
					v105(v267, "👉 選択: " .. v1110, function()
						local v1446 = 831 - (762 + 69);
						while true do
							if (v1446 == (3 - 2)) then
								v12("Active: " .. v1110);
								if not v265 then
									v266(v264);
								end
								break;
							end
							if (v1446 == (0 + 0)) then
								v262 = v905;
								v261 = v905.Name;
								v1446 = 1 + 0;
							end
						end
					end);
					break;
				end
			end
		end
	end
end
game.Players.LocalPlayer.CharacterAdded:Connect(function()
	task.wait(2.5 - 1);
	v274();
	if v261 then
		local v988 = 0 + 0;
		local v989;
		while true do
			if ((0 + 0) == v988) then
				v989 = game.Players.LocalPlayer:FindFirstChild(v261);
				if v989 then
					v262 = v989;
					if v265 then
					else
						v266(v264);
					end
				end
				break;
			end
		end
	end
end);
game.Players.LocalPlayer.ChildAdded:Connect(function(v722)
	if v722.Name:find("VFXColor") then
		task.wait(0.1 - 0);
		v274();
	end
end);
game.Players.LocalPlayer.ChildRemoved:Connect(function(v723)
	if v723.Name:find("VFXColor") then
		local v990 = 0;
		local v991;
		while true do
			if (v990 == 0) then
				v991 = 157 - (8 + 149);
				while true do
					if (v991 == (1320 - (1199 + 121))) then
						task.wait(0.1 - 0);
						v274();
						break;
					end
				end
				break;
			end
		end
	end
end);
v105(v260, "🔥 GAMING RAINBOW (0.2s)", function()
	local v724 = 0 - 0;
	while true do
		if (v724 == 1) then
			if v263 then
				local v1288 = 0;
				local v1289;
				while true do
					if (v1288 == 0) then
						v1289 = 0 + 0;
						while true do
							if ((0 - 0) == v1289) then
								v263:Disconnect();
								v263 = nil;
								break;
							end
						end
						break;
					end
				end
			end
			if v265 then
				local v1290 = 0;
				while true do
					if (v1290 == 0) then
						v263 = game:GetService("RunService").Heartbeat:Connect(function()
							local v1581 = 0;
							local v1582;
							local v1583;
							while true do
								if (v1581 == (2 - 1)) then
									v266(Color3.fromHSV(v1583, 1 + 0, 1));
									break;
								end
								if (v1581 == (1807 - (518 + 1289))) then
									local v1729 = 0;
									while true do
										if (v1729 == (1 - 0)) then
											v1581 = 1 + 0;
											break;
										end
										if (v1729 == (0 - 0)) then
											v1582 = 0.2 + 0;
											v1583 = (tick() % v1582) / v1582;
											v1729 = 470 - (304 + 165);
										end
									end
								end
							end
						end);
						v12("Rainbow ON");
						break;
					end
				end
			else
				local v1291 = 0 + 0;
				local v1292;
				while true do
					if ((160 - (54 + 106)) == v1291) then
						v1292 = 0;
						while true do
							if (v1292 == 0) then
								v266(v264);
								v12("Rainbow OFF");
								break;
							end
						end
						break;
					end
				end
			end
			break;
		end
		if (v724 == (1969 - (1618 + 351))) then
			if not v262 then
				local v1293 = 0;
				while true do
					if (v1293 == 0) then
						v12("先にVFXを選択してください");
						return;
					end
				end
			end
			v265 = not v265;
			v724 = 1 + 0;
		end
	end
end);
local v275 = {{"Red",Color3.new(1 + 0, 0, 0 - 0)},{"Orange",Color3.new(1 + 0, 0.5 - 0, 0 + 0)},{"Yellow",Color3.new(3 - 2, 187 - (165 + 21), 111 - (61 + 50))},{"Lime",Color3.new(0.5 - 0, 1 + 0, 1460 - (1295 + 165))},{"Green",Color3.new(0 + 0, 1, 1397 - (819 + 578))},{"Mint",Color3.new(1282.4 - (546 + 736), 1938 - (1834 + 103), 0.6 + 0)},{"Aqua",Color3.new(0 + 0, 1, 0.8 - 0)},{"Cyan",Color3.new(0 - 0, 1, 2 - 1)},{"Sky",Color3.new(0.2 + 0, 0.6, 1 + 0)},{"Blue",Color3.new(0 - 0, 0 - 0, 1 + 0)},{"Purple",Color3.new(0.6, 0 - 0, 1)},{"Magenta",Color3.new(1400 - (653 + 746), 0 - 0, 1)},{"Pink",Color3.new(2 - 1, 0.4, 0.7)},{"White",Color3.new(1, 1 + 0, 1 + 0)},{"Gold",Color3.new(1 + 0, 0.8 - 0, 0)},{"Crimson",Color3.new(0.6, 0 - 0, 0)},{"Forest",Color3.new(801 - (768 + 33), 0.4 - 0, 0 - 0)},{"Navy",Color3.new(0, 0, 0.5)},{"Silver",Color3.new(1672.7 - (741 + 931), 0.7 + 0, 0.7)},{"Ghost",Color3.new(0.9, 0.9, 1 + 0)}};
for v725, v726 in pairs(v275) do
	v105(v260, "Color: " .. v726[1 + 0], function()
		local v906 = 0 - 0;
		while true do
			if (v906 == (0 + 0)) then
				v265 = false;
				if v263 then
					local v1369 = 0;
					while true do
						if (v1369 == (0 + 0)) then
							v263:Disconnect();
							v263 = nil;
							break;
						end
					end
				end
				v906 = 1;
			end
			if (v906 == (4 - 3)) then
				v264 = v726[2 + 0];
				v266(v726[496 - (64 + 430)]);
				break;
			end
		end
	end);
end
v274();
local v276 = v102("Sea Beast / Sea Event");
local v210 = game:GetService("Players");
local v147 = game:GetService("RunService");
local v277 = game:GetService("Workspace");
local v278 = game:GetService("ReplicatedStorage");
local v279 = game:GetService("VirtualInputManager");
local v1 = v210.LocalPlayer;
local v280 = v278.Remotes.CommF_;
local v281 = {DefaultY=(199 + 1),SeaBeastY=50,ShipY=(383 - (106 + 257)),MoveSpeed=(3 + 0),HuntTweenSpeed=(1071 - (496 + 225)),ReturnTweenSpeed=(511 - 261),BoatsPath=v277:WaitForChild("Boats"),SeaBeastsPath=v277:WaitForChild("SeaBeasts"),EnemiesPath=v277:WaitForChild("Enemies")};
local v282 = {Hunting=false,Terror=false,Shark=false,Piranha=false,Brigade=false,Fishman=false,Moving=false,Processing=false,LastSeat=nil};
local function v283(v727)
	if not (v727 and v727.Parent) then
		return false;
	end
	local v728 = v727:FindFirstChildOfClass("Humanoid");
	if v728 then
		return v728.Health > (0 - 0);
	end
	local v729 = v727:FindFirstChild("Health");
	if (v729 and v729:IsA("ValueBase")) then
		return v729.Value > 0;
	end
	return v727:FindFirstChild("HumanoidRootPart") or v727:FindFirstChildWhichIsA("BasePart", true);
end
local function v284()
	local v730 = 1658 - (256 + 1402);
	local v731;
	local v732;
	local v733;
	while true do
		if (v730 == 0) then
			v731 = 0;
			v732 = nil;
			v730 = 1900 - (30 + 1869);
		end
		if (v730 == (1370 - (213 + 1156))) then
			v733 = nil;
			while true do
				if (v731 == (188 - (96 + 92))) then
					v732 = v1.Character;
					v733 = v732 and v732:FindFirstChild("Humanoid");
					v731 = 1;
				end
				if (v731 == (1 + 0)) then
					if v733 then
						local v1522 = 899 - (142 + 757);
						while true do
							if (v1522 == (0 + 0)) then
								v733.Sit = false;
								task.wait(0.3);
								v1522 = 1 + 0;
							end
							if (v1522 == 1) then
								for v1730 = 80 - (32 + 47), 1982 - (1053 + 924) do
									if v732:FindFirstChildOfClass("Tool") then
										break;
									end
									v279:SendKeyEvent(true, Enum.KeyCode.Two, false, game);
									task.wait(0.05 + 0);
									v279:SendKeyEvent(false, Enum.KeyCode.Two, false, game);
									task.wait(0.1 - 0);
								end
								break;
							end
						end
					end
					break;
				end
			end
			break;
		end
	end
end
local function v285()
	for v907, v908 in ipairs({Enum.KeyCode.Z,Enum.KeyCode.X,Enum.KeyCode.C,Enum.KeyCode.F}) do
		v279:SendKeyEvent(true, v908, false, game);
		task.wait(0.01 - 0);
		v279:SendKeyEvent(false, v908, false, game);
	end
end
local function v286(v734, v735, v736)
	local v737 = 1709 - (541 + 1168);
	local v738;
	local v739;
	while true do
		if (v737 == 0) then
			if not (v734 and v734.Parent) then
				return;
			end
			v738 = v1.Character and v1.Character:FindFirstChild("HumanoidRootPart");
			v737 = 1598 - (645 + 952);
		end
		if (v737 == (839 - (669 + 169))) then
			if not v738 then
				return;
			end
			v739 = nil;
			v737 = 6 - 4;
		end
		if (v737 == 2) then
			v739 = v147.RenderStepped:Connect(function(v1203)
				local v1204 = 0;
				local v1205;
				local v1206;
				local v1207;
				while true do
					if (v1204 == (0 - 0)) then
						v1205 = 0 + 0;
						v1206 = nil;
						v1204 = 1;
					end
					if (v1204 == (1 + 0)) then
						v1207 = nil;
						while true do
							if (v1205 == 2) then
								v738.CFrame = CFrame.new(v738.Position + ((v1206 - v738.Position).Unit * v735 * v1203));
								v738.Velocity = Vector3.zero;
								break;
							end
							if (v1205 == 1) then
								v1207 = (v1206 - v738.Position).Magnitude;
								if (v1207 < (769 - (181 + 584))) then
									local v1731 = 0;
									local v1732;
									while true do
										if (v1731 == 0) then
											v1732 = 0;
											while true do
												if (v1732 == (1395 - (665 + 730))) then
													v738.CFrame = CFrame.new(v1206);
													v739:Disconnect();
													v1732 = 1;
												end
												if (v1732 == 1) then
													return;
												end
											end
											break;
										end
									end
								end
								v1205 = 5 - 3;
							end
							if (v1205 == (0 - 0)) then
								if not (v734 and v734.Parent and v738.Parent) then
									local v1733 = 1350 - (540 + 810);
									while true do
										if (v1733 == (0 - 0)) then
											v739:Disconnect();
											return;
										end
									end
								end
								v1206 = v734.Position + (v736 or Vector3.new(0 - 0, 0, 0));
								v1205 = 1 + 0;
							end
						end
						break;
					end
				end
			end);
			while v739.Connected do
				task.wait();
			end
			break;
		end
	end
end
local function v287()
	local v740 = 203 - (166 + 37);
	local v741;
	while true do
		if (v740 == (1882 - (22 + 1859))) then
			if v282.Brigade then
				for v1371, v1372 in pairs(v741) do
					if ((v1372.Name:find("Brigade") or v1372.Name:find("Ship") or v1372.Name:find("Boat")) and v283(v1372)) then
						return v1372, false, v281.ShipY;
					end
				end
			end
			if v282.Fishman then
				for v1373, v1374 in pairs(v741) do
					if ((v1374.Name:find("Fish") or v1374.Name:find("Crew")) and v283(v1374)) then
						local v1523 = 1772 - (843 + 929);
						local v1524;
						while true do
							if (v1523 == (262 - (30 + 232))) then
								v1524 = not v1374.Name:find("Boat");
								return v1374, v1524, (v1524 and v281.DefaultY) or v281.ShipY;
							end
						end
					end
				end
			end
			v740 = 5 - 3;
		end
		if (v740 == (779 - (55 + 722))) then
			if v282.Piranha then
				for v1375, v1376 in pairs(v741) do
					if ((v1376.Name == "Piranha") and v283(v1376)) then
						return v1376, true, v281.DefaultY;
					end
				end
			end
			if v282.Shark then
				for v1377, v1378 in pairs(v741) do
					if ((v1378.Name:find("Shark") or (v1378.Name == "Sharks")) and (v1378.Name ~= "Terrorshark") and v283(v1378)) then
						return v1378, true, v281.DefaultY;
					end
				end
			end
			v740 = 3;
		end
		if (v740 == (0 - 0)) then
			v741 = v281.EnemiesPath:GetChildren();
			if v282.Terror then
				for v1379, v1380 in pairs(v741) do
					if ((v1380.Name == "Terrorshark") and v283(v1380)) then
						return v1380, true, v281.DefaultY;
					end
				end
			end
			v740 = 1676 - (78 + 1597);
		end
		if (v740 == 3) then
			if v282.Hunting then
				for v1381, v1382 in pairs(v281.SeaBeastsPath:GetChildren()) do
					if v283(v1382) then
						return v1382, false, v281.SeaBeastY;
					end
				end
			end
			return nil;
		end
	end
end
local function v288()
	if v282.Processing then
		return;
	end
	local v742, v743, v744 = v287();
	if not v742 then
		return;
	end
	v282.Processing = true;
	v284();
	while true do
		v742, v743, v744 = v287();
		if not v742 then
			break;
		end
		local v909 = v1.Character:FindFirstChild("HumanoidRootPart");
		local v910 = v742:FindFirstChild("HumanoidRootPart") or v742:FindFirstChildWhichIsA("BasePart", true);
		if v910 then
			v286(v910, v281.HuntTweenSpeed, (v743 and Vector3.new(0 + 0, 14 + 1, 0 + 0)) or Vector3.new(549 - (305 + 244), v744 - v910.Position.Y, 0 + 0));
			while v283(v742) and (v282.Hunting or v282.Terror or v282.Shark or v282.Piranha or v282.Brigade or v282.Fishman) do
				if v743 then
					v909.CFrame = v910.CFrame * CFrame.new(0, 20, 105 - (95 + 10));
				else
					v909.CFrame = CFrame.new(v910.Position.X, v744, v910.Position.Z);
				end
				v909.Velocity = Vector3.zero;
				v285();
				v147.Heartbeat:Wait();
				if not (v282.Hunting or v282.Terror or v282.Shark or v282.Piranha or v282.Brigade or v282.Fishman) then
					break;
				end
			end
		end
		task.wait(0.2 + 0);
	end
	if (v282.LastSeat and v282.LastSeat.Parent) then
		v286(v282.LastSeat, v281.ReturnTweenSpeed, Vector3.new(0 - 0, 3 - 0, 0));
		task.wait(762.3 - (592 + 170));
		pcall(function()
			v282.LastSeat:Sit(v1.Character.Humanoid);
		end);
	end
	v282.Processing = false;
end
v281.SeaBeastsPath.ChildAdded:Connect(function()
	task.spawn(v288);
end);
v281.EnemiesPath.ChildAdded:Connect(function()
	task.spawn(v288);
end);
v104(v276, "Hunt Speed", 348 - 248, 500, 878 - 528, function(v746)
	v281.HuntTweenSpeed = v746;
end);
v103(v276, "AUTO MOVE", false, function(v748)
	v282.Moving = v748;
end);
v103(v276, "SEA BEAST", false, function(v750)
	v282.Hunting = v750;
end);
v103(v276, "TERROR SHARK", false, function(v752)
	v282.Terror = v752;
end);
v103(v276, "SHARKS", false, function(v754)
	v282.Shark = v754;
end);
v103(v276, "PIRANHA", false, function(v756)
	v282.Piranha = v756;
end);
v103(v276, "PIRATE SHIPS", false, function(v758)
	v282.Brigade = v758;
end);
v103(v276, "FISHMAN / BOAT", false, function(v760)
	v282.Fishman = v760;
end);
v105(v276, "RETURN TO BOAT", function()
	local v762 = 0 + 0;
	local v763;
	while true do
		if (0 == v762) then
			v763 = 0 + 0;
			while true do
				if (v763 == (0 - 0)) then
					if v282.Processing then
						return;
					end
					if (v282.LastSeat and v282.LastSeat.Parent) then
						task.spawn(function()
							v282.Processing = true;
							v286(v282.LastSeat, v281.ReturnTweenSpeed, Vector3.new(0 + 0, 5 - 2, 507 - (353 + 154)));
							task.wait(0.3);
							pcall(function()
								v282.LastSeat:Sit(v1.Character.Humanoid);
							end);
							v282.Processing = false;
						end);
					end
					break;
				end
			end
			break;
		end
	end
end);
do
	local v764 = {{"Dinghy",false},{"Sloop",true},{"Brigade",true},{"Grand Brigade",true},{"Miracle",false,true},{"The Sentinel",false,true},{"Guardian",false,true},{"Lantern",false,true},{"Sleigh",false,true},{"Beast Hunter",false,true}};
	for v911, v912 in ipairs(v764) do
		v105(v276, "Buy: " .. v912[1 - 0], function()
			local v992 = 0;
			local v993;
			local v994;
			local v995;
			while true do
				if (v992 == 0) then
					v993 = (v912[3] and "Luxury Boat Dealer") or "Boat Dealer";
					v994 = ((v1.Team.Name == "Marines") and "Marine") or "Pirate";
					v992 = 231 - (19 + 211);
				end
				if (v992 == 2) then
					for v1385, v1386 in ipairs(v995) do
						if (v280:InvokeServer("BuyBoat", v1386, v993) ~= 0) then
							task.wait(114 - (88 + 25));
							local v1525 = v1.Character.HumanoidRootPart;
							local v1526 = nil;
							local v1527 = 2543 - 1544;
							for v1585, v1586 in pairs(v281.BoatsPath:GetChildren()) do
								local v1587 = 0;
								local v1588;
								while true do
									if (v1587 == 0) then
										v1588 = v1586:FindFirstChildWhichIsA("BasePart", true);
										if (v1588 and ((v1588.Position - v1525.Position).Magnitude < v1527)) then
											v1527 = (v1588.Position - v1525.Position).Magnitude;
											v1526 = v1586;
										end
										break;
									end
								end
							end
							if v1526 then
								local v1679 = v1526:FindFirstChildWhichIsA("VehicleSeat", true);
								if v1679 then
									v282.LastSeat = v1679;
									v286(v1679, 125 + 125, Vector3.new(0, 3 + 0, 0));
									task.wait(1036.2 - (1007 + 29));
									pcall(function()
										v1679:Sit(v1.Character.Humanoid);
									end);
								end
							end
							break;
						end
					end
					break;
				end
				if ((1 + 0) == v992) then
					v280:InvokeServer("BuyBoat", "Speak");
					v995 = {v912[1],(v994 .. v912[1 + 0]),(v994 .. " " .. v912[2 - 1])};
					v992 = 2;
				end
			end
		end);
	end
end
v147.Heartbeat:Connect(function()
	local v765 = 0;
	local v766;
	local v767;
	local v768;
	while true do
		if (v765 == (591 - (276 + 313))) then
			if (v768.SeatPart and v768.SeatPart:IsA("VehicleSeat")) then
				v282.LastSeat = v768.SeatPart;
			end
			if (v282.Moving and not v282.Processing and v282.LastSeat and v768.Sit) then
				local v1296 = 0 - 0;
				local v1297;
				while true do
					if (v1296 == 1) then
						v767.CFrame = CFrame.new(v767.Position.X, v281.DefaultY, v767.Position.Z) * (v767.CFrame - v767.CFrame.Position);
						break;
					end
					if (v1296 == (0 + 0)) then
						v1297 = Vector3.new(v767.CFrame.LookVector.X, 0 + 0, v767.CFrame.LookVector.Z).Unit;
						v767.CFrame = CFrame.new(v767.Position + (v1297 * v281.MoveSpeed), v767.Position + (v1297 * v281.MoveSpeed) + v767.CFrame.LookVector);
						v1296 = 1 + 0;
					end
				end
			end
			v765 = 1975 - (495 + 1477);
		end
		if (v765 == (8 - 5)) then
			if not v282.Processing then
				if v287() then
					task.spawn(v288);
				end
			end
			break;
		end
		if (0 == v765) then
			v766 = v1.Character;
			v767 = v766 and v766:FindFirstChild("HumanoidRootPart");
			v765 = 1;
		end
		if (v765 == (1 + 0)) then
			v768 = v766 and v766:FindFirstChild("Humanoid");
			if not (v767 and v768) then
				return;
			end
			v765 = 2;
		end
	end
end);
local function v289(v769)
	local v770 = 403 - (342 + 61);
	local v771;
	while true do
		if (v770 == 0) then
			v771 = game.Players.LocalPlayer.Character;
			if (v771 and v771:FindFirstChild("HumanoidRootPart")) then
				v771.HumanoidRootPart.CFrame = CFrame.new(v769);
				v12("Teleported to Location");
			end
			break;
		end
	end
end
v105(v108, "Mansion (マンション)", function()
	v289(Vector3.new(-(5447.860000000001 + 7008), 541.3399999999999 - (4 + 161), -(4632.61 + 2933)));
end);
v105(v108, "Hydra Island (ヒドラ)", function()
	v289(Vector3.new(17732.43 - 12083, 1015.29, -341.05));
end);
v105(v108, "Sea Castle (海の城)", function()
	v289(Vector3.new(-5029.62, 827.97 - 512, -3195.88));
end);
local v290 = v102("stats");
local function v291(v772)
	local v773 = 497 - (322 + 175);
	local v774;
	local v775;
	local v776;
	while true do
		if (v773 == (563 - (173 + 390))) then
			v774 = 0;
			v775 = nil;
			v773 = 1;
		end
		if (v773 == 1) then
			v776 = nil;
			while true do
				local v1210 = 0;
				while true do
					if (v1210 == (0 + 0)) then
						if (v774 == (314 - (203 + 111))) then
							v775 = Instance.new("TextLabel", v290);
							v775.Size = UDim2.new(1, -10, 0 + 0, 35);
							v775.BackgroundColor3 = Color3.fromRGB(15 + 5, 0, 0);
							v775.TextColor3 = Color3.fromRGB(255, 255, 744 - 489);
							v774 = 1;
						end
						if (v774 == (2 + 0)) then
							v776 = Instance.new("UIPadding", v775);
							v776.PaddingLeft = UDim.new(706 - (57 + 649), 394 - (328 + 56));
							return v775;
						end
						v1210 = 1 + 0;
					end
					if (v1210 == (513 - (433 + 79))) then
						if (v774 == 1) then
							v775.Font = Enum.Font.SourceSansBold;
							v775.TextSize = 2 + 13;
							v775.TextXAlignment = Enum.TextXAlignment.Left;
							Instance.new("UICorner", v775);
							v774 = 2;
						end
						break;
					end
				end
			end
			break;
		end
	end
end
local v292 = v291("Server ID: Loading...");
local v293 = v291("滞在時間: 00:00:00");
local v294 = v291("FPS: 0");
local v295 = v291("Ping: 0 ms");
v105(v290, "サーバーIDをコピー", function()
	setclipboard(game.JobId);
	v12("サーバーIDをクリップボードにコピーしました");
end);
local v147 = game:GetService("RunService");
local v296 = game:GetService("Stats");
local v297 = os.time();
task.spawn(function()
	local v777 = 0 + 0;
	local v778;
	while true do
		if (v777 == 0) then
			v778 = 0 - 0;
			while true do
				if (v778 == (0 - 0)) then
					v292.Text = "Server ID: " .. (((game.JobId ~= "") and game.JobId) or "Studio/Private");
					while task.wait(0.5 + 0) do
						local v1447 = 0 + 0;
						local v1448;
						local v1449;
						local v1450;
						local v1451;
						local v1452;
						local v1453;
						local v1454;
						while true do
							if (v1447 == 2) then
								v1452 = nil;
								v1453 = nil;
								v1447 = 1039 - (562 + 474);
							end
							if (v1447 == 3) then
								v1454 = nil;
								while true do
									if (v1448 == 1) then
										v1451 = math.floor((v1449 % (8398 - 4798)) / (122 - 62));
										v1452 = v1449 % (965 - (76 + 829));
										v1448 = 1675 - (1506 + 167);
									end
									if (v1448 == (5 - 2)) then
										v294.Text = "FPS: " .. v1453;
										v1454 = math.floor(v296.Network.ServerStatsItem["Data Ping"]:GetValue());
										v1448 = 4;
									end
									if (v1448 == 0) then
										v1449 = os.time() - v297;
										v1450 = math.floor(v1449 / (3866 - (58 + 208)));
										v1448 = 1;
									end
									if (v1448 == 2) then
										v293.Text = string.format("滞在時間: %02d:%02d:%02d", v1450, v1451, v1452);
										v1453 = math.floor((1 + 0) / v147.RenderStepped:Wait());
										v1448 = 3;
									end
									if (v1448 == (3 + 1)) then
										v295.Text = "Ping: " .. v1454 .. " ms";
										break;
									end
								end
								break;
							end
							if (0 == v1447) then
								v1448 = 0 + 0;
								v1449 = nil;
								v1447 = 1;
							end
							if (v1447 == (3 - 2)) then
								v1450 = nil;
								v1451 = nil;
								v1447 = 339 - (258 + 79);
							end
						end
					end
					break;
				end
			end
			break;
		end
	end
end);
local v298 = v291("--- 出現中のボス ---");
v298.TextColor3 = Color3.fromRGB(33 + 222, 50, 0 - 0);
local v300 = Instance.new("ScrollingFrame", v290);
v300.Size = UDim2.new(1471 - (1219 + 251), -10, 0, 1821 - (1231 + 440));
v300.BackgroundTransparency = 59 - (34 + 24);
v300.BorderSizePixel = 0 + 0;
v300.ScrollBarThickness = 5 - 2;
v300.CanvasSize = UDim2.new(0, 0, 0 + 0, 0);
v300.AutomaticCanvasSize = Enum.AutomaticSize.Y;
local v307 = Instance.new("TextLabel", v300);
v307.Size = UDim2.new(2 - 1, 0 - 0, 0, 0 - 0);
v307.AutomaticSize = Enum.AutomaticSize.Y;
v307.BackgroundTransparency = 3 - 2;
v307.TextColor3 = Color3.fromRGB(255, 556 - 301, 1844 - (877 + 712));
v307.Font = Enum.Font.SourceSansBold;
v307.TextSize = 9 + 6;
v307.TextXAlignment = Enum.TextXAlignment.Left;
v307.TextYAlignment = Enum.TextYAlignment.Top;
v307.TextWrapped = true;
v307.Text = "待機中...";
local v319 = {};
local v320 = {};
local v321 = false;
local function v322(v779)
	return v779:gsub("%[Lv%. %d+%]%s*", ""):gsub("%[Boss%]", ""):match("^%s*(.-)%s*$");
end
local function v323()
	local v780 = 0;
	local v781;
	while true do
		if (v780 == (754 - (242 + 512))) then
			v781 = 0;
			while true do
				if (v781 == (0 - 0)) then
					if v321 then
						return;
					end
					v321 = true;
					v781 = 628 - (92 + 535);
				end
				if (v781 == (1 + 0)) then
					task.delay(0.5 - 0, function()
						local v1455 = 0 + 0;
						local v1456;
						local v1457;
						while true do
							if (v1455 == 0) then
								v1456 = {};
								for v1703, v1704 in pairs(v320) do
									table.insert(v1456, v1704 .. " " .. v1703);
								end
								v1455 = 1;
							end
							if ((3 - 2) == v1455) then
								local v1680 = 0 + 0;
								while true do
									if (v1680 == (1 + 0)) then
										v1455 = 1 + 1;
										break;
									end
									if (v1680 == (0 - 0)) then
										v1457 = ((#v1456 > 0) and table.concat(v1456, "\n")) or "なし";
										if (v307.Text ~= v1457) then
											v307.Text = v1457;
										end
										v1680 = 1 - 0;
									end
								end
							end
							if (v1455 == (1787 - (1476 + 309))) then
								v321 = false;
								break;
							end
						end
					end);
					break;
				end
			end
			break;
		end
	end
end
local function v324()
	local v782 = 1284 - (299 + 985);
	local v783;
	local v784;
	while true do
		if (v782 == (1 + 1)) then
			if v784 then
				local v1299 = 0 - 0;
				local v1300;
				while true do
					if (v1299 == (93 - (86 + 7))) then
						v1300 = nil;
						function v1300(v1598)
							local v1599 = 0 - 0;
							local v1600;
							while true do
								if (v1599 == (0 + 0)) then
									v1600 = v322(v1598.Name);
									if (v319[v1600] or v1598.Name:find("%[Boss%]")) then
										v319[v1600] = true;
										v320[v1600] = "⚔️";
										v323();
									end
									break;
								end
							end
						end
						v1299 = 881 - (672 + 208);
					end
					if (v1299 == (1 + 1)) then
						for v1601, v1602 in pairs(v784:GetChildren()) do
							v1300(v1602);
						end
						break;
					end
					if (v1299 == (133 - (14 + 118))) then
						v784.ChildAdded:Connect(v1300);
						v784.ChildRemoved:Connect(function(v1603)
							local v1604 = v322(v1603.Name);
							if (v320[v1604] == "⚔️") then
								local v1705 = 445 - (339 + 106);
								local v1706;
								while true do
									if (v1705 == (0 + 0)) then
										v1706 = 0 + 0;
										while true do
											if (v1706 == (1395 - (440 + 955))) then
												v320[v1604] = nil;
												v323();
												break;
											end
										end
										break;
									end
								end
							end
						end);
						v1299 = 2 + 0;
					end
				end
			end
			break;
		end
		if (v782 == (1 - 0)) then
			v784 = game:GetService("Workspace"):FindFirstChild("Enemies");
			if v783 then
				local function v1301(v1388)
					if v1388.Name:find("%[Boss%]") then
						local v1531 = 0 + 0;
						local v1532;
						while true do
							if (v1531 == 0) then
								v1532 = v322(v1388.Name);
								v319[v1532] = true;
								v1531 = 2 - 1;
							end
							if (v1531 == 1) then
								v320[v1532] = "📍";
								v323();
								break;
							end
						end
					end
				end
				v783.ChildAdded:Connect(v1301);
				v783.ChildRemoved:Connect(function(v1389)
					local v1390 = 0 + 0;
					local v1391;
					while true do
						if (v1390 == (353 - (260 + 93))) then
							v1391 = v322(v1389.Name);
							if (v320[v1391] == "📍") then
								local v1709 = 0 + 0;
								local v1710;
								while true do
									if ((0 - 0) == v1709) then
										v1710 = 0 - 0;
										while true do
											if (v1710 == (1974 - (1181 + 793))) then
												v320[v1391] = nil;
												v323();
												break;
											end
										end
										break;
									end
								end
							end
							break;
						end
					end
				end);
				for v1392, v1393 in pairs(v783:GetChildren()) do
					v1301(v1393);
				end
			end
			v782 = 1 + 1;
		end
		if (v782 == (307 - (105 + 202))) then
			v783 = game:GetService("Workspace"):FindFirstChild("_WorldOrigin");
			if v783 then
				v783 = v783:FindFirstChild("EnemySpawns");
			end
			v782 = 1 + 0;
		end
	end
end
task.spawn(v324);
local v325 = v291("--- 特殊島 出現状況 ---");
v325.TextColor3 = Color3.fromRGB(255, 860 - (352 + 458), 0);
local function v327(v785)
	local v786 = v291(v785 .. " : ❌");
	v786.TextSize = 14;
	return v786;
end
local v328 = v327("Mirage Island");
local v329 = v327("Kitsune Island");
local v330 = v327("Frozen Dimension");
local v331 = v327("Prehistoric Island");
local v332 = {["Mirage Island"]=v328,["Kitsune Island"]=v329,["Frozen Dimension"]=v330,["Prehistoric Island"]=v331};
task.spawn(function()
	local v788 = 0 - 0;
	local v789;
	while true do
		if (v788 == 0) then
			v789 = game:GetService("Workspace"):FindFirstChild("Map");
			while task.wait(7 - 4) do
				if not v789 then
					continue;
				end
				for v1302, v1303 in pairs(v332) do
					v1303.Text = v1302 .. " : ❌";
					v1303.TextColor3 = Color3.fromRGB(150, 150, 150);
				end
				for v1306, v1307 in pairs(v789:GetChildren()) do
					if v332[v1307.Name] then
						v332[v1307.Name].Text = v1307.Name .. " : ⭕";
						v332[v1307.Name].TextColor3 = Color3.fromRGB(0, 247 + 8, 0);
					end
				end
			end
			break;
		end
	end
end);
local v217 = -(584586.48 - 384590);
local v333 = false;
local v218 = nil;
local v334 = {};
local v335 = false;
v9.FinalZ = v9.FinalZ or false;
local function v337()
	local v790 = 949 - (438 + 511);
	while true do
		if (v790 == (1384 - (1262 + 121))) then
			if (v1.Character and v1.Character:FindFirstChild("Humanoid")) then
				workspace.CurrentCamera.CameraSubject = v1.Character.Humanoid;
			end
			if v218 then
				local v1310 = v1.Character and v1.Character:FindFirstChild("HumanoidRootPart");
				if (v1310 and (v1.Character.Humanoid.Health > 0)) then
					v1310.CFrame = v218.HumanoidRootPart.CFrame;
				end
				v218:Destroy();
				v218 = nil;
			end
			break;
		end
		if ((1068 - (728 + 340)) == v790) then
			v333 = false;
			workspace.CurrentCamera.CameraType = Enum.CameraType.Custom;
			v790 = 1791 - (816 + 974);
		end
	end
end
local function v338(v791)
	local v792 = 0;
	local v793;
	local v794;
	while true do
		if (v792 == 0) then
			if (v333 or not v9.FinalZ) then
				return;
			end
			v333 = true;
			v793 = v1.Character;
			v794 = v793 and v793:FindFirstChild("HumanoidRootPart");
			v792 = 2 - 1;
		end
		if (v792 == 2) then
			for v1211, v1212 in ipairs(v218:GetDescendants()) do
				if v1212:IsA("BasePart") then
					v1212.CanCollide = false;
				end
			end
			v218.HumanoidRootPart.CFrame = CFrame.new(v791 + Vector3.new(0, 10 - 7, 339 - (163 + 176)));
			workspace.CurrentCamera.CameraSubject = v218.Humanoid;
			task.spawn(function()
				local v1213 = 0 - 0;
				local v1214;
				while true do
					if (v1213 == 1) then
						v337();
						break;
					end
					if (v1213 == (0 - 0)) then
						v1214 = tick();
						while v333 and v9.FinalZ do
							if (((tick() - v1214) > (1.5 + 0)) or (v793.Humanoid.Health <= 0)) then
								break;
							end
							v794.CFrame = CFrame.new(v794.Position.X, v217, v794.Position.Z);
							v794.AssemblyLinearVelocity = Vector3.zero;
							game:GetService("RunService").Heartbeat:Wait();
						end
						v1213 = 1;
					end
				end
			end);
			break;
		end
		if (v792 == 1) then
			if not v794 then
				return;
			end
			v793.Archivable = true;
			v218 = v793:Clone();
			v218.Parent = workspace;
			v792 = 1812 - (1564 + 246);
		end
	end
end
local function v339(v795)
	local v796 = v795:WaitForChild("Humanoid");
	v795.ChildAdded:Connect(function(v913)
		if ((v913.Name == "TridentGrabZ") and v9.FinalZ) then
			local v1121 = 345 - (124 + 221);
			local v1122;
			local v1123;
			while true do
				if (v1121 == (1 + 0)) then
					v1123 = ((typeof(v1122) == "Vector3") and v1122) or (v1122:IsA("Model") and v1122:FindFirstChild("HumanoidRootPart") and v1122.HumanoidRootPart.Position);
					if v1123 then
						v338(v1123);
					end
					break;
				end
				if (v1121 == 0) then
					task.wait();
					v1122 = v913.Value;
					v1121 = 1;
				end
			end
		end
	end);
	v796.AnimationPlayed:Connect(function(v914)
		if (v914.Name == "Saddi_Z_Attack") then
			local v1124 = 451 - (115 + 336);
			while true do
				if (v1124 == 0) then
					v335 = true;
					task.delay(1, function()
						v335 = false;
					end);
					break;
				end
			end
		end
	end);
	game:GetService("RunService").Heartbeat:Connect(function()
		if (not v335 or not v9.FinalZ) then
			return;
		end
		local v915 = v795:FindFirstChild("HumanoidRootPart");
		if not v915 then
			return;
		end
		for v996, v997 in ipairs(game.Players:GetPlayers()) do
			if ((v997 ~= v1) and v997.Character) then
				local v1215 = 0;
				local v1216;
				local v1217;
				local v1218;
				while true do
					if (v1215 == (1 - 0)) then
						v1218 = nil;
						while true do
							if (v1216 == 0) then
								v1217 = v997.Character:FindFirstChildOfClass("Humanoid");
								v1218 = v997.Character:FindFirstChild("HumanoidRootPart");
								v1216 = 1;
							end
							if ((1 + 0) == v1216) then
								if (v1217 and v1218 and (v1217.Health > (46 - (45 + 1)))) then
									if (v334[v997] and (v1217.Health < v334[v997])) then
										if ((v1218.Position - v915.Position).Magnitude < (7 + 113)) then
											local v1806 = 0;
											while true do
												if (v1806 == (1990 - (1282 + 708))) then
													v335 = false;
													v338(v1218.Position);
													break;
												end
											end
										end
									end
									v334[v997] = v1217.Health;
								end
								break;
							end
						end
						break;
					end
					if (v1215 == 0) then
						v1216 = 1212 - (583 + 629);
						v1217 = nil;
						v1215 = 1 + 0;
					end
				end
			end
		end
	end);
end
if v1.Character then
	v339(v1.Character);
end
v1.CharacterAdded:Connect(v339);
if v108 then
	v103(v108, "Final-Z (Trident/Saddi)", v9.FinalZ, function(v998)
		local v999 = 0;
		while true do
			if (0 == v999) then
				v9.FinalZ = v998;
				if not v998 then
					v337();
				end
				break;
			end
		end
	end);
end
local function v340(v797)
	local v798 = 0;
	local v799;
	local v800;
	local v801;
	while true do
		if ((2 - 1) == v798) then
			v801 = nil;
			while true do
				if (v799 == 0) then
					v800 = game:GetService("ReplicatedStorage"):WaitForChild("Remotes");
					v801 = {"CommF","CommF_","CommE"};
					v799 = 1;
				end
				if (v799 == (1 + 0)) then
					for v1462, v1463 in pairs(v801) do
						local v1464 = 0;
						local v1465;
						while true do
							if (v1464 == (1631 - (1539 + 92))) then
								v1465 = v800:FindFirstChild(v1463);
								if v1465 then
									pcall(function()
										if v1465:IsA("RemoteFunction") then
											v1465:InvokeServer("SetTeam", v797);
										else
											v1465:FireServer("SetTeam", v797);
										end
									end);
								end
								break;
							end
						end
					end
					v12("Team changed to: " .. v797);
					break;
				end
			end
			break;
		end
		if (v798 == (1946 - (706 + 1240))) then
			v799 = 0;
			v800 = nil;
			v798 = 259 - (81 + 177);
		end
	end
end
if v108 then
	local v916 = 0;
	local v917;
	while true do
		if (v916 == 2) then
			v917.TextColor3 = Color3.fromRGB(720 - 465, 255, 255);
			v917.Font = Enum.Font.SourceSansBold;
			v916 = 260 - (212 + 45);
		end
		if ((9 - 6) == v916) then
			v917.TextSize = 16;
			v105(v108, "Pirate", function()
				v340("Pirates");
			end);
			v916 = 1950 - (708 + 1238);
		end
		if (v916 == (1 + 0)) then
			v917.BackgroundTransparency = 1;
			v917.Text = "--- Team Changer ---";
			v916 = 1 + 1;
		end
		if (v916 == 4) then
			v105(v108, "Marine", function()
				v340("Marines");
			end);
			break;
		end
		if (v916 == 0) then
			v917 = Instance.new("TextLabel", v108);
			v917.Size = UDim2.new(1668 - (586 + 1081), -(521 - (348 + 163)), 0 + 0, 30);
			v916 = 1;
		end
	end
end
local v278 = game:GetService("ReplicatedStorage");
local v147 = game:GetService("RunService");
local v341 = v278:WaitForChild("Modules"):WaitForChild("Net");
local v342 = v341["RE/RegisterAttack"];
local v343 = v341["RE/RegisterHit"];
local v344 = v341["RE/ShootGunEvent"];
v9.GunM1 = false;
local v346 = 160;
local v347 = 282 - (215 + 65);
local function v348()
	local v802 = 0 - 0;
	local v803;
	local v804;
	local v805;
	local v806;
	while true do
		if (v802 == (1860 - (1541 + 318))) then
			if not v804 then
				return nil;
			end
			v805, v806 = nil, v346;
			v802 = 2 + 0;
		end
		if (v802 == (2 + 0)) then
			local v1125 = 0 + 0;
			while true do
				if (v1125 == (1750 - (1036 + 714))) then
					for v1466, v1467 in pairs({workspace:FindFirstChild("Enemies"),workspace:FindFirstChild("Characters")}) do
						if v1467 then
							for v1681, v1682 in pairs(v1467:GetChildren()) do
								if ((v1682 ~= v803) and v1682:FindFirstChild("Humanoid") and (v1682.Humanoid.Health > (0 + 0))) then
									local v1737 = 0 + 0;
									local v1738;
									while true do
										if (v1737 == (1280 - (883 + 397))) then
											v1738 = v1682:FindFirstChild("HumanoidRootPart");
											if (v1738 and ((v804.Position - v1738.Position).Magnitude < v806)) then
												v806 = (v804.Position - v1738.Position).Magnitude;
												v805 = {v1682,v1738};
											end
											break;
										end
									end
								end
							end
						end
					end
					return v805;
				end
			end
		end
		if (v802 == 0) then
			v803 = v1.Character;
			v804 = v803 and v803:FindFirstChild("HumanoidRootPart");
			v802 = 591 - (563 + 27);
		end
	end
end
v147.Stepped:Connect(function()
	if not v9.GunM1 then
		return;
	end
	local v807 = v1.Character;
	local v808 = v807 and v807:FindFirstChildOfClass("Tool");
	if not v808 then
		return;
	end
	local v809 = v348();
	if not v809 then
		return;
	end
	local v810, v811 = v809[3 - 2], v809[2];
	pcall(function()
		local v918 = 1986 - (1369 + 617);
		local v919;
		while true do
			if (v918 == (1487 - (85 + 1402))) then
				v919 = 0 + 0;
				while true do
					if (v919 == 1) then
						if v808:FindFirstChild("LeftClickRemote") then
							v808.LeftClickRemote:FireServer((v811.Position - v807:GetPivot().Position).Unit, 2 - 1);
						end
						break;
					end
					if ((403 - (274 + 129)) == v919) then
						for v1536 = 218 - (12 + 205), v347 do
							v342:FireServer(0 + 0);
							v343:FireServer(v811, {{v810,v811}});
						end
						if (v808.ToolTip == "Gun") then
							local v1605 = 480 - (91 + 389);
							local v1606;
							local v1607;
							while true do
								if (v1605 == (297 - (90 + 207))) then
									v344:FireServer(v811.Position, {v811});
									v808:Activate();
									v1605 = 1;
								end
								if ((862 - (706 + 155)) == v1605) then
									v1606 = v808:FindFirstChild("RemoteEvent") or v808:FindFirstChildOfClass("RemoteEvent");
									if v1606 then
										v1606:FireServer("Down", v811.Position);
									end
									v1605 = 1797 - (730 + 1065);
								end
								if (v1605 == (1565 - (1339 + 224))) then
									v1607 = v807:FindFirstChildOfClass("Humanoid");
									if v1607 then
										for v1794, v1795 in pairs(v1607:GetPlayingAnimationTracks()) do
											if (v1795.Name:lower():find("gun") or v1795.Name:lower():find("shoot")) then
												v1795:AdjustSpeed(2);
											end
										end
									end
									break;
								end
							end
						end
						v919 = 1 + 0;
					end
				end
				break;
			end
		end
	end);
end);
if v108 then
	v103(v108, "gun m1", v9.GunM1, function(v1000)
		local v1001 = 0;
		while true do
			if (0 == v1001) then
				v9.GunM1 = v1000;
				if v1000 then
					v12("gun m1 有効");
				else
					v12("gun m1 無効");
				end
				break;
			end
		end
	end);
end
local v349 = game:GetService("RunService");
local v350 = 624 + 76;
local v351 = {"LeftUpperArm","LeftLowerArm","LeftHand","RightUpperArm","RightLowerArm","RightHand"};
v9.BigBuddha = false;
local function v353()
	local v812 = 0;
	local v813;
	while true do
		if ((1805 - (323 + 1482)) == v812) then
			if not v9.BigBuddha then
				return;
			end
			v813 = v1.Character;
			v812 = 1919 - (1177 + 741);
		end
		if (v812 == 2) then
			v1.CameraMaxZoomDistance = 10 + 130;
			break;
		end
		if (v812 == 1) then
			if not v813 then
				return;
			end
			for v1226, v1227 in pairs(v351) do
				local v1228 = 0 - 0;
				local v1229;
				while true do
					if (v1228 == (0 + 0)) then
						v1229 = v813:FindFirstChild(v1227);
						if (v1229 and v1229:IsA("BasePart")) then
							v1229.CanQuery = false;
							local v1609 = v1229:FindFirstChildOfClass("SpecialMesh") or Instance.new("SpecialMesh", v1229);
							v1609.MeshType = Enum.MeshType.Brick;
							v1609.Scale = Vector3.new(v350 * (0.1 - 0), v350, v350 * (0.1 + 0));
							v1229.Color = Color3.new(1, 1, 110 - (96 + 13));
							v1229.Material = Enum.Material.Neon;
							v1229.Transparency = 0.5;
							local v1617 = v1229:FindFirstChildOfClass("Motor6D");
							if v1617 then
								v1617.C0 = CFrame.new(v1617.C0.Position.X, 1921 - (962 + 959), v1617.C0.Position.Z) * CFrame.new(0, v350 / 2, 0);
							end
						end
						break;
					end
				end
			end
			v812 = 4 - 2;
		end
	end
end
v349.RenderStepped:Connect(function()
	if v9.BigBuddha then
		pcall(v353);
	end
end);
if v108 then
	v103(v108, "大仏の範囲でかくなる", v9.BigBuddha, function(v1002)
		local v1003 = 0;
		while true do
			if (v1003 == (0 + 0)) then
				v9.BigBuddha = v1002;
				if not v1002 then
					local v1468 = 1351 - (461 + 890);
					while true do
						if (v1468 == (0 + 0)) then
							v1.CameraMaxZoomDistance = 128;
							v12("大仏範囲: OFF (戻すには再スポーン推奨)");
							break;
						end
					end
				else
					v12("大仏範囲: ON ");
				end
				break;
			end
		end
	end);
end
