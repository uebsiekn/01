function Notify(Title1, Text1, Icon1, Time1)
  game:GetService("StarterGui"):SetCore("SendNotification", {
    Title = Title1,
    Text = Text1,
    Icon = Icon1,
    Duration = Time1,
  })
end
Notify("派脚本中心", "作者七赢", "rbxassetid://17360377302", 3)
Notify("永久免费", "祝你玩的开心","rbxassetid://17360377302",3)
Notify(""本脚本由凡尘指导,"rbxassetid://17360377302",3)
Notify("派脚本中心", "永久免费","rbxassetid://17360377302",3)
Notify("拒绝跑路", "拒绝倒卖","rbxassetid://17360377302",3)
Notify("启动完成", "祝你玩的开心","rbxassetid://17360377302",5)

local Library = loadstring(game:HttpGet('https://raw.githubusercontent.com/XiaoYunCN/UWU/main/Library%2FSilent%20ui'))()
local Window = Library:new("派脚本中心 X");

local creds = Window:Tab("公告",'16060333448')
local bin = creds:section("信息",true)
local about = creds:section("作者",true)

local Main = Window:Tab("主要",'16060333448')
local General = Main:section("玩家",true)
local GX = Main:section("通用",true)
local QU = Main:section("ESP",true)
local QW = Main:section("其他",true)

local JSDGt = Window:Tab("驾驶帝国",'16060333448')
local JSDG = JSDGt:section("自动&刷钱",true)

local FMDHt = Window:Tab("伐木大亨2",'16060333448')
local FMDH = FMDHt:section("伐木大亨2",true)

local SKQSt = Window:Tab("鲨口求生2",'16060333448')
local SKQS = SKQSt:section("鲨口&求生",true)

local DoorsT = Window:Tab("doors",'16060333448')
local Doors = DoorsT:section("通用&功能",true)
local DOORSR = DoorsT:section("透视",true)
local BP = DoorsT:section("其他",true)

local LLCQt = Window:Tab("力量传奇",'16060333448')
local LLCQ = LLCQt:section("主要&功能",true)
local LLQR = LLCQt:section("自动收集",true)
local LLRQ = LLCQt:section("跑步机",true)
local LLRE = LLCQt:section("岩石",true)
local LLQQ = LLCQt:section("传送位置",true)

local JSCQt = Window:Tab("极速传奇",'16060333448')
local JSCQ = JSCQt:section("自动&玩家",true)
local JSQC = JSCQt:section("传送位置",true)

local RZCQt = Window:Tab("忍者传奇",'16060333448')
local RZCQ = RZCQt:section("自动&模式",true)
local RZQC = RZCQt:section("传送位置",true)

local JYRSt = Window:Tab("监狱人生",'16060333448')
local TLT = JYRSt:section("整合",true)
local JYRS = JYRSt:section("监狱&主要",true)
local DL = JYRSt:section("身份",true)
local DP = JYRSt:section("其他",true)
local DX = JYRSt:section("传送地点",true)

local ZDYSt = Window:Tab("战斗勇士",'16060333448')
local ZDYS = ZDYSt:section("主要",true)

local HBTXt = Window:Tab("河北唐县",'16060333448')
local HBTX = HBTXt:section("主的",true)
local HBXT = HBTXt:section("传送位置",true)

local ZRZHt = Window:Tab("自然灾害",'16060333448')
local ZRZH = ZRZHt:section("自然&灾害",true)
local RHE = ZRZHt:section("玩家",true)

local EVt = Window:Tab("Evade",'16060333448')
local EV = EVt:section("Evade",true)

local XGt = Window:Tab("新更",'16060333448')
local XG = XGt:section("新更",true)
local GN = XGt:section("实用工具",true)

local OSCt = Window:Tab("其他脚本",'16060333448')
local OSC = OSCt:section("通用脚本",true)

local SIJt = Window:Tab("视觉",'16060333448')
local SIJ = SIJt:section("视觉",true)
local GIY = SIJt:section("光影",true)

local QH = Window:Tab("俄亥俄州",'16060333448')
local QB = QH:section("自动模式",true)

local EF = Window:Tab("FE",'16060333448')
local FE = EF:section("FE",true)

local EN = Window:Tab("作者通告",'16060333448')
local NE = EN:section("玩家公告!",true)

local VT = Window:Tab("其他注入器",'16060333448')
local YV = VT:section("输入器整合",true)

local OH = Window:Tab("火箭发射模拟",'16060333448')
local HO = OH:section("主要",true)
local HQ = OH:section("传送位置",true)

local UR = Window:Tab("超级大力士",'16060333448')
local RU = UR:section("主要的",true)
local OR = UR:section("其他",true)
local QS = UR:section("位置传送",true)

local OSQ = Window:Tab("战争大亨",'16060333448')
local QOS = OSQ:section("主要",true)
local SQO = OSQ:section("其他",true)
local Tab2 = OSQ:section("传送位置",true)

bin:Label("你的用户名:"..game.Players.LocalPlayer.Name)
bin:Label("你的注入器:"..identifyexecutor())
bin:Label("服务器id:"..game.GameId)

about:Label("作者七赢")
about:Label("此脚本由凡尘指导制成")
about:Label("正在努力优化")
about:Label("请勿倒卖")
about:Button("复制作者QQ", function()
    setclipboard("")
end)
about:Button("复制QQ群", function()
    setclipboard("")
end)
about:Toggle("移除UI辉光", "DHG", false, function(DHG)
    if DHG then
        game:GetService("CoreGui")["frosty is cute"].Main.DropShadowHolder.Visible = false
    else
        game:GetService("CoreGui")["frosty is cute"].Main.DropShadowHolder.Visible = true
    end
end)
about:Toggle("彩虹UI", "RBUI", false, function(RBUI)
    if RBUI then
        game:GetService("CoreGui")["frosty is cute"].Main.Style = "DropShadow"
    else
        game:GetService("CoreGui")["frosty is cute"].Main.Style = "Custom"
    end
end)
about:Button("摧毁界面", function()
    game:GetService("CoreGui")["frosty is cute"]:Destroy()
end)

General:Slider("步行速度!", "WalkSpeed", game.Players.LocalPlayer.Character.Humanoid.WalkSpeed, 16, 400, false, function(Speed)
  spawn(function() while task.wait() do game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Speed end end)
end)
General:Slider("跳跃高度!", "JumpPower", game.Players.LocalPlayer.Character.Humanoid.JumpPower, 50, 400, false, function(Jump)
  spawn(function() while task.wait() do game.Players.Lo
