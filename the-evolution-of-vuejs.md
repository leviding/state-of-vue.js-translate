## Vue.js的演变

你知道Vue第一次发布是在什么时候吗? 最初它甚至并不叫"Vue". 作者的首次提交是在2013年06月27日, 那时项目叫"Seed", 转瞬间, Vue.js已经四岁了. "Seed"这个名字用了六个月, 在 2013年12月初, 作者把它正式更名为"Vue". 但是, Vue的第一个对外的版本(0.8.0)在2014年2月才发布, 在那时候, Vue.js还只关注MVC架构中视图(View)部分.

Vue拥有的一些特性, 让开发很容易接受它. Vue的模板语法很像AngularJS的风格, 也有被React引入的基于组件的架构. 这样, 开发者可以从二者平滑地过渡到Vue. 我会把Vue想象为一个继承了父母(AngularJS, React)优秀基因的孩子, 他自己也不断地提升开发者的使用体验.

一年之后, JS社区才对Vue产生兴趣. 当时, Laravel(一款流行的PHP框架)社区首先开始使用Vue(TODO). 几个月之后, 期盼已久的1.0版本终于发布了, 对于Vue来说, 这是具有里程碑意义的一次版本发布.

与此同时, vue-router(2015-08-18)、vuex(2015-11-28)、vue-cli(2015-12-27)相继发布. 这意味着Vue.js从一个视图层库发展为我们现在所说的渐进式框架

去年, 备受期待的2.0-alpha版本发布, 它被彻底重写了, 同时引入了一些新的概念, 比如: Virtual DOM 和 服务端渲染. 但是, API基本没有变化, 因此从1.0 到 2.0 版本可以平滑迁移. 使用官方出品的[迁移工具](https://github.com/vuejs/vue-migration-helper)会帮助你完成迁移过程.

### 社区

在接近一年的时间里, 至今依然活跃的社区促使Vue.js成为了JavaScript三大顶级框架之一, 而且看起来并不会止步不前.

人们非常喜爱Vue. 嘴上说没用`这句话是意译的`, 数字是真实的: 在GitHub上, Vue是2016年star数最多的框架.(TODO)

社区的兴趣是非常浓厚的`TODO: 这句话有点硬翻的感觉`, 当我们启动[Vue Newsletter](http://vue-newsletter.com/)项目时, 在几分钟内, 便有数百人订阅了. 一直没间断的邮件通知, 让我们感觉自己就像Instagram的明星一样(备受关注). 每一期(TODO)都是很难准备的, 因为每周都产生很多和Vue相关的内容(TODO). 每天都有高质量的教程、见解深刻的文章以及我能想到的库翻陈出新. 有点疯狂(TODO, 这边的insane不知道该如何翻译好点, 个人理解, 作者的意思应该是每周都有很多和Vue相关的内容出现, 而他也要出每一期的订阅, 要从这么多的新内容里面做挑选,  有点哭笑不得感觉). 这不是全部, Vue社区有`(TODO is bolstered with, 这个翻译也不太确定)`一个`活跃(TODO)`的论坛[thriving forum](https://forum.vuejs.org/)和一个`聊天频道(TODO)`[channel](https://chat.vuejs.org/), 每天都有成百上千的开发者活跃在上面.

此外, 我们可以发现, 随着开发者对Vue的兴趣逐渐浓厚, 全球很多公司开始关注`这里翻译成关注待定, TODO`Vue. 点击这里[vuejobs.com](http://vuejobs.com/), 看看他们发布的的职位吧.

### 生态

值得一提的是, 除了社区项目之外, Vue核心开发团队也维护了一些官方库, 比如vue-router、vue-loader、vuex(状态管理)、vue-rx 以及针对RxJS开发的vuex-observable. 还有一些工具库, 比如vue-cli、vue-server-renderer、vue-loader、vetur、vue-migration-helper. 它们为什么重要? 因为这样, 你就可以渐进式地使用其他核心库, 这些库可以完美配合, 使得Vue转变为一个像Angular、Ember一样`完善的 TODO`框架. 当然, 如果你的项目需要, 你可以随时将其中的一部分切换为其它非官方的解决方案. 官方库的另外一个好处是它们往往代表着高质量、长期支持以及与Vue良好的兼容性.

正如大家所料, 像Vue社区这种大型而且参与感高的社区(TODO, 这边也可以帮忙看下), 会出现大量社区项目. 不仅仅是小型项目、解决单一问题的库(TODO,  focused libraries 这里觉得需要再考虑), 我们现在来谈谈大型项目. 举个例子, [Nuxt.js](https://nuxtjs.org)是一个基于Vue(TODO, highly-opinionated这边不知道如何翻译?)的框架, 它采用了一些小工具库以及设计模式, 这使得开发需要服务端渲染的应用变得极其简单.

[Quasar 框架](http://quasar-framework.org)可以帮助开发复杂的移动和桌面应用. 还有其他流行的UI框架, 比如: [Element-UI](http://element.eleme.io/#/en-US) and [Vuetify](https://vuetifyjs.com/), 这些框架提供了几十个风格统一的UI组件来帮助你开发`bootstrap your application TODO`. Vue在移动端开发方面, 得到了[OnsenUI](https://onsen.io/vue/)(由Monaca开发) 和 [NativeScript](https://www.nativescript.org/blog/a-new-vue-for-nativescript)的大力支持.


从我作为一个Web开发者的角度来看, 我可以向你保证: Vue已经有你开发应用所需的一切了. 每周, 我都见证越来越多的库发布, 以至于没有办法追踪所有的库(TODO). 你可以在[awesome-vue](https://github.com/vuejs/这里)找到这些库. 此外, Vue核心开发团队在[curated.vuejs.org](http://curated.vuejs.org/)管理了一些推荐的库, 这些库主要用于像表单验证、国际化、AJAX等常见的任务, 避免开发者在选择合适的库出现选择恐惧症.

### 支持

许多人指出, 和Angular或React不同的是, Vue背后没有大公司的支持, 而且看起来这也不太乐观. 我绝不同意. Vue和jQuery、Babel、webpack以及JS世界中其它可被信赖的工具一样体现了真正的开源精神. 这样有一个明显的优势: 这些项目不用去满足这些公司的特定需求, 取而代之的是更专注社区的需求.

Vue实现了很多社区最需要的功能(TODO). 说起code spliting, webpack核心开发团队成员Sean Larkin, 这样评价Vue:

> 首个将开发者开发体验放在心上(TODO)的公司.

但在开发体验上已经远远超越webpack, 而且体验在各个方面: 易用性、无缝集成(TODO)、优秀的文档(TODO)、整体的可扩展性.

显而易见, Vue.js和很多其它开源项目一样, 刚开始是一个个人作品. 慢慢地(TODO), 它拥有了一个全职(TODO)核心团队, 专门负责维护它的各个方面和生态系统(TODO).

基金会呢? 近两年, 通过在Patreon 和 Open Collective上的成功运作, 全球的很多个人和公司决定每个月固定赞助尤雨溪(Vue作者)和核心团队超过$10. 这样, 尤雨溪就可以全职(TODO)从事Vue的开发了.

赞助者包括许多公司和几百位个人赞助者. 在[这里](https://vuejs.org/support-vuejs/)可以看到这些赞助者们.

### 成长

让我们通过一组数字来更直观地感受到Vue生态的快速成长.

以GitHub的star数为例, 尽管它不是衡量一个项目知名度的完美指标. 但令人振奋的是, Vue是[GitHub 2016年获得star数最多的项目](https://risingstars2016.js.org/#all). 不限于JavaScript 或者前端分类, 在2016年, 它是获得star数最多的项目. 过了一段时间, 到现在为止, 它已经是star数第二多的前端框架了, 仅次于React. 同时, 也是GitHub上star数第六多的项目. 已经超过了jQuery和Angular.

[2016年前端调查](https://stateofjs.com/2016/frontend/)这样的问卷调查显示:Vue是用户满意度最高的语言之一, 89%使用过Vue的开发者表示会再次使用Vue.

当然, 还有其他指标来衡量. 诸如npm上每个月的下载量(大约800k), 开发者工具每周活跃用户数达到270k. npm下载量和React的下载量比起来, 相差很小. 但值得一提的是: 在过去的十二月, Vue的下载量增长了5倍. 以Vue现在的增幅`TODO`, 我相信在未来几年, 这个数字将会以更快的速度增长.

事实上很大一部分的增长是因为越来越多的公司选择Vue作为主要的前端框架. 除此之外, 开发者们很欣赏Vue平滑的学习曲线，集成到他们现有的技术栈的易用性，以及顶尖的性能(TODO)。也许最重要的因素是提升开发效率和减少维护成本。换句话说, 选择Vue, 省钱.

但不要只信我的一家之言。为此, 我们对来自88个国家的1126位开发者做了调研, 并收集了一系列来自不同行业的采用Vue的案例.

以上.
