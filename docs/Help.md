# <div align="center"><font color=#FD366D>插件教学</font></div>

## 领地系统

>本服务器默认圈地工具：木棍

### 快速上手：如何圈地

第一步：使用“木棍”圈地

具体操作为，电脑版拿木棍左键点击方块选择第一个选取点，右键选择第二个。

手机版同样拿木棍点击，点击选择第一个选取点，短按一下选择第二个。

被选择对角线区域，即如下图所示长方体为选中的范围。

![res1.png](https://a.ideaopen.cn/Keishi/nEYO6L6G.png)

![res2.png](https://a.ideaopen.cn/Keishi/QnvQB7f4.png)

第二步：两个点选中之后，电脑版将会在正下方显示花费金额，手机版则会在左上方文字中显示，如果你有足量的金币支付，则可以建立领地。

若显示太快没有看清楚，可以输入这条指令再次查看所需金额 /res select cost

第三步：输入这条指令创建领地 /res create [领地名] ，需注意的是，领地名需要是英文字母。

![res3.png](https://a.ideaopen.cn/Keishi/PKxxXbRg.png)

![res4.png](https://a.ideaopen.cn/Keishi/lz3B3tIk.png)

说明：领地创建完，默认仅可创建者使用，其他玩家可参观但无法破坏/放置/操作领地内任何方块。若需要详细设置，可以处在想设置的领地内，输入 /kfs 打开云星岛服务器菜单，点击上面的时钟进行设置。

### 进阶操作：更改领地

① 如何退款，删除领地？

输入指令 /res remove [领地名] 即可，需要是自己已创建过的领地。

![res5.png](https://a.ideaopen.cn/Keishi/6x9HJENA.png)

![res6.png](https://a.ideaopen.cn/Keishi/DAZJ4oiX.png)

![res7.png](https://a.ideaopen.cn/Keishi/G7WmBAUm.png)

注意退款只能退一部分，并非原价退款！

② 如何选中该区域正上方所有方块/正下方所有方块/上下所有方块？

第一步选择完之后，输入下方任意一条指令即可。

/res select sky —— 选择区域扩展到天空

/res select bedrock —— 选择区域扩展到基岩

/res select vert —— 选择区域从天空到基岩

③ 如何给予其他玩家基本权限，使用自己的领地？

输入下方指令即可。

/res padd [领地名] [玩家名] 

删除其权限为：

/res pdel [领地名] [玩家名]

④ 如何打开可视化领地权限操作界面（GUI）？

/kfs 打开云星岛菜单，位于想要设置权限的领地中，点击时钟。

或 /res set 打开菜单。

⑤ 如何扩大已有领地大小？

/res expend [领地名] [扩展单位]

玩家面向哪里就往哪里扩展输入的扩展单位的大小。

### 常用指令：配置领地

/res tp [领地名] —— 传送到指定领地

/res tpset —— 设置领地中的传送位置（当玩家输入/res tp [领地名]时，将会传送至您在领地内设置的传送位置）

/res unstuck —— 将您移动到你所在的领地外

/res show [领地名] —— 显示领地的边界

/res message [领地名] enter [信息] —— 自定义玩家进入领地的消息

/res message [领地名] leave [信息] —— 自定义玩家离开领地的消息

/res rename [旧名称] [新名称] -重命名领地

### 其他指令：详细操作

#### 领地创建与删除：

/res create [领地名] —— 创建一个领地

/res remove <领地名> —— 删除一个领地

/res subzone [子领地名] —— 在所处的领地中创建一个子领地

/res auto [领地名] [范围] —— 自动在你站着的位置为中心，创建你能创建最大的领地

/res select [x] [y] [z] —— 选取以你为中心需要被保护的区域，（Z=高度，X/Y=横轴）

/res select size —— 显示所选区域大小

/res select cost —— 显示已选择区域价格

/res select auto [玩家]  —— 打开自动选择区域

/res select expand [数值] —— 选区向面对的方向选择扩展数值大小

/res contract <领地> [缩小单位] —— 从你面对的方向缩小领地

/res select shift [数值] —— 选区向面对的方向平移

/res select vert —— 高度从天空扩展到基岩

/res select sky —— 高度扩展到天框

/res select bedrock —— 高度扩展都基岩

/res select chunk —— 选择目前所在区块

/res select worldedit —— 使用Worldedit的选区作为领地选区

/res area add [领地] [区域ID] —— 为领地添加物理区域

/res area remove [领地] [区域ID] —— 移除领地的物理区域

/res area remove [领地] [区域ID] —— 替换领地的物理区域（可以与其他领地区域重叠）

/res setmain <领地> —— 设置主领地

/resadmin server [领地] —— 创建一个属于服务器所有的领地

#### 领地权限与名称：

/res padd <领地名> [玩家] —— 向玩家添加基本权限

/res pdel <领地名> [玩家] —— 删除玩家的基本权限

/res pset <领地名> [玩家] [权限] [true/false/remove] —— 给不同的玩家上设置权限

/res set <领地名> [权限] [true/false/remove] —— 在不同的领地内设置权限 (以上两指令，不输入标志及其后面的内容打开GUI面板）

/res pset <领地> [玩家] removeall —— 删除一个玩家所有权限

/res rename [旧名称] [新名称] -重命名领地。如果需要重命名子领地，必须使用全名称(主领地.子领地),而新名称不用全名称。

/res mirror [原领地名] [目标领地名] -从原领地复制权限到目标领地，但前提是你是两个领地的所有者。

/res gset <领地名> [组名] [标志] [true/false/remove]  —— 在不同的权限组里设置标志

/res reset <领地> —— 将领地的所有权限重置.

/res lset <领地> [blacklist/ignorelist] [材料] —— 将某物品加入黑名单以阻止这种物品被放置在领地中

/res lset <领地> Info —— 忽略名单选项

#### 领地信息：
/res message <领地名> [enter/leave] [信息] —— 自定义玩家进入或离开领地的消息。（enter=进入,leave=离开）（信息可以是彩色&的）

/res info —— 显示目前所处的领地信息，如果在领地外使用该指令，将会显示自己的领地信息

/res list [玩家] —— 列出玩家拥有的领地信息

/res listall <页码> —— 列出玩家所有领地

/res area list [领地] <页码> —— 列出领地的物理区域

/res area listall [领地] <页码> —— 列出所有区域的坐标和详细信息

/res lists —— 预定义的权限列表可以应用到领地上

/res lists add <列表名> —— 添加一个列表

/res lists remove <列表名> —— 删除一个列表

/res lists apply <列表名> <领地> —— 将列表应用于领地

/res lists set <列表名> <权限> <值> —— 设置列表全局权限

/res lists pset <列表名> <玩家> <权限> <值> —— 设置列表玩家权限

/res lists view <列表名> —— 设置列表组权限

/res lists view <列表名> —— 查看列表

/res listhidden <玩家> <页码> —— 列出指定玩家拥有的隐藏领地

#### 传送相关：

/res tp [领地名] —— 传送到指定领地

/res tpset —— 设置领地中的传送位置（当玩家输入/res tp [领地名]时，将会传送至您在领地内设置的传送位置）

/res unstuck —— 将您移动到你所在的领地外

#### 领地使用：

/res show <领地> —— 显示领地的边界

/res bank [deposit/withdraw] <领地> [数额] —— 管理领地银行（deposit=存款,withdraw=取款)

/res resbank [deposit/withdraw] [数量] —— 从领地银行借贷

/res give [领地名] [玩家] —— 将所选领地给予给另外一名玩家！(该玩家须在线，且你是领地所有者。)

/res compass <领地名字> —— 设置指南者指向领地

/res shop —— 管理领地商店

/res shop list —— 显示所有作为商店的领地

/res shop vote <领地> [分数] —— 为领地商店评分

/res shop like <领地> —— 为领地商店点赞

/res shop votes <领地> <页码> —— 显示当前或指定领地商店的评分列表

/res shop likes <领地> <页码> —— 显示当前或指定领地商店的赞列表

/res shop setdesc [描述文字] —— 设置领地商店描述, 支持颜色代码, 用 /n 表示换行

/res shop createboard [位置] —— 在选区位置建立商店宣传板. [位置] 表示宣传板的起始位置

/res shop deleteboard —— 右击宣传板的告示牌以删除宣传板

#### 领地聊天频道：

/res rc <领地> —— 加入当前领地或者指定领地的聊天频道

/res rc leave —— 如果你在一个领地频道内, 你将会离开此频道

/res rc setcolor [颜色代码] —— 设置领地频道文字颜色

/res rc setprefix [新前缀] —— 设置领地频道前缀

/res rc kick [玩家] —— 从频道中踢出玩家

## 粘液科技