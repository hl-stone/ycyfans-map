# ycyfans-map
## 项目目的
分析杨超越粉丝的数据样本，构建大屏可视化。
## 基本构想
主要就是先用Python爬虫扒取超越妹妹的微博粉丝数量，然后对大量数据进行分析。主要分析啥呢？分析粉丝都大概在哪个年龄段，性别，名族，所在地，开始关注时间，已经关注时间及尽可能多的信息，更深层次地可以分析粉丝之间的关系（朋友，同事）建立关系图谱。然后还可以再深度挖掘分析大家转发超越妹妹表情包到底是为了考试还是升职加薪去水逆。到最后当然是地理可视化展示啦~，看粉丝大在全国的分布情况，男女占比，年龄段分布情况以及转发超越妹妹关键热词云图可视化。
## 总体设计
* 页面模块
   * 打算采用左中右布局，左右两侧为菜单模块，中间部分为地图可视化，整体格调为蓝黑色调的科技感
* 菜单模块
   * 性别占比分析（百分比扇形图）
   * 名族分布（百分比扇形图）
   * 粉丝区域排行榜（竖排的柱状图，打算做滚动条）
   * 粉丝关注时长对比（百分比扇形图）
   * 某时间段内涨粉关注情况（折线统计趋势）
   * 粉丝职业分析（横排的柱状图）
   * 粉丝关联度（是否同事朋友，需要深度挖掘，做成关系图谱）
   * 热词云图展示
   * 粉丝活跃度分析
   * 粉丝线下活动分享墙
   * 粉丝心愿墙
   * ...包括但不仅限于
* 地图模块
   * 粉丝区域分布渲染（根据每个省份不同粉丝数量，渲染色块[参考1](https://gallery.echartsjs.com/editor.html?c=xa5_zRRpes)）
   * 粉丝热力图（根据每个省份不同粉丝数量，键入插值）
   * 粉丝应援流向图（比方说，鸟巢举办超越妹妹的活动，各地粉丝从各自所在地向北京迁徙轨迹动画[轨迹流向1](https://gallery.echartsjs.com/editor.html?c=xHyiG_MDEz)[轨迹流向2，流向要改成向中间流](https://gallery.echartsjs.com/editor.html?c=xN7FI60doi)）
   * ...包括但不仅限于