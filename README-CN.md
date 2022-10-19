# 加勒比工业

加勒比海的工业是国营经济的典范，除了运输网络之外，你还拥有工业和生产链。经济是出口驱动的：除非你出口货物，否则你不会因为运输货物而获得报酬。

你们的岛屿有肥沃的土壤和丰富的石油和镍储量，但并没有加工工业来生产有价值的产品。

(跳转至 [设计理念(未翻译)](#design-philosophy))

## 工业产业链(暂未翻译)
![Cargo flowchart](docs/cargo_chart.png)

#### 进出口详情
* 出口 咖啡 -> 进口 食品
* 出口 糖 -> 进口 原油
* 出口 镍 -> 进口 肥料
* 出口 钴 -> 进口 PC塑料管
* 出口 雪茄 -> 进口 化学品
* 出口 旅客 -> 进口 机械装置

## 货物类型
与大多数OpenTTD经济体系不同，货物支付并不取决于运输距离。这为玩家提供了进出口的经济模型,而不仅仅是经营一家运输公司。(GRF参数设置中可以关闭,默认开启)

#### 出口货物
这些货物被出口到外贸进出口，在那里它们被交易为其他货物。这些都带来了可观的利润。

#### 进口货物
在外贸进出口通过出口货物换取的进口货物。它们需要你花钱运输，所以不要进口你不需要的东西！

#### 国产货物
本土可以生产的都是其他货物，包括在不同行业之间运输的工人和中间货物。他们损失不大。唯一的例外是邮件，它可以正常盈利。

## 工厂行为
所有工厂都要求工人生产货物。行业不会关闭或改变生产。

#### 初级产业
* 咖啡种植园
* 甘蔗种植园
* 烟叶种植园
* 油井
* 镍矿场

这些产业是自动创建的，有时与村庄要求的海拔或距离有关。他们本身无法生产任何东西，除非你交付工人和任何其他所需的基本货物（如油井管道）。此外，运送大量货物将使产量翻一番。在每次生产周期（每月8-9次）期间，都会储存和消耗大量货物，以确定生产了多少货物。

#### 加工产业
* 炼油厂 (Oil Refinery 译者存疑?)
* 锯木厂 (Sawmill 译者存疑?)
* 家具厂 (Furniture Factory 译者存疑?)
* 造纸厂 (Paper Mill 译者存疑?)
* 盒子工厂 (Box Factory 译者存疑?)
* 面包房 (Bakery 译者存疑?)

译者注:翻译时没有看到对应的加工工厂 应当是如下
* 炼油厂
* 烟草公司
* 朗姆酒厂
* 镍矿加工厂
* 制糖厂

这些行业由玩家设立(建设产业工厂)。每单位的货物需要一名工人。若觉得需要的工人很多,没错!每个工人是主要的生产瓶颈，你需要将许多城镇与各个行业连接起来，并运送必要的货物来发展这些城镇。

此外，其中一些行业还有额外的货物，如镍矿加工厂，这些都是必需的输入货物。行业窗口列出了每单位输出货物所需的输入货物比率。

## 入门

最初，唯一可以直接获利的货物是咖啡，出口前不需要加工。

从出口尽可能多的咖啡开始，直到你买得起第一个加工行业：制糖厂。之后，根据货物流程图和进出口贸易协议，通过建造适当的行业来解锁新的货物链。

不过，要小心，在获得所需货物之前，不要扩展新的货物链，例如，镍相关需要化学品，这些化学品是通过出口雪茄获得的。

请记住，进口货物的运输费用花费是你大量的钱，如果不清楚，请查看货物支付费率图。

#### 建议的游戏设置

* 新闻/顾问：如果车辆收入为负，则发出警告：关闭
* 新闻/顾问：车辆丢失时发出警告：关闭
* 环境>行业>公司站点可以为连接中性站的行业提供服务：关闭
* 环境>货物配送：手动

#### 建议的全局设置

* 气候：亚热带(其实只能是这个图,不然无法正常加载)
* 海平面：中等(如果是非常平整,那么很多产业园将无法刷新,部分产业是有海拔需求的)
* 城镇数量：高
* 行业数量：低
* 沙漠覆盖率：0%(咖啡种植园, 甘蔗种植园, 烟叶种植园 是不能建设在沙漠中的)

#### 所需要的GRFs

* ~~Improved Town Layouts 1.4.0 or later~~
  * ~~(These houses don’t accept Workers or Food, keeping those cargos going only to your industries.)~~

* 以上原文保留(原因是所需的mod前置已经更名)
* 包含 ILT House 2.1 (Improved Town Layouts 已更名为 ILT House) 或更高
* 
#### (可选) GRFs
作者使用的GRFs,如果不需要可以不添加(译者注:其实可以忽略.能玩这个mod的常用的都已经添加过了,有些还奇奇怪怪的 例如有了2cc 完全没必要用Iron Horse2)
* Iron Horse 2
* Termite (tracks)
* SHARK (ships)
* Mop Expanded Road Vehicles
* Unspooled (roads)
* Av9.8 Aircraft Set
* OpenGFX+ Airports
* Industrial Stations Renewal
* ISR-style Dock
* ISR/DWE-style Objects
* US Stations set
* Total Bridge Renewal Set
* Rainforest Ruins

## 版权声明 (译者注:这个没必要翻译了)
* Beach sprites: [Beach Objects](https://www.tt-forums.net/viewtopic.php?f=26&t=62258) by Quast65, GPL v3 license

## 翻译语言
* 英语
* 法语 (arikover)

欢迎通过PR添加你使用的语言(译者注:这个实在懒得翻译,我都搞完了..)

## 设计理念 (译者注:机翻,实在懒了,原文在文末)
加勒比海工业是一个实验性的工业/经济模式，旨在通过打破常见的设计模式，回收“无用”功能，增加有趣的游戏体验，从根本上重新思考OpenTTD经济。

在讨论我所做的改变之前，让我们简要回顾一下普通和大多数新GRF经济体的结构：

* 金钱是游戏初期的限制因素，但到了游戏中期，你的公司挣钱的速度比你花得快。然后，约束成为车站、交叉口和主线吞吐量的平铺空间。没有钱，OpenTTD仍然很有趣。

* 无论是通过电站评级推动的产量增长（香草型），还是通过提振货物（FIRS），行业都增长到了巨大的产量。这种高产量通常需要双轨基础设施，甚至不要梦想使用公路车辆运输货物。

* 大多数生产链都会将城镇货物运送到“黑洞”行业，如货物、酒精或车辆。这些都是非常有利可图的，但当你完成生产链到这个程度时，金钱通常不是一个激励因素。

与我交谈的那些严肃的OpenTTD玩家往往分为两类游戏：
1.玩家使用CargoDist构建乘客网络，自动为乘客提供路线，并为游戏趣味创造网络设计和容量挑战。
2.使用FIRS Steeltown或XIS等复杂行业模型构建货运网络的玩家。
我玩过两种风格的游戏，对每种游戏中缺少有趣的游戏玩法的功能感到失望和好奇：
* 道路车辆的容量太小，无法在利基角色之外发挥作用，如促进货物配送、支线或非常短的距离路线。
* 如果没有像JGRPP这样的日间补丁，大多数铁路线都需要双轨。除了繁重的干线外，还有一些低交通量的支线也不错。
* 船只速度如此之慢，除非你绝对需要它们才能到达石油钻塔（香草）或渔场（FIRS），否则用它们代替火车常常会让人觉得很傻。
* 客运只给你钱（“糟糕的特性”，记得吗？）它唯一的游戏兴趣来自与CargoDist和城镇发展保持同步的战斗……这常常是令人沮丧而非乐趣。
* Endgame镇的货物没有运送的动机，将它们全部倾倒在一个地方而不是在地图上分发，同样有利可图。
* 货物老化和每件货物的不同价值只在早期游戏中起作用。
* 如果你不是在玩弄乘客或邮件，那么城镇对你来说毫无用处，只会成为你的拦路虎。

那么，~~我们能做些什么~~奇怪的、不明智的~~有趣的事情来改变这种情况呢？
* 初级工业的固定产量远低于FIRS，以鼓励公路车辆和单轨铁路线进入工业，同时仍能为繁忙的干线保持足够的产量。
* 只有初级产业会在地图生成时产生，而所有次级产业都由玩家资助——稍后将详细介绍。行业从未改变生产或关闭，只有酒店在游戏期间产生。
* 所有行业都需要工人（乘客）进行生产。
* 初级工业需要来自最近城镇的少量但稳定的工人流动，创造一个令人满意的地方道路和公交线路网络，并使城镇具有相关性。
* 第二产业需要大量工人：每单位货物需要一名工人。资助他们需要你考虑劳动力供应，一旦建成，你就需要发展城市，从附近的城镇运营通勤列车。
## 设计理念原文
Industries of the Caribbean is an experimental industry/economy mod which aims to radically rethink the OpenTTD economy by breaking common design patterns and reclaiming “useless” features to add interesting gameplay.

Before we get into what I’ve changed, let’s briefly recap how vanilla and most NewGRF economies are structured:

* Money is an early-game constraint, but by mid-game your company earns money faster than you can spend it. The constraint then becomes tile space for stations, junctions, and mainline throughput. OpenTTD would still be fun without money.
* Industries grow to immense production either through station rating-fueled production increases (vanilla), or boost cargos (FIRS). This high production usually requires double-track infrastructure, and don’t even dream of using road vehicles for cargo.
* Most production chains lead to town cargos which are delivered to “black hole” industries, such as Goods, Alcohol, or Vehicles. These are highly profitable, but by the time you complete the production chain to this extent, money is generally not a motivating factor.

The serious OpenTTD players I talk to tend to fall into two gameplay categories:

1. Players who build passenger networks using CargoDist to route passengers automatically and create network design and capacity challenges for gameplay interest.
2. Players who build cargo networks using a complex industry mod like FIRS Steeltown or XIS.

I have played both styles of game and have been frustrated and intrigued by features in each which fall short of interesting gameplay:

* Road vehicles are too low capacity to be useful outside niche roles like boost cargo distribution, feeder lines, or very short distance routes.
* Without daylength patches such as in JGRPP, most rail lines require double track. It would be nice to have some low-traffic branch lines in addition to the heavy trunk lines.
* Ships are so slow that unless you absolutely need them to reach Oil Rigs (vanilla) or Fishing Grounds (FIRS), using them instead of trains often feels silly.
* Passenger transportation gives you nothing but money (a “bad feature,” remember?) and its only gameplay interest comes from fighting to keep up with CargoDist and town growth...which is often more frustrating than fun.
* Endgame town cargos have no incentive to deliver them, and it’s just as profitable to dump them all in one place rather than distributing them across the map.
* Cargo aging and different values per cargo only matter in the early game.
* If you’re not playing with passengers or mail, towns are useless to you and just get in the way.

So, what ~~weird and ill-advised~~ interesting things can we do to change this?

* Primary industries have a fixed production much lower than FIRS, to encourage road vehicles and single-track rail lines to industries while still keeping enough production for busy trunk lines.
* Only primary industries spawn on map generation, and all secondary industries are funded by the player — more on this later. Industries never change production or close, and only Hotels spawn during the game.
* All industries require Workers (Passengers) for production. 
    * Primary industries need a small but steady flow of workers from the nearest town, creating a pleasing network of local roads and bus routes and making towns relevant.
    * Secondary industries need an immense supply of Workers: one per unit of cargo converted. Funding them requires you to think about worker supply and once built, you’ll need to grow cities and run commuter trains from nearby towns and cities.
