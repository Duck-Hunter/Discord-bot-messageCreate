      local content = message.content
        local attachment = message.attachments or nil
        local ch = message.channel.id
        local name = message.author.username
        local userid = message.author.id
        local xd = message.channel
        local emoji = message.react
        local tag = message.author.tag
----------------------------------------------------------------------------------------------------
local discordia = require('discordia')

local client = discordia.Client()

local prefix = "!" ----- คำนำหน้า

client:on('messageCreate', function(message)

    local userid = message.author.id
    
    if message.content == prefix.. "Cool" then
    
        message.channel:send ("<@" .. userid .. ">, done")
        
        message.member:send("test")
        
    end
    
end)

client:run("Bot ใส่ token ตงนี้ ลบตั่งเเต่ ใส่ออกเเล้วใส่ token เเถน")
