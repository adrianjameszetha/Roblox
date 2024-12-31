-- Unlimited Jumps script (for educational purposes)

local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")

-- Allow unlimited jumps by disabling jump cooldown
local function enableUnlimitedJumps()
    humanoid.JumpHeight = 50 -- Set jump height
    humanoid.PlatformStand = true -- Disable platform standing
end

-- Event for when the player jumps
humanoid.Jumping:Connect(function()
    -- Re-enable jump whenever the player jumps
    humanoid:ChangeState(Enum.HumanoidStateType.Physics)
    enableUnlimitedJumps()
end)

-- Initial setup
enableUnlimitedJumps()
