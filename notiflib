local Lib = {}

function Lib:NewNotif(player, title, body, buttons, isFPS)
	if isFPS then
		if type(isFPS) == "boolean" then
			game:GetService("UserInputService").MouseIconEnabled = isFPS
		else
			isFPS = false
		end
	end
	local Closed = false
	
	if not title or not type(title) == "string" then title = "Title" end
	if not body or not type(body) == "string" then body = "Body" end --Checking if there's values

	local Notification = Instance.new("ScreenGui")
	local Main = Instance.new("Frame")
	local Head = Instance.new("TextLabel")
	local Body = Instance.new("TextLabel")
	local Buttons1 = Instance.new("Frame")
	local Button = Instance.new("TextButton")
	local Buttons2 = Instance.new("Frame")
	local Button_2 = Instance.new("TextButton")
	local Button2 = Instance.new("TextButton")
	local UICorner1 = Instance.new("UICorner")
	local UICorner2 = Instance.new("UICorner")
	local UICorner3 = Instance.new("UICorner")
	local UICorner4 = Instance.new("UICorner")

	UICorner1.Parent = Main
	UICorner1.CornerRadius = UDim.new(0.05, 0)

	UICorner2.Parent = Button
	UICorner2.CornerRadius = UDim.new(0.25, 0)

	UICorner3.Parent = Button_2
	UICorner3.CornerRadius = UDim.new(0.25, 0)

	UICorner4.Parent = Button2
	UICorner4.CornerRadius = UDim.new(0.25, 0)

	Notification.Name = "Notification"
	Notification.Parent = player.PlayerGui
	Notification.ZIndexBehavior = Enum.ZIndexBehavior.Global

	Main.Name = "Main"
	Main.Parent = Notification
	Main.BackgroundColor3 = Color3.fromRGB(49, 49, 49)
	Main.Position = UDim2.new(1.1, 0, 0.6, 0)
	Main.Size = UDim2.new(0.202970296, 0, 0.196539178, 0)
	Main.ZIndex = 2147483646

	Head.Name = "Head"
	Head.Parent = Main
	Head.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Head.BackgroundTransparency = 1.000
	Head.Size = UDim2.new(1, 0, 0.18341051, 0)
	Head.Font = Enum.Font.SourceSansBold
	Head.Text = title
	Head.TextColor3 = Color3.fromRGB(255, 255, 255)
	Head.TextScaled = true
	Head.TextSize = 14.000
	Head.TextWrapped = true
	Head.ZIndex = 2147483647

	Body.Name = "Body"
	Body.Parent = Main
	Body.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Body.BackgroundTransparency = 1.000
	Body.Position = UDim2.new(0, 0, 0.176088959, 0)
	Body.Size = UDim2.new(1, 0, 0.544856012, 0)
	Body.Font = Enum.Font.SourceSansBold
	Body.Text = body
	Body.TextColor3 = Color3.fromRGB(255, 255, 255)
	Body.TextScaled = true
	Body.TextSize = 14.000
	Body.TextWrapped = true
	Body.ZIndex = 2147483647

	Buttons1.Name = "Buttons1"
	Buttons1.Parent = Main
	Buttons1.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Buttons1.BackgroundTransparency = 1.000
	Buttons1.Position = UDim2.new(0, 0, 0.720944762, 0)
	Buttons1.Size = UDim2.new(1, 0, 0.278036356, 0)
	Buttons1.Visible = false
	Buttons1.ZIndex = 2147483647

	Button.Name = "Button"
	Button.Parent = Buttons1
	Button.BackgroundColor3 = Color3.fromRGB(60, 60, 60)
	Button.Position = UDim2.new(0.0146341445, 0, 0, 0)
	Button.Size = UDim2.new(0.970000029, 0, 0.899999976, 0)
	Button.Font = Enum.Font.SourceSansBold
	Button.TextColor3 = Color3.fromRGB(255, 255, 255)
	Button.TextScaled = true
	Button.TextSize = 14.000
	Button.TextWrapped = true
	Button.ZIndex = 2147483647
	Button.Modal = isFPS

	Buttons2.Name = "Buttons2"
	Buttons2.Parent = Main
	Buttons2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Buttons2.BackgroundTransparency = 1.000
	Buttons2.Position = UDim2.new(0, 0, 0.720944762, 0)
	Buttons2.Size = UDim2.new(1, 0, 0.278036356, 0)
	Buttons2.Visible = false
	Buttons2.ZIndex = 2147483647

	Button_2.Name = "Button"
	Button_2.Parent = Buttons2
	Button_2.BackgroundColor3 = Color3.fromRGB(60, 60, 60)
	Button_2.Position = UDim2.new(0.0146341445, 0, 0, 0)
	Button_2.Size = UDim2.new(0.469999999, 0, 0.899999976, 0)
	Button_2.Font = Enum.Font.SourceSansBold
	Button_2.TextColor3 = Color3.fromRGB(255, 255, 255)
	Button_2.TextScaled = true
	Button_2.TextSize = 14.000
	Button_2.TextWrapped = true
	Button_2.ZIndex = 2147483647
	Button_2.Modal = isFPS

	Button2.Name = "Button2"
	Button2.Parent = Buttons2
	Button2.BackgroundColor3 = Color3.fromRGB(60, 60, 60)
	Button2.Position = UDim2.new(0.545000017, 0, 0, 0)
	Button2.Size = UDim2.new(0.440731704, 0, 0.899999976, 0)
	Button2.Font = Enum.Font.SourceSansBold
	Button2.Text = "Button2"
	Button2.TextColor3 = Color3.fromRGB(255, 255, 255)
	Button2.TextScaled = true
	Button2.TextSize = 14.000
	Button2.TextWrapped = true
	Button2.ZIndex = 2147483647
	Button2.Modal = isFPS

	Main:TweenPosition(UDim2.new(0.791, 0, 0.6, 0), Enum.EasingDirection.InOut, Enum.EasingStyle.Sine, .5, true)
	
	--Notification comes out the bottom right side of the screen

	local function Close()
		Closed = true
		Main:TweenPosition(UDim2.new(1.1, 0, 0.6, 0), Enum.EasingDirection.InOut, Enum.EasingStyle.Sine, .5, true)
		wait(.6)
		Notification:Destroy()
	end --Guess what this does...

	if buttons and type(buttons) == "table" then
		pcall(function() --Use a protected call just incase Text or func in one of the tables is nil or wrong type
			if #buttons == 1 then
				Button.Text = buttons[1].Text --Button text
				Button.MouseButton1Click:Connect(function()
					if buttons[1]["func"] then if type(buttons[1]["func"]) == "function" then buttons[1]["func"]() end end
					Close()
				end) --Calling the function of the button if there is one, then close the notif
				Buttons1.Visible = true
			elseif #buttons == 2 then
				Button_2.Text = buttons[1].Text
				Button_2.MouseButton1Click:Connect(function()
					if buttons[1]["func"] then if type(buttons[1]["func"]) == "function" then buttons[1]["func"]() end end
					Close()
				end)
				Button2.Text = buttons[2].Text
				Button2.MouseButton1Click:Connect(function()
					if buttons[2]["func"] then if type(buttons[2]["func"]) == "function" then buttons[2]["func"]() end end
					Close()
				end)
				Buttons2.Visible = true
			end
		end)
	end
	
	spawn(function()
		wait(10)
		if not Closed then Close() end
	end)
end

return Lib
