![2017-11-20_182302](https://user-images.githubusercontent.com/26959437/33013724-005297ca-ce20-11e7-8682-97b56068e933.png)

# Vue 2017 报告

> * 译文出自：[掘金翻译计划](https://github.com/xitu/gold-miner)
> * Event Organizer：[leviding](https://github.com/leviding)
> * Translaters：[sasa-m](https://github.com/sasa-m)、[altairlu](https://github.com/altairlu)、[ParadeTo](https://github.com/ParadeTo)、[ly525](https://github.com/ly525)、[zwwill](https://github.com/zwwill)、[html5challenge](https://github.com/html5challenge)、[vxqqb](https://github.com/vxqqb)
> * Reviewers：[leviding](https://github.com/leviding)、[ParadeTo](https://github.com/ParadeTo)、[PCAaron](https://github.com/PCAaron)、[vxqqb](https://github.com/vxqqb)、[zwwill](https://github.com/zwwill)、[caoyi0905](https://github.com/caoyi0905)、[JohnJiangLA](https://github.com/JohnJiangLA)、[html5challenge](https://github.com/html5challenge)、[iFwu](https://github.com/iFwu)
> * 本文永久链接：[https://github.com/xitu/gold-miner/blob/master/TODO/state-of-vue-report-2017.md](https://github.com/xitu/gold-miner/blob/master/TODO/state-of-vue-report-2017.md)

## 序

几年前，Monterail 因其在 Ruby 和 Rail上 的专业建树，还是一家享有盛誉的软件开发商。不过现在看来，Monterail 和她的产品似乎有点过时了。当我们用 Ruby开发传统多页面应用程序时，很快意识到，随着技术的进步和发展，许多的好的开发实践和规范已经发生了变化。因循守旧是无法满足市场需求的，在2011年，我们选择了 Backbone.js 作为我们涉足的第一个js框架。我们一直都积极地关注这个快速变化的世界，较早地采用了 Angular JS， 而且对其非常精通。如今，新一代的基于组件的开发框架里，我们团队已经研究了 React(包括React Native),Angular(angular2及以上)和使用最广泛的- Vue.js！

### 熟悉的不一定是好的

那些要求用Vue开发应用程序的客户在此之前，都没有听说过 Vue。可当他们使用后，都对 Vue 的扩展性和能力留下深刻印象，并希望在他们技术栈中包含 Vue。
我们认为，很多公司之所以使用那些选择有名的框架，并非是因为全面考虑相关信息做出的决定，而只是因为那些框架比较出名和耳熟而已。他们并没有意识到，名不见经传的 Vue 结合了 Angular，React 的先进的部分，并且更加友好。

### 为什么要做这份调查

当使用Vue后，我们能够更有效率地交付更好的产品，更好地推动我们的业务，使客户更加满意，我们相信，Vue 值得关注并受到大家的喜爱。正因如此，我们决心开始向发者们和企业布道，把 Vue 传播到全世界；同时，我们策划了每周的 Vue-newsletter,组织了第一个 Vue.js 的国际性大会 VueConf，创建了 Vuelidate 和 Vue-mulitselect 等 Vue 库。

你即将阅读的这份报告我们是布道与宣传 Vue 的另一个里程碑。报告有三个主要目的。1.提供可信赖的Vue商业使用案例，让任何人都能够一窥其它公司是如何使用 Vue；2.让那些没有听说 Vue 的人了解 Vue，并让他们有足够的理由来更加仔细了解这个框架；3.让我们不再费力地说服客户相信 Vue.js 已经是一个成熟的解决方案，可以帮我们构建各类应用。

### 报告的内容

享受阅读吧！

**报告**展示了从企业主和开发者的角度去看待 Vue。我们调查了来自88个国家的1100多名行业专家，了解他们对于 Vue 的使用体验，他们喜欢的特性和那些不喜欢的特性；我们深入采访了6家公司，询问他们想用 Vue.js 解决哪些问题；另外，为了让读者对 Vue 近几年的发展有一个全面的了解，我们讲述了 Vue.js 的历史，以及框架的创建者尤雨溪对 Vue.js 未来的想法。

![](https://i.niupic.com/images/2017/10/31/fXsajR.png)

报告的顺利完成得到了许多人的支持。他们分享他们的知识和经验，给予了我们莫大的帮助，仅仅因为他们想为社区贡献一份属于自己的力量。

感谢 Evan You（尤雨溪）。他从一开始就对这篇报告抱以热情，并在创建报告过程的各个阶段支持我们。同时，Evan You（尤雨溪）还分享了对 Vue.js 未来和后期规划相关的宝贵看法，并对我的的努力表示支持。

感谢Vue.js的核心成员 Chris Fritz 和 Evan ，对我们分析调查结果给予了很大的帮助。真的很荣幸！因为有了这样的合作，我们对最终的报告质量非常满意。<br>

非常感谢 Jacob Schatz, Sylvain Simao, Roman Kuba, Gilles Bertaux, Scott O’Brien, Erin Depew, Matt O’Connell 和 Yuriy Nemtsov。没有你们花费间分享们们的故事，报告中的学习案例就不会存在。

### 主要贡献者

![](https://user-gold-cdn.xitu.io/2017/11/21/15fdc7d743074a0d?imageView2/0/w/1280/h/960/format/webp/ignore-error/1)

## Vue.js 的演变

你知道 Vue 第一次发布是在什么时候吗? 最初它甚至并不叫「Vue」。作者的首次提交是在 2013 年 06 月 27 日，那时项目叫「Seed」，转瞬间，Vue.js 已经四岁了。「Seed」这个名字用了六个月，在 2013 年 12 月初，作者把它正式更名为「Vue」。但是，Vue 的第一个对外的版本（0.8.0）在 2014 年 2 月 才发布，在那时候，Vue.js 还只关注 MVC 架构中视图（View）部分。

Vue 具有几方面重要的特性，使得它很容易被开发人员接受。 Vue 的模板语法风格很像 AngularJS，也有被 React 引入的基于组件的架构 这样，开发者可以从二者平滑地过渡到 Vue。我会把 Vue 想象为一个继承了父母（AngularJS，React）优秀基因的孩子，它自己也不断地提升开发者的使用体验。

也就在一年后，当时 Laravel 社区（一款流行的 PHP 框架的社区）首次使用 Vue，JS 社区才对 Vue 越来越感兴趣，也才真正的流行起来。几个月之后，期盼已久的 1.0 版本终于发布了，对于 Vue 来说，这是具有里程碑意义的一次版本发布。

与此同时，vue-router（2015-08-18）、vuex（2015-11-28）、vue-cli（2015-12-27）相继发布，这意味着 Vue.js 从一个视图层库发展为我们现在所说的渐进式框架。

去年，备受期待的 2.0-alpha 版本发布，它被彻底重写了，同时引入了一些新的概念，比如: Virtual DOM 和服务端渲染。但是，API 基本没有变化，因此从 1.0 到 2.0 版本可以平滑迁移。使用官方出品的[迁移工具](https://githubcom/vuejs/vue-migration-helper)会帮助你完成迁移过程。

### 社区

在接近一年的时间里，至今依然活跃的社区促使 Vue.js 成为了 JavaScript 三大顶级框架之一，而且看起来并不会止步不前。

人们非常喜爱 Vue。不要相信我们带有情感色彩的评估，看看这个数字：Vue 是 2016 年 GitHub 上 star 数最多的框架。

社区的兴趣是非常浓厚的，当我们启动 [Vue Newsletter](http://vue-newslettercom/) 项目时，在几分钟内，便有数百人订阅了。一直没间断的邮件通知，让我们感觉自己就像 Instagram 的明星一样（备受关注）。Newsletter 的第一期有 759 人订阅，而到了 63 期，我们的订阅人数已差不多达 6000 人。每一期都是很难准备的，因为每周都产生很多和 Vue 相关的内容。每天都有高质量的教程、见解深刻的文章以及我能想到的库翻陈出新。有点疯狂。这还不是全部，Vue 社区有一个[活跃的论坛](https://forumvuejsorg/)和一个[聊天频道](https://chatvuejsorg/)，每天都有成百上千的开发者活跃在上面。

此外，我们可以发现，随着开发者对 Vue 的兴趣逐渐浓厚，全球很多公司开始关注 Vue。点击 [vuejobscom](http://vuejobscom/)，看看他们发布的的职位吧。

### 生态

值得一提的是，除了社区项目之外，Vue 核心开发团队也维护了一些官方库，比如 vue-router、vue-loader、vuex（状态管理库）、vue-rx 以及针对 RxJS 开发的 vuex-observable。还有一些工具库，比如 vue-cli、vue-server-renderer、vue-loader、vetur、vue-migration-helper。它们为什么重要? 因为这样，你就可以渐进式地使用其他核心库，这些库可以完美配合，使得 Vue 转变为一个像 Angular、Ember 一样完善的框架。当然，如果你的项目需要，你可以随时将其中的一部分切换为其它非官方的解决方案。官方库的另外一个好处是它们往往代表着高质量、长期支持以及与 Vue 良好的兼容性。

正如大家所料，像 Vue 社区这种大型而且参与感高的社区，会出现大量社区项目 不仅仅是小型项目、解决单一问题的库，我们现在来谈谈大型项目 举个例子，[Nuxtjs](https://nuxtjsorg) 是一个很有想法的基于 Vue 的框架，它采用了一些小工具库以及设计模式，这使得开发需要服务端渲染的应用变得极其简单。

[Quasar 框架](http://quasar-frameworkorg)可以帮助开发复杂的移动和桌面应用。还有其他流行的UI框架，比如：[Element-UI](http://elementelemeio/#/en-US) 和 [Vuetify](https://vuetifyjscom/)，这些框架提供了几十个风格统一的 UI 组件来帮助你开发 Vue。在移动端开发方面，得到了 [OnsenUI](https://onsenio/vue/) （由Monaca开发） 和 [NativeScript](https://wwwnativescriptorg/blog/a-new-vue-for-nativescript) 的大力支持。


从我作为一个 Web 开发者的角度来看，我可以向你保证 Vue 已经有你开发应用所需的一切了。每周，我都见证越来越多的库发布，以至于没有办法追踪所有的库。你可以在 [awesome-vue](https://githubcom/vuejs/这里) 找到这些库。此外，Vue 核心开发团队在 [curatedvuejsorg](http://curatedvuejsorg/) 管理了一些推荐的库，这些库主要用于表单验证、国际化、AJAX 等常见的任务，避免开发者在选择合适的库出现选择恐惧症。

### 支持

许多人指出，和 Angular 或 React 不同的是，Vue 背后没有大公司的支持，而且看起来这也不太乐观 我绝不同意。Vue 和 jQuery、Babel、webpack 以及 JS 世界中其它可被信赖的工具一样体现了真正的开源精神。 这样有一个明显的优势：这些项目不用去满足这些公司的特定需求，取而代之的是更专注社区的需求。

Vue 实现了很多社区最需要的功能 说起 code spliting，webpack 核心开发团队成员 Sean Larkin，这样评价 Vue：

> 首个使用 webpack 来提高开发者体验的框架。

但在开发体验上已经远远超越 webpack，而且体验在各个方面: 易用性、无缝集成、优秀的文档、整体的可扩展性。

显而易见，Vue.js 和很多其它开源项目一样，刚开始是一个个人作品。 慢慢地，它拥有了一个全职核心团队，专门负责维护它的各个方面和生态系统。

基金会呢? 近两年，通过在 Patreon 和 Open Collective 上的成功运作，全球的很多个人和公司决定每个月固定赞助尤雨溪（Vue 作者）和核心团队超过 10000 美元。这样，尤雨溪就可以全职从事 Vue 的开发了。

赞助者包括许多公司和几百位个人赞助者。在[这里](https://vuejsorg/support-vuejs/)可以看到这些赞助者们。

### 成长

让我们通过一组数字来更直观地感受到 Vue 生态的快速成长。

以 GitHub 的 star 数为例，尽管它不是衡量一个项目知名度的完美指标。但开发者们很兴奋，而且这份兴奋使得 Vue 成为 [2016 年 Github 上获得 star 数最多的项目](https://risingstars2016jsorg/#all)。不限于 JavaScript 或者前端分类，在2016年，它是获得star数最多的项目。过了一段时间，到现在为止，它已经是 star 数第二多的前端框架了，仅次于 React。同时，它也是 GitHub 上 star 数第六多的项目，已经超过了 jQuery 和 Angular。

[2016 年前端调查](https://stateofjscom/2016/frontend/)显示: Vue 是用户满意度最高的语言之一，89% 使用过 Vue 的开发者表示会再次使用 Vue。

当然，还有其他指标来衡量 诸如 npm 上每个月的下载量（大约 800k），开发者工具每周活跃用户数达到 270k。npm 上的下载量相比 React 的下载量相差很小。但值得一提的是：在过去的十二月，Vue 的下载量增长了 5 倍。以 Vue 现在的增幅，我相信在未来几年，这个数字将会以更快的速度增长。


事实上很大一部分的增长是因为越来越多的公司选择 Vue 作为主要的前端框架。除此之外，开发者们很欣赏 Vue 平滑的学习曲线、集成到现有的技术栈的便捷，以及顶尖的性能。也许最重要的因素是提升开发效率和减少维护成本。换句话说，选择 Vue，省钱。

但不要只信我的一家之言。为此，我们对来自 88 个国家的 1126 位开发者做了调研，并收集了一系列来自不同行业的采用 Vue 的案例。

## 使用 Vue.js 的开发者调研报告

我们很好奇软件开发者以及技术主管们都是如何看待并使用 Vue.js 的，因此我们分发了一份网上问卷给他们，其中列举了以下这些问题：

- 为何要将 Vue 加入你们的技术栈？
- 使用该框架能带来哪些好处？
- 如果考虑在项目中使用 Vue 的话，你们会主要担心哪些问题？
- 你们使用哪些资源以便熟练地使用 Vue.js？
- 你们的同事中有多少也在用 Vue？你们觉得在未来一年里这个人数会上升吗？
- 你们和你们的团队分别使用 Vue.js 多久了？
- 你们公司还使用过哪些其它的前后端技术？

### 报告的数据说明

该报告中的所有数据来源于我们在 2017 年的八月至九月进行的一次为期四周的调研。我们总共收到了 1,126 份问卷回复，大多来自于使用 Vue 的组织中的技术主管及软件开发者们（94.1% 的问卷回复者都承担相关的技术工作）。这些回复者们来自世界各大洲（除了南极洲），总共 88 个国家。

我们在撰写该报告的同时还针对一些调研结果咨询了 Vue 的创始人尤雨溪以及 Vue 的核心成员 Chris Fritz，他们为我们提供了一些独到的观点并分享了更深远的洞见。

### 主要观点

- **96%** 的调研回复者表示会在他们的下一个项目中继续使用 Vue.js。
- **94%** 的回复者使用官方 Vue 文档作为他们了解该框架的主要资源。
- **81%** 的回复者说 Vue 的集成很方便，这是他们在自己组织中的技术栈里推行它的一个主要好处。
- **54%** 的回复者相信在未来 12 个月里，Vue.js 会在自己的组织中变得愈发流行。

### 调研问卷中的问题

#### 将 Vue.js 加入技术栈中的最主要原因是？

不管开发者们新建还是接手已有的项目，他们基本一致地认为：Vue.js 很容易上手，哪怕是对于一个非常复杂的应用而言。他们评论说集成 Vue.js 很容易，原因在于它使用简单、架构优雅、同时设计精巧。不仅如此，他们还在将其与其它主流框架对比后声称 Vue 更轻量、性能更优，是毋庸置疑的胜者。总的来说，**超过半数的问卷回复者都认为 Vue.js 是个对入门者相当友好的框架。**

**将 Vue.js 加入技术栈中的最主要原因**

![](https://i.loli.net/2017/11/01/59f9674ec9cac.png)

- Vue.js 上手很容易 59%
- 技术栈需要更新了 22%
- 团队想尝试下这个框架 10%
- 其它原因 9%

> 很适合用于现有的或者新项目，而且用起来很容易！
>
> —— 技术主管，大企业，法国

> 集成进现有应用中，或者实现个纯单页应用都很方便。
>
> —— 软件开发，中型企业，澳洲

#### 你和你的团队考虑将 Vue.js 加入技术栈的时候会有哪些顾虑？

对于这个提问，回复者们提到了两个主要担心的问题。首先的一点是关系到自己团队成员的，45% 的回复者都表示，这些成员们 **缺乏 Vue 的相关经验** ，而这会是他们在考虑将 Vue.js 加入技术栈的时候可能面临的问题。

**考虑将 Vue.js 加入技术栈时的顾虑**
该题为多项选择，因而结果总和超过 100%

![](https://i.loli.net/2017/11/01/59f96a6bb6cff.png)

- 同事们缺少 Vue.js 相关经验 45%
- 不确定该框架的未来趋势 45%
- 缺少成熟的相关原生应用开发平台 23%
- 对该框架的扩展性有所顾虑 15%
- 其它顾虑 12%

> Vue 在手机上的支持是在持续提高的。现在 Vue 已经提供了对 Progressive Web Apps 的强大支持，这其中包括了我们提供的可靠模板。社区项目中像是 Onsen UI 就简化了构建类 native 的 hybrid UI 的过程。
>
> —— Chris Fritz，Vue.js 的核心开发

> 我们现在就有 Weex 和 NativeScript（译者补充：来支持开发原生应用）, 但我们也承认这两者都有很多改善空间。Weex 其实被阿里巴巴用以线上开发已经很长一段时间了，也是其在手机开发领域上的主要选择。但 Weex 欠缺了一些英文文档和学习资料。为了弥补这一点，我们也已准备在接下来一年内提供官方指南，帮助大家使用 Vue 来开发 Weex。（译者补充：现已有[官网教程](https://weex.apache.org/cn/guide/intro/using-vue.html)）
>
> NativeScript 也是个很成熟的技术了，虽然它和 Vue 的集成还相对年轻，但每天进展飞速，令人印象深刻。所以如果你对使用 Vue 来开发原生应用有兴趣的话请一定要关注下。
>
> —— 尤雨溪，Vue.js 创始人

**缺少成熟的原生应用开发平台** 也被相近比例的回复者提到，这也是他们在将 Vue.js 加入技术栈前的顾虑。

有 172 个被调研者勾选了对 Vue.js 扩展性的顾虑，这使得该选项成为五个阻碍着开发者们拥抱 Vue.js 的主要原因之一。

> Vue 的开发是基于组件化模型的，这也是现在所有主流框架中共享的一种适用于 UI 开发的设计模式。对于单页应用，Vue 提供了官方支持的路由库，也支持大规模状态管理。Vue 的设计初衷是轻量级易上手，但支持规模化也被我们设计在案。
> 
> 现已有很多成功的大规模项目是使用 Vue 打造的，有些甚至由几百个组件构成还照样运转得很顺利。另外值得一提的是，一些现有的大规模应用都在用 Vue 重写，我们收到了来自这些应用开发者们非常肯定的反馈，比如 Adobe Portfolio 和 JSFiddle。
>
> —— 尤雨溪

#### 使用 Vue.js 给你的组织带来的最大好处是哪些?

**81% 的开发者都强调了 Vue.js 的易于集成**，这个比例很惊人。大多数回复者都谈到要想熟练掌握 Vue 很容易，而且比起其它主流框架来说更容易。他们还称赞其**与后端框架集成也不复杂**。

60% 的开发者还提到 Vue 的文档是其亮点。差不多比例的回复者（56%）认为该框架的性能优异是其最大的优势。

**Vue 最大的优势**
多项选择，结果总和超过 100%

![](https://i.loli.net/2017/11/01/59f96ed5e1c69.png)

- 易于集成 81%
- 文档详尽 60%
- 性能优异 56%
- 与时俱进 49%
- 社区活跃 29%
- 其它优势 4%

> Vue.js 的学习曲线很平缓，很多人因此产生兴趣。
>
> —— 高级开发，中型企业，新西兰

> 我们之前在 React 和 Vue 之间进行过抉择，最后我们选择了 Vue，至今我们都很庆幸我们的选择。
>
> —— 软件开发，中型企业，美国

> Vue.js 使得前端开发容易管理也易扩展。它的学习成本也不高，这使得后端开发们也不需要太多指导就能清楚前端这边的工作。因为现在已经有很多好用的 webpack 相关配置，使用 Vue 现在有点像是装个插件一样。最后说一点，运行时和编译时我们都能使用 Vue.js，它真的是个很棒的工具，无论是对于小型的应用来说还是大型应用而言，想要扩展都不太难。
>
> —— 软件开发，小公司，菲律宾

#### 有哪些建议是你想对 Vue.js 提的吗？

对于这个开放式问题，我们收到了 481 份有效回答。由于有些建议被 20 多人提到了，因此我们决定列举几项比较共性的建议，再开放个单选题。

缺乏 Vue 相关的原生开发解决方案是几个最大的问题之一，24% 的回复者都同时提到了这点。毫无疑问地，**Vue.js 需要更先进完善的移动端解决方案**。

15% 回答这个问题的都指出 Vue 还有个不足是其**生态环境相对较小**。如果其生态环境能更强大的话，它一定能孕育出更为优秀的组件库。

除此之外,

> **随着下一版 CLI 的更新，Vue 的工具也会得到改善**，尤雨溪如此保证。

在这些回复中，还有人提到说 Vue 缺少一些官方教程（一个回复者称为《 Vue 圣经 》），或者一份能提供更多现实案例，特别是针对复杂应用的指导手册。Christ Fritz 指出，

> **现在已经发布的[官方风格指南](https://vuejs.org/v2/style-guide/)某种程度上来说可作为 Vue 圣经，但在开展调研那时还没提供。**

同时还有个建议是， **该框架需要一份更完善的文档**。有 53 个回复者提到了和该建议直接相关的一些问题（比如建议多提供些用 Vue 构建一个大型应用的架构设计文档），以及和该建议并不直接相关的问题，比如一些他们错误地认为不能用 Vue 解决的问题。有两个问题被 20 多个回复者都指出了，一个是需要加强测试工具，另一个是需要**优化核心库**。

**对 Vue.js 的建议**

![](https://i.loli.net/2017/11/01/59f977f3035c6.png)

- 需要更先进完善的 Vue 原生应用客户端解决方案 116票
- 需要更强大的生态环境，能提供更优秀的组件库和工具组 74票
- 需要官方教程以及其它相关学习资源，以期提供更多现实案例和最佳实践（特别是复杂应用相关的） 67票
- 需要更完善的文档，以便更顺利地开发应用 53票
- 需要更棒的测试工具和库 37票
- 优化核心库 21票

> 我们将在十一月起认真撰写使用手册，以便为构建大型应用、通用集成方案、架构设计探索等问题提供示例。
>
> —— Chris Fritz

#### 开发下一个项目时，你有多大可能会再次使用 Vue？

超过 **95% 的回复者声称他们在下一个项目中还会使用 Vue**。许多开发者明确表示他们使用过该框架后，之前的顾虑都不再是问题。即使他们还是指出了它的一些不足和值得改进之处，但几乎所有人在用过该框架后都对其称赞有加。同时绝大多数回复者选择在下一个项目中依然使用 Vue。

**在下一个项目中会使用 Vue 的可能性**

![](https://ooo.0o0.ooo/2017/11/01/59f98213a9d6f.png)

- 5（非常高）82.9%
- 4 12.5%
- 3 3.5%
- 2 1%
- 1（非常低）0.1%

#### 你所在的组织机构使用 Vue.js 有多久？

随着 Vue 社区的逐步壮大，精心打造的相关项目在世界各地层出不穷，同时它也跻身于 [GitHub 上星数排名前十的仓库列表](https://github.com/search?p=1&q=stars%3A%3E1&s=stars&type=Repositories)，Vue 愈来愈受到普遍认同。**超过 3/4 的回复者在近一年内将 Vue.js 加入了他们的技术栈中**。

我们可以预见在未来几年内使用 Vue 的开发者数量会飞速上涨，同时该框架自身也在不断变得成熟，其生态环境将不断强大，也会有越来越多的使用案例。

**你所在的组织机构使用 Vue.js 有多久？**

![](https://ooo.0o0.ooo/2017/11/01/59f984a53aeeb.png)

- 少于 6 个月 45%
- 6–12 个月 34%
- 1–2 年 19%
- 超过 2 年 2%

#### 学习 Vue.js 时你会使用哪些资源？

**官方 Vue 文档是最普遍使用的参考资源。** 94% 的软件开发者都勾选了它，这也说明了，一份深思熟虑后发布的文档是学习任何框架的主要资源。另外，70% 受调研的软件开发者还选择了线上文献、技术博客、一些社区像是 StackOverflow 或者官方 Vue 论坛等作为知识来源。线上课程受到了 41% 开发者的青睐，而选择了在职培训、相关书籍的只占 1/4 不到。

**Vue.js 的学习资源**
多项选择，结果总和超过 100%

![](https://ooo.0o0.ooo/2017/11/01/59f987f910880.png)

- 官方文档 94%
- 线上文献及博客 78%
- 线上社区（比如 StackOverflow、Vue 官方论坛） 72%
- 线上课程 41%
- 在职培训 22%
- 书籍 12%
- 其它 5%

#### 你觉得你所在的组织机构中使用 Vue.js 的员工比例会在一年内增长吗？

**54% 的回复者相信 Vue.js 在未来一年中，将在其组织里变得愈发流行。** 然而那些在大型企业（超过 1,000 员工）工作的开发人员更确信 Vue 在其公司会被广泛接受：76% 的受调研者勾选了赞同。

**使用 Vue.js 的员工比例会上升吗**

![](https://ooo.0o0.ooo/2017/11/01/59f98810daa31.png)

- 5（绝对会）33%
- 4 21%
- 3 24%
- 2 11%
- 1（绝对不会）11%

> 公司的其它项目都打算使用 Vue（甚至已经开始用了）。
>
> —— 软件开发，大型企业，法国

> 我们在疯狂扩招，有非常多的项目将要涌现。这些项目都会使用 Vue.js 来开发。
>
> —— 技术总监，大型企业，德国

#### 你主要使用的前端技术和框架是哪些？

**主要使用的前端框架**
多项选择，结果总和超过 100%

![](https://ooo.0o0.ooo/2017/11/01/59f9883bf1687.png)

- Vue.js 33%
- Angular 21%
- ReactJS 24%
- 其它 11%
- Backbone 6%

#### 你主要使用的后端技术与框架是？

**主要使用的后端语言与框架**
多项选择，结果总和超过 100%

![](https://ooo.0o0.ooo/2017/11/01/59f98eac1734c.png)

- PHP 53%
- Node.js 45%
- Java 18%
- C#/.Net 17%
- Python (Django、Flask等框架) 17%
- Ruby (Rails等框架) 10%
- 其它 8%

### 受调研人员数据

我们对来自 88 个国家的 1,126 名熟悉 Vue 的软件开发者、CTO、以及其他相关技术人员进行了调研。

**公司规模（员工数量）**

![](https://ooo.0o0.ooo/2017/11/01/59f98f1be43bd.png)

- 小型企业（少于 100 人）77%
- 中型企业（100-999 人）15%
- 大企业（超过 1000 人）8%

**团队规模（组员数量）**

![](https://ooo.0o0.ooo/2017/11/01/59f98f761c64e.png)

- 小团队（2-10 人）73%
- 个企 17%
- 中型团队（11-25 人）8%
- 大型团队（超过 25 人）2%

**在组织中担任的职能**

![](https://ooo.0o0.ooo/2017/11/01/59f98fcd2ddaf.png)

- 软件开发 66%
- 技术主管 20%
- 其他技术人员 8.5%
- 项目经理 4%
- 其他 1.5%

## 案例研究

起草这份关于 Vue.js 现状的报告，是想通过大量的数据来证明，Vue 已被不同种类、不同规模的公司采用，已然成为了一门成熟的技术。每一个研究案例都证明了 Vue 是足以应对商业用途的。我们采访了六家公司，他们都曾面临着选择一套合适框架的挑战，即使他们处在不同的发展阶段，也有着不同的目标，但是他们最终都选择了 Vue。

在 Codeship 和 Vue 结合之前，他们的用户忍受着卡顿甚至是浏览器崩溃。太多的用户对他们的应用程序心有不满。他们的故事很好地证实了，Vue 可以有效地帮助构建安全、可靠、易维护且具有防御性的应用程序。

如果你正在寻找 Vue.js 的优秀企业级案例，那么 Behance 和 Adobe Portfolio 的案例就可以派上用场。他们的团队使用 Vue 零基础地建立了两个独立的产品，而且不会止步于此。

在 Livestorm 案例中，Livestorm 联合创始人兼 CEO Gilles Bertaux 描述了他们如何从零开始创造一个可盈利的产品。得益于 Vue 及其可复用的组件，他们的开发速度更快也更容易。

GitLab 的前端 Leader Jacob Schatz 解释了为什么他们决定从 jQuery 技术转移到 Vue.js，同时分享了他们遇到的主要挑战。他们专注于更好的 UX （用户体验），这使得他们的产品更为理想，销量也因此提升了。

Chess.com 则不得不处理 Angular 1 项目中难以维护的遗留代码。他们发现，Vue.js使得 15 位远程开发人员的团队协作更容易。Chess.com 是一个服务全球 1900 万用户且拥有大规模基础设施的平台。在他们的案例中，你将了解 Vue.js 是如何化解了他们的难题。

最后一个案例与其他案例大有不同。墨尔本 Clemenger BBDO 的技术主管 Sylvain Simao 介绍了如何用 Vue.js 开发 4 到 12 周的短期项目。应对紧张的交付周期、大量的动画和特效需要实现、活动页面的高性能要求是他们面临的最大挑战。

### Behance 和 Adobe Portfolio

**Behance** 是展示和发现创意作品类在线平台中的引导者。 
**Adobe Portfolio** 可以让（用户）打造自己专属创意作品展示网站的定制平台。

> 我们曾因为当时并没有太多大公司使用 Vue 而犹豫。但是，每当我遇问题（通常都是因为我的多虑），Vue都可以很容易的解决，这让我感到惊喜。
>
> ——
> Erin Depew， Behance 软件工程师 
> Yuriy Nemtsov， Behance 软件工程师兼经理 
> Matt O'Connell， Adob​​e Portfolio 软件工程师

#### 挑战

从自产解决方案转移到开源技术。
保持良好的用户体验和高性能。
能够在其他团队和项目之间共享组件。

#### 解决方案

将 Behance 和 Adobe 前端团队转型到 Vue.js。 
使用 Vue.js 来迁移现有的代码库。

#### 成果

可以不紧不慢地迁移网站，而无需从头开始。
轻松整合现有代码库。
高性能，低成本。

### 挑战

Behance 是 Adobe 旗下的一家子公司，多年来他们一直在利用最新的技术和设计思想创造能够联结并壮大创意世界的革命性的产品。

该团队已决定使用开源框架，因为他们开始受限于目前已经使用的自产技术。

> Yuriy 解释说，在 Vue 之前，我们一直在使用自主研发的一个 MVC 框架，它依赖于 Hogan.js（mustache）和 jQuery。我们的框架无法以声明方式渲染 DOM，这迫使我们只能手动同步数据到 DOM 上。它也无法将功能抽离成组件，控制单向数据流，也没有全面的文档。所以尽管已经使用了几年，我们还是决定转向一个可以让我们能够快速构建，减少出错，降低成本，快速上手的技术方案。

![](https://i.loli.net/2017/11/02/59faea0ada687.jpg)

> Mustache 对我们特别重要，因为当时我们在前后端使用了相同的模板（现在多数 behance.net 的项目中依然如此）。利用 Mustache 将首屏快速提供给浏览器对于我们和用户都是非常重要的。如果我们等待浏览器下载 JS，解析，编译和执行它，然后才将页面显示给用户，要想达到与使用 Mustache 时同样的速度是非常困难的。我们也特意寻找过具有服务器端渲染功能的框架。

对于 Behance 团队，首要目标是构建一个易用的代码库，并为今后添加的新功能打下坚实的基础。

> 我认为我们面临的最大挑战就是，由于我们决定不拆分我们的代码库并从一个新平台开始，我们不得不花费大量的时间抽离旧的代码来形成新的组件。Erin 补充说，既要用 Vue 重构旧代码并保证网站其余功能正常运行，又要实现新功能，如何权衡这两件事确实是个挑战。

> 我们非常重视 Behance 的性能，所以我们非常小心，以确保在迁移代码库的同时保持性能指标。

对于 Matt 和他的团队来说，用户体验也是很重要的一点，并且有很大的改进空间。

> 关于 Adobe Portfolio，我们一开始使用 nbd.js，这是一个从原本我们已经不再维护的产品中提取出的 Backbone 自定义版本，称为“在线操作”，我们用它来构建 Behance 网络的模块。Matt 补充说，它对反应式系统有限制，因此我们使用 Ractive 构建了“反应性”部分。

> 就 Behance 的情况来说，迄今为止最大的挑战就是，在复杂的用户数据状态管理下保持快速的用户体验，同时保证站点的内容和样式的即时反馈。

### 解决方案

Adobe Portfolio 和 Behance 重新培训其现有的团队使他们可以在日常工作中使用 Vue.js，而不是重新组建一个只关注于 Vue.js 的新团队。

> 在我们切换到 Vue 之前，绝大多数的团队都在这里。一旦我们决定采用 Vue，我们需要一些小项目来练手。对我们来说，只需要非常小，只有前端功能且不公开访问的站点即可，就像我们的样式指南。这样，我们可以学习如何使用 Vue，如何编写测试，并相对安全地对组件进行风格化。只有这样，我们才能安心投入更大的项目。我们于是就用 Vue 开始打造 Behance Live，Yuriy 回忆说。

![1509617601(1).jpg](https://i.loli.net/2017/11/02/59faefebec94a.jpg)

> 在 Portfolio 项目中，我们 9 人的前端团队都开始使用 Vue。我们的一些后端开发人员也开始学习 Vue。 Matt 解释说，Behance 产品中约有8位前端开发人员在使用 Vue 进行开发。

> 两个团队确实有一些功能上的重叠（Adobe Portfolio 和 Behance）。Erin 补充说，我们在代码库之间共享了许多库和 API，而且一些功能的展现通常需要两个站点一起合作。

Behance 团队在定义如何构建应用程序的一般方法以及如何定义不同组件的角色方面遇到了许多挑战。

> 对于比较大的应用程序，vuex 存储区也很难构造。我们决定使用命名空间模块。一开始我们不清楚每个路由/页面或数据类型（例如用户或项目）是否应该存在单个存储模块。创建特定的路由存储意味着跨路由的操作将不可重用。对我们来说，使它们具有数据特性是最好的解决方案，其中包含一个顶级路由存储模块，它结合了路由所需的模块。但是，这个解决方案还不够完美。Yuriy若有所思地说。

> 为了定义各种组件的角色，我们区分“页面”组件（路由器指向的第一个组件，也是与 vuex 交互的组件）和木偶组件（仅将属性发送到子组件，将事件传输给父组件）。

使用 Vue.js 将近 1 年后，Matt 和他的团队终于构建和重构了一堆功能。

> 在 Adobe Portfolio 中，我们从内容管理功能入手。内容管理允许用户可以在自己的 portfolio 网站上进行重新排序，添加，删除等操作。根据需求，我们构建了可复用的 UI 组件，如选择下拉列表，浮窗，切换控件和拖放列表，Matt 说。

### 成果

据 Erin 介绍，由于 Vue 具有先进性和灵活性，Vue 易于和 Behance 现有的代码库集成。

![1509617746(1).jpg](https://i.loli.net/2017/11/02/59faf0615bbaf.jpg)

> 我总是说，每个框架仅仅是另一个工具而已。然而，除了更新快和易阅读的文档之外，使用 Vue 的最大好处就是可以将其集成到现有的代码库中。与其他基于组件的框架不同，Vue 给予我们在现有的页面嵌入组件的能力，使我们能够以自己节奏更新站点，而不是全部替换。

> 我会说 Vue 超出了我们的期望。我们曾因为并没有太多大公司使用 Vue 而犹豫。但是，每当我遇到问题（通常都是因为我的多虑），Vue 都可以很容易地解决，这让我感到惊喜。她笑着说。

> 目前，我们正在计划将我们的整个 Behance 代码转换为 Vue，当然，也在推荐 Adobe 的其他团队使用 Vue。

Yuriy 认为，Vue.js 提供给开发人员的可能性与其他框架一样多。然而，与一些框架相比，它使开发更容易...也更便宜。

> 我不敢说 Vue 能帮你做一些其他的框架做不到事情。但是，使用 React 的话，提升 SSR 的性能确实事件很难的事。在使用 Fiber 重写（React v16）之前，一个具有巨大组件树的页面将阻塞主线程，反过来说，这就意味着如果需要 100ms 来渲染一个页面，那么 Node 服务器的所有其他客户端就只能等待。因此，我们需要增加单个服务器的进程数量或增加服务器数量来提高吞吐量。这很难维持，而且非常昂贵。Vue 的 SSR 情况就强大很多。Vue 有内置缓存和流式传输，因此即使不做大量优化，Behance Live 的性能也很好。

> 使用 Vue.js 绝对与使用其他框架不同。不知何故，你会爱上他的。

![1509617816(1).jpg](https://i.loli.net/2017/11/02/59faf0a462160.jpg)

### Chess.com

Chess.com 是排名第一的在线国际象棋网站。来自全世界各个地方各个段位的棋手每天要对弈超过 100 万局。Chess.com 是由 100 位成员组成的完全远程工作的团队。

> 这是我第一次一口气阅读完整的文档。现在是凌晨 1:30。当我看完时，我知道了 Vue.js 是个特别的东西。它有一些独特之处。一些我从来没有见过的东西。
>
> Scott O’Brien，Chess.com 首席用户体验工程师

**挑战**

处理难以维护的 Angular 1 遗留代码。

引入新特性以增加用户参与度。

在一个完全分布式的开发团队中管理变更。

**解决办法**

对所有可用的框架进行基准测试。

从 Angular 1 迁移到 Vue.js。

构建日益增长的组件库（连同它的模块化 CSS）。

**成果**

使得全远程的团队合作更加愉悦。

app 内编写 CSS 更加高效。

与其他框架相比，在速度、能力和抽象方面更有效地进行扩展。

#### 挑战

Chess.com 是国际象棋领域中访问频率最高的网站，拥有多达 1900 万成员庞大的社交网络。它有新闻，博客，社区，教程，谜局，当然也包括实时对弈。网站门户的复杂性是巨大的。

遗留代码是用 PHP 和 Angular 1 编写的。任何时刻，Chess.com 都承载着网页上或手机上成千上万的实时对战游戏。对于这样一个网站来说，性能是第一位的。

> 我们已经知道使用 Angular 1 是一个巨大的性能瓶颈。这个问题会变得越来越大。从性能角度来看，我们网站的有些部分在一些传统的硬件设备上已经变得无法使用。它是无法维护的，Scott 回忆说。

Chess.com 面临的挑战不仅是处理现有的功能，也包括对新功能的规划

![](https://ooo.0o0.ooo/2017/11/03/59fc0a031aef2.jpg)

> 大部分讨论都是关于架构，因为我们知道需要加入很多新的功能以保证用户下更多的棋并尝试各种不同的下棋方式，Scott 解释说。

> 我不是说用 Angular 就做不了，只是用这些过时的 javascript 框架很难做到。

为了提高用户体验， Chess.com 需要做一些真正的改变。

> 我知道我们需要一个质的飞跃。从 Angular 1 迁移到哪个框架让我们深思熟虑。当然，我们有考虑过两位大佬：Angular 2 和 React。

庞大的基础设施和持续的产品开发需要一个组织良好且规模庞大的团队。

> 在我们的开发团队中，有各种各样的技术栈。此外，我们的团队是完全分布式和国际化的。任何像技术迁移一样重要的决定都会引起很多人的关注。

#### 解决办法

选择一个由 Facebook 或 Google 支持的框架，如 React 或 Angular，相对来说，貌似是一个比较安全的选择。但是，Vue.js 社区证明这个新来者无疑是一个强力的竞争者。

> 我们是如此的关心性能以至于我们可能会选择对开发者不那么友好但基准测试看上去不错的框架。看到 Vue.js 赢得了渲染和性能的基准测试是振奋人心的，Scott 解释到。

> 我们担心的是整个 Vue.js 是建立在 Evan 的想法上的，这个框架的生死都由他主导。我们决定只要社区发展迅速并且我们相信他们在做一些革命性的事情，我们就会带头并确信其他人在将来会看到它的价值，正如我们现在看到的一样。所以最大的问题是，它是否会继续发展，我认为这已经被证实了。

Chess.com 团队首先要做的事情之一就是将不同的页面从 Vue 重写为 AngularJS。

> 重写工作现在仍在进行，目前已经持续了数月。我们的另一个任务是构建我们内部的可重用组件集，Scott 指出。

![](https://ooo.0o0.ooo/2017/11/03/59fc0a6a4a369.jpg)

> 我认为用 Vue 构建一个不断增长的组件库是一件非常酷的事情，每个组件都有自己的模块化 CSS，这些组件最终会构成我们网站上的全部用户界面元素。一个团队一直在用 Vue 来实现特定产品领域的 components、routes 和 stores，而另一个团队一直致力于构建全站共享的组件库，几乎不用担心产生冲突。此外，它还使我们的产品讨论更加抽象和复用。

#### 成果

对于一个像 Chess.com 这么大的应用来说，Vue 带来的好处远远超过其他。

> 单个文件组件绝对是构建和维护我们库的不二法则，这样使得团队能够仅仅在有官方的状态管理系统的框架部分中进行投入。我们相信这些事情会一起工作——这都是集体愿景的一部分。

有了 Vue.js，Scott 发现与远程团队合作起来更加容易了。

> 他指出，我们对Vue的热爱在于，它具有难以置信的易用性和低的入门门槛，同时具备拓展能力，与其他组件库相比，有相当的(如果不是更好)能力、速度和抽象性。

> 我们是一个完全由15个开发人员组成的远程团队，我们非常依赖 Slack, Jira 和 GitHub。然而，在 Vue 中更容易进行协作，因为它与我们的遗留代码没有太大的区别——仍然有声明式模板以及我们习惯的所有内容。

> 其次，编写 CSS 的便捷性令人惊叹。它给我们带来了巨大的利益。我们有许多开发人员说着不同的语言使用不同的编程风格，他们只需针对特定文件中的标记来命名，而不需要担心全局名称空间的名称冲突。使用方便的感觉是如此美妙。

介于 Vue 给 Chess.com 团队提供了巨大的支持，未来他们无疑将会继续使用它。

> 我们现在都在用 Vue.js！正如我说的，我们的工作分两部分：重构我们的组件，从 Angular 1 迁移。因此，我们同时用两种完全不同的方式实现，这是值得骄傲的。

![1509690042(1).jpg](https://ooo.0o0.ooo/2017/11/03/59fc0ac62efa9.jpg)

### Clemenger BBDO

Clemenger BBDO 是一个全方位的服务机构，提供包括品牌战略、综合创意开发、CX、数字服务、CRM、PR、设计、顾客和激活的全套功能

在过去的12个月里，在戛纳广告奖和创意奖上，它被评为世界上最具创意的机构。

我们决定选择 Vue.js 因为它满足了我们的项目提出的所有需求，同时为我们的团队提供了一个舒适的开发环境。它非常接近于原生 JavaScript，因此很容易上手。

> Sylvain Simao, Clemenger BBDO 技术总监，墨尔本

**挑战**

项目周期短（4 到 12 周），由多人完成开发。

使用动画和过渡效果。

移动设备上加载和运行速度要快。

**解决方案**

对静态页面使用 Vue.js 的预加载方案

构建ES6模块而不是框架特定的代码。

**成果**

按时交付多个成功的互动活动。

高流量的数字项目。

快捷的入职培训和项目初始化。

#### 挑战

Clemenger BBDO 大多数项目是活动网站。他们大部分是前端的（包含小部分后端），大多数项目使用的是无服务器的方式、API、AWS 服务等。

由于同时需要开展多个有着严格工期的项目，Clemenger BBDO 必须设计出一套标准的可以显著提高开发速度，且要有足够的灵活性，可以用于不同的项目之中的方案。

> 作为技术领导，我需要记住的一件事情是我的团队在短时间内交付高端的高质量项目的能力。我们是一家广告公司，这意味着一个为期3个月的项目真的很长，Sylvain 解释道。

> 快节奏的环境意味着我们需要人们能够快速地投入到新的工具。有时我们也需要与外部承包商合作，所以对于我们最完美的方案是那些很容易学习和用于工作的东西。Vue在工作流程方面给了我们很大的灵活性——例如，能够与已经知道的 HTML 和 CSS 的预处理器一起工作是一个很大的优势。

在客户端项目上，Sylvain 和他的团队使用了不同的 JavaScript 框架。

> 我觉得我们都试过了! Sylvain 笑道。

> 我们尝试了一些框架，比如 Angular，React，和 Riot.js。但是 Vue 最终得到了我们的青睐。Vue 即简单又不失健壮。对我们来说，这是一缕新鲜的空气。它有一个丰富的生态系统，而且它是一个渐进的可采用的工具，使它成为我们所要交付的工作类型的完美工具。

交互式活动网站到处是挑战。

> 您必须处理 SEO、可访问性和浏览器兼容性，但同时也要实现一般的动画、过渡和很多交互界面。这些无疑是我们工作中最具挑战性的方面。

#### 解决方案

由于其流畅的学习曲线，Vue.js 可以很容易让新开发人员或外部承包商使用。

> 我们注意到 Vue.js 在培训新手方面表现很不错。为什么？因为学习曲线非常平滑，非常接近原生 JavaScript，Sylvain 说。

> 对我们企业来说，它真的很棒。人们可以很快获得最新的速度，我们可以更有效率地交付。另一个值得注意的一点是，Vue 的官方文档和资源的质量令人难以置信。它可能应该得到一个最容易理解的框架文档奖!

对于每一个 Clemenger 服务的网站来说，重要的是 SEO。

> 对于这个特定的问题，我们为我们的所有页面做预渲染。大多数时候，当我们有一个新的项目需要 Vue.js 的时候，我们从基于官方 Vue webpack 模板构建的样板开始。然后，我们使用像 PhantomJS 或 Prep 这样的库来呈现页面的静态快照。最后，通过使用 Nginx 或 Lambda@Edge 等用户代理工具，很容易将这些页面提供给爬虫。

Sylvain 使用 Vue.js 来处理动画和过渡效果。

> 现在我们正在改变我们实现动画的方式。自从 Vue 的最新版本发布以来，现在的过渡效果有了更多的灵活性。我们现在有了一个更细粒度的转换钩子，这使得可以触发第三方库并实现复杂的动画，同时核心仍使用 Vue。我正努力推动我的团队走向那种模式。

对于 Airbnb 的活动设计--“Until we all belong”，技术选型是 Vue.js。

![1509690301(1).jpg](https://ooo.0o0.ooo/2017/11/03/59fc0bc9c12ea.jpg)

> 该项目最初设计为一个单页面应用，基于 Vue 和 webpack。为了提高效率，web 页面托管在 Amazon S3 bucket 中，这意味着我们不能使用任何服务器端渲染。UI 的每个部分和每个页面都是使用 Vue 单个文件组件构建的。在这样一个预期会有大流量的网站上，性能是关键，这就是为什么所有东西都按需加载。我们的一个项目记录到了每分钟 6000 个的访问量——是非常大的。我们需要做好准备，Sylvain 解释道。

> 在这种情况下，Vue.js 是救星。对于 Airbnb 项目，背景中有很大的图片资源需要加载以及应用动画。为此，我们使用 Vue-router 来声明需要预加载的资源或数据，而 VueX 则负责跟踪每一页上的内容。这个项目在交互方面也很有挑战性，但我们在6周内就成功发布了这个网站。

![1509690342(1).jpg](https://ooo.0o0.ooo/2017/11/03/59fc0bf296b5a.jpg)

#### 成果

使用 Vue.js 来按时交付项目要容易得多。

> 如果不是 Vue，我们就不会那么快了。主要是因为 API 的简单性。我们最近开发了一个基于 Angular 2 的混合应用程序的原型，语法很优雅，但学习曲线很陡峭，简单的事情也需要时间。有了 Vue，你可以快速地实现原型，这可能是它最大的优势。

有了 Vue，Clemenger 团队能够处理各种不同的项目。

> 我们现在有相当多的项目建立在 Vue.js 之上。“Airbnb’s Until we all belong”，一个澳大利亚的婚姻平等活动，已经获得了一些行业奖项，包括 AWWWARDS 和 CSSDA。另一个项目--Meet Graham which introduce the only person designed to survive on our roads, Graham。在第一周内，该项目记录了超过 1000 万的页面浏览量，并获得了身临其境的公认和媒体报道。它备受好评，并获得了众多奖项，包括 2017 年戛纳国际电影节大奖。我们最近的一个项目是 Snickers Hungerithm，这次我们决定用 Vue 重写活动应用用于全球推广。Hungerithm 是饥饿识别算法，可以通过推文来监控在线情绪。当饥饿度上升时，士力架的价格就会实时下降。

### Codeship

Codeship 是一个持续集成平台，它可以让你在云端放心地发布你的应用。在 Codeship 上的开源项目总是免费的。

> Vue 给了我们做任何想做的事情所需的灵活性。它打下了坚实的基础，因此我们可以用任何我们喜欢的方式去扩展它，它不仅仅是我们用来完成目标的工具。这是我们非常喜欢它的理由。
>
> 来自 Roman Kuba ，Codeship 前端 Leader。

**挑战**

应用内的冻结和崩溃。
使用 Angular 进行单元测试非常困难。
雄心勃勃的新功能计划以及构建新的，复杂的东西。

**解决方案**

构建一个概念验证( Proof of concept )，并以此说服其他开发人员去尝试一下 Vue.js。
只接受验收测试。
重构以及重写页面。

**产出**

自从 Vue.js 实施以来，没有发生任何应用程序崩溃的现象。
牢固（Bulletproof），可靠，易于维护的代码。
得到客户满意当前用户体验的正面反馈。

#### 挑战

Codeship 是 2010 年推出的一款 CI 平台，被 CNN，Red Bull 和 Procuct Hunt 等公司使用。 他们的技术栈中包含了 jQuery 和 CoffeeScript，他们为全球开发者建立了一个成功的平台。

但随着时间的流逝，这个团队意识到是时候该去找一个新的技术去支撑更久远的发展以及促进更复杂东西的建设。

> 给你一些观点 —— 大量的客户在他们的日常操作中依赖着 Codeship。当我们正在开发一个新功能时，通常可能需要四个月的时间，不知为何，这样总感觉不太好，就好像我们正在从顾客那里拿回什么东西。但如果我们花两个月的时间去开发功能, 就反过来了，这往往意味着两个月的痛苦并且对客户不负责。快速而可靠的提供产品对我们来说至关重要。Roman 这么说。

![1509692542.jpg](https://ooo.0o0.ooo/2017/11/03/59fc15158019e.jpg)

> 我们拥有能够完整接收终端输出的页面作为我们用户的可读日志,这样他们就可以看到什么样的测试通过了以及测试的信息。像我们之前的产品使用 jQuery，因为一些变得越来越复杂的原因，不得不将它砍掉,对比很明显。Roman 反映道。

> 接下来的六个月里面我们使用了 Angular 1。 仅仅是因为我们对它比较熟悉。

公司切换到了 Angular 而且适应的很好。然而随着服务的增长，我们发现坚持使用它从长远的角度来讲是不太可能的。

> 我们一直试图去改善的一个东西是性能。这是 Angular 里面的一个超级大问题。我们在构建的页面上需要展示的数据量远远超过了 Angular 的能力上限。客户们纷纷报告严重的问题 —— 页面无响应，有些人甚至遭遇了冻结和浏览器崩溃的现象。

即使如此，Roman 还是不想马上放弃 Angular。

> 当然，我们已经尽力去优化了。我甚至尝试将一部分的渲染工作移出 Angular 的默认渲染列表并用原生的 JavaScript 代替，但是并没有什么用。Roman 叹了口气。

> 在某一时刻， Angular 试图通过跟踪页面的范围并运行相关的 digest cycles 来把握页面上的变化。。。 这很影响性能，我们尝试去消除这一影响，但没什么用，它没有办法顺利地运行。

Codeship 面临的另一个重大挑战是改进测试过程并使应用程序变得更加可靠。

> 我们在使用 Angular 的时候还是会尽可能地利用验收测试。我们基本上会把整个应用里的用户故事都给测试一遍。使用 Angular 本身进行单元测试以及单独测试组件，模块或控制器是非常痛苦的。它几乎给不了我们所需的全部画像。Roman解释说。

#### 解决方案

得到工作人员的认可以及 VPE 的批准是从 Angular 转型的第一步。

> 起初，让所有人都同意去使用 Vue 是一场艰苦的斗争。这个团队之前从来都没有听过它，他们只知道 Angular 2 以及 Google 正在抛弃它，还有 React 和它背后的 Factbook。Roman 说。

> 在团队会议中，第一个问题通常是关于 Vue.js 社区的规模，大家想知道如果在开发过程中遇到问题，他们是否能够得到来自社区的帮助，因为我们的大部分员工都是做后端的，他们更想要坚持选择他们所能听到的可信赖的名字。

Roman 决定用他的知识和调查结果来说服他们转移到 Vue.js。

> “我做了一些样例和一个内部演示，至少要让他们相信这个决定以及决定背后的理由” 他说 “如果你简单地阅读过 Vue 的源码，你会发现独立去扩展这些代码并不困难。它不像 Angular 或者其他类似的沉重的框架。”

在 Codeship 直接投入开发之前，他们需要一个概念验证。

> 当时我对 Vue也没有太多的经验，我对框架中涉及到的技术了解十分有限。但是，从 Vue 开始似乎毫无费力，我很快就意识到这是一个针对困扰我们大多数问题的解决方案。只用了一个晚上左右，我就用 Vue 重构了一个关键部分并试图使用大量的 Loglines 作为概念验证。

![](https://ooo.0o0.ooo/2017/11/03/59fc15add61e8.png)

然后我对所有的代码做了CPU性能分析，这件事立即向我的团队证明了 Vue.js 已经给我们带来了巨大的性能提升。我们将渲染时间从30秒缩短到了7秒左右。Roman 回忆到。

概念验证在手，Roman 和它的员工终于可以开始向 Vue 过渡了。

> 我们试图移走概念验证并用 Vue 代替我们现有的系统。这里头的实际风险非常小。我们有一个对用户来说正处于崩溃的系统，所以，还会有什么更糟糕的事情会发生？Roman 笑道。

> 我通过花了一个礼拜的时间重构并重写页面，然后将它发给用户来获取反馈来快速验证工作的可行性。只过了一天的时间，我们就发现过去困扰我们的问题全部都消失不见了，甚至是在有 15 Mb 日志呈现的情况下。在渲染时间在 30 到 40 秒之间（我们正在努力进一步减小这个数字），应用在所有的浏览器上都能够出色的运行并且没有被我们记录到任何一次崩溃。

![](https://ooo.0o0.ooo/2017/11/03/59fc15e8cc1c8.png)

抛弃验收测试使整个测试部分变得更加愉快和可靠。

> 我们抛弃了验收测试，开始考虑我们可以得到什么，并使用 Jest 和 Vue 来测试。我们在 Vue 中使用多个组件，甚至是复杂的页面，但是只能通过 Jest 进行测试，因为我们有快照并验证渲染 HTML 是否是我们想要的。Roman 解释道。

#### 产出

一些很少做前端的工程师现在感觉有能力去接触一些代码片段了。

> Angular 和它的结构、模块、模型和控制器，以及几十个其他东西。。引入了不必要的高度复杂性。对于这些工程师来说，大部分名词听起来就像是奇怪的魔法一样。但是当他们真正地看到 Vue.js 的时候，他们能感觉到自己有能力去马上深入研究它。这对于我们公司来讲是一个非常大的胜利，Roman反映道。

Vue.js 帮助 Codeship 组织他们的代码并优化用户体验。

> 它可以帮助我们更快的交付所需功能，用户不需要为了他们需要的或者期望的东西来等待数个月的时间，他们非常喜欢这一点。我们的页面中有一个是基于 jQuery 运行的，它的结构非常奇怪。我们将它基于 Vue 重构了。现在，它提供了更加细化的体验和更友好的 UI 交互效果，因此，它显著地改善了用户体验。人们总是这样告诉我们。

> 使用 jQuery 的时候，代码非常混乱，难以和维护。而使用 Vue 的时候就不一样了，你可以利用它组件的强大功能和它的生态系统，比如 Vuex。我们现在正在做的是页面状态管理，这是我们以前从来没有完成过的，至少没有以这样一种干净的方式完成。

对于 Codeship 来说， Angular 测试是一个非常痛苦的过程。而用了 Vue.js，他们知道他们的代码是牢固的。

> Vue.js 确实提升了我们的测试协议。Jest对我们来说是一个比较聪明的测试工具。但是有了 Vue 之后，我们觉得我们又更多的方法来控制应用的各个方面，Roman 阐述道。

> 我可以运行 15 个执行特定操作的测试。这样的方式可以让我轻松地识别代码中的断点。在以前的验收测试中，我没办法这样做，因为这需要消耗很长的时间。得到的结果不值得我们付出那么多的精力。单元测试在这方面反而更好。在代码方面，我知道它是牢固的，因为我们以全新的方式对它进行测试，结果令人难以置信。

### GitLab

GitLab 是一个集代码托管,测试,部署于一体的开源git仓库管理软件。

> 每一个框架都有自己的适用领域，使用 Vue 的时候，每一次斗争都是你自己的，而不是 Vue 的。它只是一个完美的框架。
>
> 来自 Jacob Schatz, GitLab 前端 Leader

**挑战**

实现复杂的功能以及维护现有的功能会有困难。
大型的 Rails + jQuery 应用难以扩展。
应用速度不足。

**解决办法**

逐渐将 Vue.js 引入到 GitLab 中，以便与 jQuery 一起使用。
把 Vue.js 用在合适的新的功能上以及迁移旧的功能。如无必要，不做完整的重写或者重构。
使用 webpack 创建优化后的代码包。

**产出**

整个代码库和代码结构体系中的统一的样式指南变得更加容易维护。
极大改善了时间消耗以及编码效率。
因为能够实现更复杂的功能，改善了用户体验，从而导致了更好的销售业绩。
通过减少包的体积使页面的加载时间得到改善。

#### 挑战

经过六年的市场推广，GitLab 已经成为上千家公司开发人员心目中知名的解决方案提供商。但是在两年前，公司内部的大部分代码仍然是用 Rails 和 jQuery 编写的。

直到 2015 年，公司还没有专职前端的开发人员，而且整个体系运转得十分良好。Rails 开发人员兼职写前端代码而且做的很棒。然而，公司未来的计划需要一个新的解决方案。

> 当我刚进公司的时候，我看到我们有一些比较简单的项目是只用 jQuery 实现的。但如果我们想要做一些更复杂的东西，或者说我们想要实现一些比较大的点子，我们需要一些别的东西。Jacob 解释道，

![](https://ooo.0o0.ooo/2017/11/03/59fc19771d8ba.png)

> jQuery 很棒，但是因为你要负责代码内的每一个状态的变化，这样容易导致它造成更多的 bug。

为了达成目标，GitLab 开始寻找一个新的解决方案。

> 因为我之前有使用 Backbone 的经验，所以我们考虑过它。我们也仔细考虑过 React，但是也淘汰了。还有 Embar 和其他的不同的框架。我甚至想过用每个框架都做一个小项目出来，那时候我们甚至还没想过 Vue.js！Jacob 回忆道。

测试所有的这些框架帮助 Jacob 认识到了它们的优缺点。

> Backbone 有很好的结构，它有很多小工具可以完成任务。但是你用起来其实和 jQuery 没什么太大区别。而我对使用 React 这种依赖大公司的框架有些恐惧，因此它似乎也不适合我。我非常喜欢 Mithril！唯一的问题是它写起来非常困难。如果他们能加入一些友好性， 我相信人们会开始适应它。

另外一个大的挑战就是为切换新技术做个成熟的方案。这么做有很大的风险，因此必须良好地切换它。

> 在 GitLab，我们有成吨的代码。当我加入的时候，我们的代码库已经有 8000 行的 JavaScript代码了。很明显，我完全不想去彻底重写这玩意。实际上我们的代码库中还是有些地方是用 jQuery 写的。

#### 解决方案

测试了一些框架之后，Jacob 在他手头的框架里还是找不到一个完美匹配的。只有在他用 Vue.js 的早期版本写了一个很大的项目之后，他才意识到自己可能找到黄金了。

> 当我把这个项目放在一起的时候，我就知道我们可以用这个框架写很多代码。这不仅仅是写一个简单的 todo 应用。所有问题都会在你开始处理这个大型的应用的时候真正开始，Jacob 解释道。

在 GitLab 开始切换到 Vue.js 之前，他们需要做一次概念验证。

> Phil Hughes [Sr. GitLab 前端工程师],创建一个概念验证，我们在那里采取了一个我们正在做的主要功能 —— issue boards 。Phil 用 Vue.js 写这个，显而易见，我们在很短的时间内完成了大量的工作！没有之前 jQuery 带来的各种 bug。Jacob 说道。

![](https://ooo.0o0.ooo/2017/11/03/59fc19cb934bd.png)

Vue.js 支持 Jacob 在他的团队中推广自己的方法--小范围迭代，并建立概念验证。

> 他说，我们总是有四到五个概念验证。

通过这种方法, GitLab 引入了 webpack ，它能够将资源拆分成更小的块供浏览器下载，从而缩短了应用的加载时间。

> 我们创建了一个小的概念验证来判断 webpack 是否可行，当我们发现这是可行的时候，我们走完了整个流程并结束了 Vue 和整个 trello 应用的开发。并在一个月内取代了数十亿美元的产业，干得好，Phil！Jacob 笑了。

响应式模板（reactive templates）这个功能是 Vue.js 中最有用的。

> 这是 Vue 所做的非常非常简单的一件事情。 我在 GitLab 中编程的第一件事就是进入 issue 页面，在之前，当你点击 close 的时候，你必须刷新页面。 而现再，它改变了合并按钮（merge button）的状态，它会自动改变下面所有按钮的状态。在 jQuery 中，我们需要写至少三四十行的代码来保证这个按钮的状态是正确的。在 Vue.js 中只需要一行代码。视图总是会反映出当前的情况， Jacob 解释道。

> 而且现在我们使用 Vuex，它比之前做的更好。状态管理工作有了很大的不同

虽然 Vue 有很多优点，但是它也有一个缺点。

> 目前 GitLab 有 15 名开发者。像 Angular 这样的框架，大家可以在一起用同样的方式工作。而 Vue 比它开放很多，所以我们需要建立文档来告诉大家在 Vue.js 中写代码时该遵循什么样的模式。不过这是我们已经解决了的问题，Vue的开放性也是它的魅力所在，但是你需要保证所有人都在同一个层面上。

**[VUE.JS STYLE GUIDE BY GITLAB](https://docs.gitlab.com/ee/development/fe_guide/style_guide_js.html)

#### 产出

> 使用 jQuery 来扩展应用和引入新功能其实是可以的，不过维护起来就要困难的多。

> 我们现在正在做的事情需要非常大的代码量以及很多的组织。针对这些问题 Vue 解决了很多。Jacob 说。

> 像 Vue.js 中的响应式这种, 你给它一个变量，它会直接绑定到 DOM 上并处理好所有其他的事情，尤其是 2.0 版本中的虚拟 DOM，它提供给我们一个简化工作流程的办法去改善性能。

GitLab 之所以可以快速迭代并提高代码的可用性，这都要归功于 Vue.js。

> 在之前我们需要专注一些小的细节和代码，现在我们终于可以专注于代码可用性以及用户体验。我们可以思考更大的图景。

Vue.js 是如此的开放和易上手，GitLab 的前端开发人员每天都能够处理它。

> 和其他工具相比，Vue 不用遵循任何严格的知道规则。它是开放的，这点实在太赞了。我喜欢它现在做的一切。当然它有着你能想象到的最神奇的文档。它对于新人非常直观和友好。

Vue.js 帮助 GitLab 改善了时间和成本效益

> 大家知道事实上我们的发展速度更快了。这很容易看出来。从销售角度来看，我们正在创造的更良好的用户体验功能吸引人们使用 GitLab ，并使它成为更加令人期待的产品。人们喜欢我们用 Vue.js 开发的新功能。因为我们改善了用户体验，也间接增加了销售量。

Jacob 认为他们将来肯定会再使用 Vue.js。

> 我们都准备好了！现在我们还有其他的挑战。目前我们正在努力改进我们的流程并加快测试的速度。 Vue.js 为我们解决了如此多的问题以至于我们肯定在将来持续地使用它。

### Livestorm

Livestorm 是一种基于网络的、集成一体的在线会议解决方案。它帮助像 Workable, Pipedrive 或者 Instapage 等公司进行现场销售演示或者客户培训。

> 我们不需要花一个月时间用 React 来把所有事都安排好，Vue 让我们在一周内就可以办到。我完全确信如果没有 Vue ，就不会有今天的我们。
> 
> 来自 Livestorm 的联合创始人兼首席执行官 Gilles Bertaux.

**挑战**

从零开始建立可靠的实时网络软件，并使其在竞争激烈的市场中产生影响。
在巴黎，只有极少数的 Vue.js 专家。
吸引初始用户并验证产品的理念。

**解决方案**

建立一个快速的最优秀应用。
使用 Vue.js 和 Ruby 创建一个高性能的应用。
在 Vue.js 社区上为团队寻找潜在的员工。

**成果**

立即得到用户的积极反馈。
可重用的组件以及快速开发。
快速成长的业务量以及每月 20-30% 的收入增长。

#### 挑战

与其他网络平台不同，Livestorm 渲染了浏览器中的一切。该服务通过分析、与流行的客户关系管理系统集成、以及营销自动化软件提供可实施的办法。

对于这样的应用，Gilles 和他的团队必须选择一个高性能的技术栈。他们打算从零开始验证他们的想法并建立一个稳定可靠的产品。

> Livestorm 的主干是一个 Rails 应用程序——后端所有东西都是用 Ruby 做的。 Gilles 解释道：对于我们所有的前端组件，我们选择了 Vue.js。

> 我们从 2016 年 1 月开始开发我们的项目，从第一天开始，我们就知道我们会使用 Vue。我们需要一些完全开源的、高性能的、有特定逻辑的组件。Vue 是唯一能满足我们所有需求的框架。

![1509695413(1).jpg](https://ooo.0o0.ooo/2017/11/03/59fc1fc911d6a.jpg)

Livestorm 由四位联合创始人创建，力图从公司的最初阶段组建一支强大的员工队伍。

> 我们考虑了很多招聘问题。在我们工作的巴黎地区只有很少的 Vue.js 开发人员。我们也考虑招聘精通类似于 Vue 的其他框架的开发人员，但是这种情况下，新员工培训过程可能花更长时间，这对我们来说是有问题的。

为了建立一个成功的流媒体产品，团队必须关注可靠性。

> 可靠性对我们来说是头等大事。Gilles 说：如果你失去了直播流，网络研讨会和演示会崩溃并且流媒体丢失，我们的业务就会变得毫无意义。

> 如果应用程序挂了，或者有一个 bug 让它无法使用，我们会失去用户。我们需要一种技术来保证最高的代码质量，并且运行得很快。我们仍然在执行端到端单元测试。有些事情我们还没有用 Vue 实现，这对我们来说是全新的。

#### 解决方案

大多数开发人员仍然选择 React 和其他流行的框架，但是 Gilles 相信这将会有所改变。

> 为了给我们的员工招聘专家，我们参加了在巴黎的 Vue.js 聚会，在那里我们遇到了很有经验的人。我们也试了在招聘网站上发布招聘，有趣的是，约谈的大多数程序员说他们在自己的项目上用 Vue.js，但是他们平日工作用的基本是 Angular、React，和其他框架。Gilles 指出，他们大多数来自大公司。

> 然而，我注意到一件事，那些经常使用这些技术的公司，是因为代码遗留所迫，或者是因为他们想尝试一下其他人也在尝试的技术新热点。在创业社区，在我参加的多个轻松的渠道和会面中，与我交谈的首席技术官和联合创始人对迁移到 Vue.js 很感兴趣，他们对我们在 Livestorm 里用了 Vue 很兴奋并且问了很多问题。坦率地说，我相信会有一个重大的转变——人们会对迁移到可靠、高效的东西更感兴趣，像 Vue.js。Gilles 补充说：而像 React 这类炒作的技术会逐步减少流行，直到他们最后被淘汰。

Gilles 想把他的产品尽快发布，他的团队创建了一个快速的 MVP 来获得外部世界的最初反馈。

![](https://ooo.0o0.ooo/2017/11/03/59fc226671fba.png)

> 我们花了不到一个月的时间创建了第一个 MVP。这足以展示产品和基本理念。他回忆说：最后，我们得到了很多积极的反馈，从而确保了我们是符合市场需求的。

> 我们花了 5 个月的时间卖出了第一份订阅。这是相当长的一段时间，但是我们需要首先完成一些与技术没有必然联系的东西。

Gilles 的团队在他们的平台上创建的一系列功能使其成为一个有竞争力的解决方案，真是令人惊叹。

> 直播会议、网络摄像头和屏幕共享中的 WebRTC 实时流、全高清流媒体直播是主要的视频相关的功能。我们也提供了一个运行于 Vue.js 的聚焦于分析的部分，并且与流行的销售和营销工具，例如 Salesforce 集成。我们也开发了其他基于浏览器的网络会议软件所没有的独一无二的功能，让用户可以在飞机上从 WebRTC 切换到 HLS，使媒体流可以与 IE 浏览器用户以及一部分移动设备匹配。

#### 成果

投入市场一年后，Livestorm 拥有来自世界各地的用户，并且有了一个已经盈利的产品。

> 我们已经有大约 150 名付费用户，他们都对 Livestorm 的速度之快印象深刻，他们也喜欢界面和交互。从商业上来说，我们有一个不受我们干扰能独立运行的应用程序，所以说——我们没有一个销售团队。我们有 7 名员工，包括产品专家、工程师，以及一名营销人员。那个人是我，Gilles 解释道：但是只是因为产品非常好而且可靠，我们每个月有 20%-30% 的增长。

借助 Vue.js ，Livestorm 可以更快地发布新功能，以满足客户的需求。

>  当然，我们试图尽快地上新功能。现在我们在一个为期两个月的开发阶段，该阶段将以一个大型功能的发布而结束，但是我们通常在一两周内发布功能，Gilles 解释道。

> 有了 Vue.js 我们不必每次都去造轮子。

> 我们可以重用所有已有的组件来加快开发。现在，我们代码库的 39.5% 是用 Vue 创建的。

![](https://ooo.0o0.ooo/2017/11/03/59fc22c98b5f1.png)

Gilles 声称选择 Vue.js 而不是其他框架让他的公司成功得更快。

> 只有基准说明了真相，而现在基准清楚地证明了 Vue.js 绝对是新产品和现有产品的选择。他说：所以如果任何人在不久的将来必须做出技术选择，他们应该依靠具体事实、数据和基准，而不是观点。

> 如果你有很多开发人员，他们已经习惯了使用 Angular 或者是更加经典的框架，让他们迁移到 React 会使整个团队感到痛苦。另一方面，过渡到 Vue，更加顺畅，反过来只要更低的成本。 我们不需要像 React 花一个月的时间来把所有事都建立好。Vue 让我们在一周内开始运作。如果不是 Vue，我 100% 地肯定我们永远不会达到现在这样的成就。

### Vue.js 的特点

来自 Vue.js 的作者 Evan You

#### 可持续性

作为一个项目，Vue.js 已经走了很长的路才能成为今天的样子。它已经从一个小的实验成长为一个成熟的框架，并且被全世界成千上万的开发者使用。它已经从一个“项目”发展成一个生态系统，在 vuejs 组织中有超过 300 个贡献者，并由来自全球的超过 20 个活跃成员组成的核心团队维护。核心团队成员承担了核心库的维护、文档、社区参与以及主要的新特性例如类型声明的改进和测试功能。说 Vue 是“一个人的项目”不再准确，也是对团队和社区的所有惊人贡献的不尊重。

从财政上来说，从 2016 年 2 月来，Patreon 活动已经收到了稳定的有保障的收入，这让我可以在过去一年半时间里全职工作在这个项目里。另外，最近开始的 OpenCollective 活动，旨在为社区举措提供财政支持，在短短两周里已经收到超过 11000 美元的年预算，而且还在持续增长。更重要的是，这些开放的财政贡献渠道意味着你的公司可以通过成为赞助商积极帮助确保项目的可持续性。

今天我有信心地说作为一个开源项目，Vue.js 已经超越了这一临界点，即项目的生存对任何考虑是否采用该项目的人来说不再是一个问题。

#### 稳定性 

前端的设计变化很快，我们知道不断改变有多么令人沮丧。这是为什么我们这么重视稳定性。在 GitHub 上查看项目的历史，你会看到一系列新特性和改进的版本的坚实记录，及时的 bug 修复，以及对代码一丝不苟的标准（是的，我们保证 100% 测试覆盖率）。

所有 Vue.js 包的发布遵循了语义版本控制，我们尽最大努力通过交流提前知道任何潜在的需要的操作。2015 年 10 月，1.0 版本发布了，并没有在公共接口中有所突破，直到一年后 2.0 版本的发布。在 2.0 发布之前，我们进行了公开设计讨论，并发布了多个 alpha/beta/RC 版本来确保最终版本的稳定性。我们尽力保持接口与 1.0 相似，并提供全面的指导和升级工具。今天，2.0 已经发布了一年多了，在全球的产品内得到广泛应用，我们不认为在可预见的将来需要对主要的接口做修改。我们致力于在对用户最小影响下改进框架。

#### 连续改进 

当然，我们不会只满足于当前我们已经做的事情。
我们在未来几年的探索和实施的计划中有很多想法，我会将它们分为三类：

##### 近期的改进

这些新特性/改进将会持续发布于 2.x 小版本中，它们可以来自特性需求、来自更广网络开发社区的灵感，以及我们在实际开发中遇到的用例。

##### 中期的改进

有新的 JavaScript 语言特性（比如 ES2015 代理，Promises）可以简化或改进当前的接口，但是因为必须要支持 IE9，现在还不适合放在主分支上，我们计划在并行分支中开始利用这些特性，而这需要最新的主流浏览器支持。

##### 长期的改进

我们还关注新兴的标准，比如 ES 类语法改进（类变量和装饰器），网络组件（自定义元素和 HTML 模块）以及 WebAssembly。我们已经开始了其中一些实验，并且一定会利用它们来进一步改进 Vue 的开发经验和性能，因为它们在浏览器适应方面已经成熟。

#### 长期愿景

很多人问我为什么开始使用 vue.js。老实说，一开始目的是为了“给自己挠痒痒”，创建一个我自己喜欢用的前端库。在这个过程中，随着 Vue 被越来越多的用户接受，我收到了很多来自用户的消息说 Vue 使他们的工作变得越来越令人愉快，因此看上去我的偏好与很多网络开发者朋友们不谋而合。今天，我设想 Vue 的目的变为用来帮助更多开发人员喜欢在网络上创建应用程序。我相信更快乐的开发人员会更加高产，并且最终为每个人创造很多价值。目标需要提供一个可获得的、直观的、同时可靠、强大并且可扩展的框架。我相信我们正处于正轨上，但我们也可以做更多的事情，特别是通过 Web 平台得到比以往更快的发展。

我们为即将到来的事情感到兴奋。

© Monterail, October 2017

Monterail 是一个由 80 多个专家组成的紧密团队
为创业公司和企业提供网络和移动开发。
并且我们喜欢 Vue。

[http://www.monterail.com](http://www.monterail.com)
[hello@monterail.com](mailto:hello@monterail.com)

---

> [掘金翻译计划](https://github.com/xitu/gold-miner) 是一个翻译优质互联网技术文章的社区，文章来源为 [掘金](https://juejin.im) 上的英文分享文章。内容覆盖 [Android](https://github.com/xitu/gold-miner#android)、[iOS](https://github.com/xitu/gold-miner#ios)、[React](https://github.com/xitu/gold-miner#react)、[前端](https://github.com/xitu/gold-miner#前端)、[后端](https://github.com/xitu/gold-miner#后端)、[产品](https://github.com/xitu/gold-miner#产品)、[设计](https://github.com/xitu/gold-miner#设计) 等领域，想要查看更多优质译文请持续关注 [掘金翻译计划](https://github.com/xitu/gold-miner)、[官方微博](http://weibo.com/juejinfanyi)、[知乎专栏](https://zhuanlan.zhihu.com/juejinfanyi)。
