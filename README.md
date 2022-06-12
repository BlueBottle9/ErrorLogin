# bukkit-ErrorLogin
A smiple bukkit login plugin (with many bugs) 一个简单的bukkit插件(许多bug)

Because I am a noob,so this plugin may be unstable. 因为本人是个菜鸡，所以这个插件可能很不(稳定)

To use this(使用方法):

Warning(警告): This plugin maybe not work well on craft-bukkit or spigot server,because it used paper-api... 

这个插件可能不会很好地在非Paper服务器上运行,(因为开发时用的Paper的API))

  1.Download the release jar and put it into plugins floder. 下载jar文件并放置在插件文件夹下
  
  2.Restart or reload your server to load this. 重启或重载你的服务器
  
  Configurations:
  
config.yml:

```allow-insecure-password: false #Allow insecure passwords 允许不安全的密码 

login-point: #Login point,to teleport players to target location when they join 登录点，当玩家进入时将他们传送到指定位置
  
  enable: false #Enale login point 是否启用
  
  point:
    
    world: 'world' #Login world 登录点的维度
    
    X: 0
    
    Y: 100
    
    Z: 0
  
  tp-back: true #Teleport player back to thier original locations. 将玩家传回原位置
  

skip-genuine-player: false #Skip online players(Warning: Is not tested) 跳过正版玩家(未经测试！！！(好吧，其实就是我没正版))

auto-login:#自动登录
  
  enable: true #启用
  
  allow-time(min): 120 #When the time to last login less than this vaule,the player will login automatically(Sorry for my English).
                       #当玩家距上次登录的时间小于该值时，将自动登录
  
  
  do-not-tp-to-loginpoint: true #Whether teleport the player that logined automatically to login point or not. 
                                #是否不将自动登录的玩家传到登录点
  

allow-reset-password: false #Allow players reset thier password. 是否允许玩家重设他们的密码


prompts: #提示
  
  title: true #Enable send title to players. 是否给玩家发送标题(让他登录)
  
  message:#How to send messages to players.配置如何给玩家发送提示信息
    
    timer-delay(tick): 40 #Delay bettween messages.消息间隔
    

tone: true #Enable tone. 是否启用音效

player-kicks: #When should kick players.何时该提出玩家
  
  
  wrongpassword: false #When a player enters a wrong password. 当一个玩家输错密码时
  
  
  server-reload: true #When server reloads.Do not recommand to disable it,because that may cause some problem.当服务器重载时(不建议关闭，可能会导致部分问题)



default-language: 'zh_cn' #Default language. 默认语言



date-format: 'yyyy-MM-dd hh:mm:ss' #Data format template. 日期格式化模板







You can modify plugins/ErrorLogin/lang/language-files to custom message or create more files to support more language!


你可以修改plugins/ErrorLogin/lang/ 下的语言文件来自定义消息，也可以创建更多语言文件来支持更多的语言
