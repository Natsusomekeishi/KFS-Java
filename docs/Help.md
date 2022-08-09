# <div align="center"><font color=#FD366D>插件教学</font></div>

[[toc]]

## 领地系统

>领地系统可以保护你所圈的土地，免受他人破坏！

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

![res8.png](https://a.ideaopen.cn/Keishi/iZU79gG4.png)

### 付费业务：领地系统

每个玩家最多免费建立10个领地，如果想要建更多领地，可以找群主购买，目前定价150点券增加一个领地。

## 粘液科技

>懒得写教学，自己去B站搜~

## 商店系统

>商店系统可以帮助你收购/出售物资，换取金币/点券/以物易物。

### 快速入门：如何购物

打开菜单/kfs，点击钻石进入商店，选择商店购物即可。

支付点券和金币请仔细看数额哦，如果买错了在群里面找卖家吧。

如果是以物易物，需要提前去主城，打开管理库存。点击创建一个物品的库存，手持该物品输入数值即可，这样才能去以物易物。

![egs10.jpg](https://a.ideaopen.cn/Keishi/UIYCvYOy.jpg)

### 快速入门：如何创建商店

>每个人只能创建一个商店，且商店命名在6字符及以内。

第一步：打开云星岛菜单，点击上方“钻石”。

![egs1.jpg](https://a.ideaopen.cn/Keishi/Y06Qc3Cp.jpg)

第二步：点击下方“钻石镐”，管理商店。

![egs2.jpg](https://a.ideaopen.cn/Keishi/Ex8TqUmq.jpg)

第三步：点击下方“末影箱”，创建商店。

![egs3.jpg](https://a.ideaopen.cn/Keishi/6ylEhPFv.jpg)

第四步：跟随提示，在输入框中输入店铺名称并发送。

第五步：点击自己创建好的店铺，进入管理界面。

![egs4.jpg](https://a.ideaopen.cn/Keishi/yxDCvt03.jpg)

第六步：点击一个店铺的实体坐标。

>在实体坐标附近32格内，卖家可以存商品。

![egs5.jpg](https://a.ideaopen.cn/Keishi/BPUJIj8R.jpg)

第七步：点击“箱子”进入店铺。

![egs6.jpg](https://a.ideaopen.cn/Keishi/i2yL9CzF.jpg)

第八步：点击下方“钻石”创建商品。

![egs7.jpg](https://a.ideaopen.cn/Keishi/GRhqYXTT.jpg)

第九步：手持想要添加的商品，依次发送“商品名称”、“出售或者收购”。

>商品名称即展示在页面上的物品名称，出售和收购为交易类型。

![egs8.jpg](https://a.ideaopen.cn/Keishi/kalPTOj4.jpg)

第十步：点击商品进行管理。

第二行选择支付类型：分别为“金币”、“点券”、“以物易物”。

“金币”和“点券”直接输入价格就行，“以物易物”需要手持需要易物的物品，再输入价格。

如何交易类型为出售，则需要买家支付给卖家，如果是收购，商品为“面包”，价格为金币10，则玩家会支付背包里的面包给商店主，商店主需支付金币给该玩家。

>买家“以物易物”时，需要将物品提前存入银行才行，否则无法交易，具体教学看如何购物。

第三行是存入和取出商品，如果你交易类型为收购，玩家支付的物品将可以从这里取出。

![egs9.jpg](https://a.ideaopen.cn/Keishi/SIyVnRPs.jpg)

其他功能自己去研究吧，比如设置限购时间、设置商店图标、提高商店热力值等等。

注意，商店支付“金币”和“点券”会收取一点税，金币是0.05，点券是0.1，自己算吧。

### 付费业务：商店系统

每个玩家最多免费建立1个商店，如果想要建更多商店，可以找群主购买，目前定价100点券增加一个商店。

商店图标可以设置成其他样式，想要设置其他样式可以找群主购买，目前定价为200点券添加一次。

## 自定义图片

服务器支持将自己喜欢的图片添加到游戏中，但因为需要手动操作且占用服务器运行，故收费使用，目前定价为20点券/方块。

你可以选择自己喜欢的图片，告诉群主想要放置的位置及方块区域大小，群主将给你放置在该位置。

图片可以任意缩放，一个方块可以放置128×128的像素面积。

![img1.jpg](https://a.ideaopen.cn/Keishi/GBOVYbN6.jpg)

譬如以下图片为宽2高3，占6个方块。

![img2.jpg](https://a.ideaopen.cn/Keishi/7ysYcM4l.jpg)

放置效果如下。

![img3.jpg](https://a.ideaopen.cn/Keishi/LgRlis1e.jpg)

以下图片为宽1高1，占据一个方块。

![img4.png](https://a.ideaopen.cn/Keishi/vNQkFvDw.png)

放置效果如下。

![img5.jpg](https://a.ideaopen.cn/Keishi/bAxTlfl7.jpg)

以下图片为宽5高7，占据35个方块。

![img6.png](https://a.ideaopen.cn/Keishi/Qbp7Sm7Y.png)

放置效果如下。

![img7.jpg](https://a.ideaopen.cn/Keishi/ZXk8Y85L.jpg)

注意：图片一经放置则不得修改，删除免费，但重新放置需另付费。