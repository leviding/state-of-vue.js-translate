### Chess.com

Chess.com is the #1 destination for online chess. Every day more than a million games are played by chess players from all around the world and all skill levels. Chess.com is a fully remote team with 100 team members.

Chess.com 是排名第一的在线国际象棋网站。来自全世界各个地方各个段位的棋手每天要对弈超过 100 万局。Chess.com 是由 100 位成员组成的完全远程的团队。

> It was the first time I’ve read the entire documentation in one sitting. It was 1:30am in the morning. By the time I got to the end of it, I knew that Vue. js was something special. There was something unique about it. Something I’d never seen before.
>
> From Scott O’Brien, Lead UX Engineer at Chess.com.

> 这是我第一次一口气阅读完整的文档。现在是早上 1:30。当我看完时，我知道了 Vue.js 是个特别的东西。它有一些独特之处。一些我从来没有见过的东西。
>
> Scott O’Brien，Chess.com 首席用户体验工程师

**CHALLENGE**

**挑战**

Dealing with hard-to-maintain legacy code in Angular 1.
Introducing new features to increase user engagement.
Managing change in a fully distributed development team.

处理难以维护的 Angular 1 遗留代码。

引入新特性以增加用户参与度。

在一个完全分布式的开发团队中管理变更。

**SOLUTION**

**解决办法**

Benchmarking all available frameworks.
Moving from Angular 1 to Vue.js.
Architecting a growing library of components, each with its modular CSS.

对所有可用的框架进行基准测试。

从 Angular 1 迁移到 Vue.js。

构建日益增长的组件库（连同它的模块化 CSS）。


**OUTCOME**

**成果**

Ease of collaboration with a fully remote team.
More effective way to write CSS inside the app.
Scaling up efficiently in terms of speed, power, and abstraction when compared to other frameworks.

使得全远程的团队合作更加愉悦。

app 内编写 CSS 更加高效。

与其他框架相比，在速度、能力和抽象方面更有效地进行扩展。

#### Challenge

#### 挑战

Chess.com is the most frequently visited website about chess with a great social network with over 19 million members. It has news, blogs, community, lessons, puzzles, and of course real-time gaming. The complexity of the portal may be overwhelming.

Chess.com 是国际象棋领域中访问频率最高的网站，拥有多达 1900 万成员庞大的社交网络。它有新闻，博客，社区，教程，谜局，当然也包括实时对弈。网站门户的复杂性是巨大的。

Its legacy code was in PHP and Angular 1. At any given moment, Chess.com is hosting tens of thousands of games in real time on the Web and mobile devices. For such a website, performance is everything.

遗留代码是用 PHP 和 Angular 1 编写的。任何时刻，Chess.com 都承载着网页上或手机上成千上万的实时对战游戏。对于这样一个网站来说，性能是第一位的。

> We got to the point where the old way of doing things with Angular 1 was a huge performance bear. It was just getting bigger and bigger. Some parts of our website became unusable on legacy hardware from a performance perspective. It was unmaintainable, Scott recals.

> 我们已经知道使用 Angular 1 是一个巨大的性能瓶颈。它只会变得越来越大。从性能角度来看，我们网站的有些部分在一些遗留的硬件设备上已经变得无法使用。它是无法维护的，Scott 回忆说。


The challenge that Chess.com was facing was not only dealing with existing features, but also planning for future ones.

Chess.com 面临的挑战不仅是处理现有的功能，也包括对新功能的规划

![](https://ooo.0o0.ooo/2017/11/03/59fc0a031aef2.jpg)

> A lot of the discussion was about architecture because we knew we had a bunch of new features we are trying to add to keep people engaged to play more chess and try different ways of playing chess, Scott explains.

> 大部分讨论都是关于架构，因为我们知道需要加入很多新的功能以保证用户下更多的棋并尝试各种不同的下棋方式，Scott 解释说。

> I wouldn’t say it was out of reach with Angular, but it was very tough to do it well in terms of performance with those legacy javascript frameworks.

> 我不是说用 Angular 就做不了，只是用这些过时的 javascript 框架很难做到。

To improve the user experience, Chess.com required some real changes.

为了提高用户体验， Chess.com 需要做一些真正的改变。

> We knew we needed to take a leap. There was significant delibera- tion over which framework we wanted to move to from Angular 1. Of course, we considered the big players—Angular 2 and React.

> 我知道我们需要一个质的飞跃。对于从 Angular 1 迁移到哪个框架我们深思熟虑。当然，我们有考虑过两位大佬：Angular 2 和 React。

The massive infrastructure and ongoing product development requires a well-organized and quite big-sized team.

庞大的基础设施和持续的产品开发需要一个组织良好且规模庞大的团队。

> We have a collection of very different skillsets within our development team. Moreover, the team is fully distributed and international—we are all over the map. Any decision as big as leaping to another technology brings a lot of concerns.

> 在我们的开发团队中，有非常不同的技术栈。此外，我们的团队是完全分布式和国际化的。任何像技术迁移一样重要的决定都会引起很多人的关注。

#### Solution
#### 解决办法

Choosing a framework backed by Facebook or Google, such as React or Angular, respectively, seemed to be a safer choice. Yet, the Vue.js community proved that the newcomer framework is definitely a contender.

选择一个由 Facebook 或 Google 支持的框架，如 React 或 Angular，相对来说，貌似是一个比较安全的选择。但是，Vue.js 社区证明这个新来者无疑是一个强力的竞争者。

> We were so performance-centric that we would probably go with a less developer-friendly framework if the benchmarks looked good. Seeing Vue.js win the rendering and performance benchmarks was mind-blowing, Scott explains.

> 我们是如此的关心性能以至于我们可能会选择对开发者不那么友好但基准测试看上去不错的框架。看到 Vue.js 赢得了渲染和性能的基准测试是振奋人心的，Scott 解释到。

> We were concerned that the entirety of Vue.js was built on Evan’s ideas and that the framework would live or die with him. We decided that as long as the community was rapidly growing and we believe they are doing something revolutionary, we wanted to take the leap and believe that other people will see the value in the future that we see now. So the big concern was if it’s going to continue to grow and I think that has been proven by now.”

> 我们担心的是整个 Vue.js 是建立在 Evan 的想法上的，这个框架的生死都由他主导。我们决定只要社区发展迅速并且我们相信他们在做一些革命性的事情，我们就会带头并确信其他人在将来会看到它的价值，正如我们现在看到的一样。所以最大的问题是，它是否会继续发展，我认为这已经被证实了。

One of the first things that Chess.com team had to work on was rewriting different pages from AngularJS to Vue.

Chess.com 团队首先要做的事情之一就是重写不同的从 AngularJS 到 Vue 的页面。

> The process of rewriting is still going on today. It has been happen- ing for months at this point. The other mission that we had was essentially building our internal collection of reusable components, Scott points out.

> 重写工作现在仍在进行，目前已经持续了数月。我们的另一个任务是构建我们内部的可重用组件集，Scott 指出。

![](https://ooo.0o0.ooo/2017/11/03/59fc0a6a4a369.jpg)

> I think it’s the most impressive thing we have been using Vue for— architecting a growing library of components, each with its own modular CSS, which will eventually comprise the entirety of user interface elements on our site. While one team has been using Vue to implement components, routes, and stores for particular product domains, another team has been working on our component library to be shared throughout the site with little to no concern for collision. Additionally, it has infused our product discussions with a greater sense of abstraction and reuse.

> 我认为用 Vue 构建一个不断增长的组件库是一件非常酷的事情，每个组件都有自己的模块化 CSS，这些组件最终会构成我们网站上的全部用户界面元素。一个团队一直在用 Vue 来实现特定产品领域的组件，路由和存储，而另一个团队一直致力于构建全站共享的组件库，几乎不用担心产生冲突。此外，它还使我们的产品讨论更加抽象和复用。

#### Outcome
#### 成果

For a big app like Chess.com, one thing about Vue brings more benefits than the rest.
对于一个像 Chess.com 这么大的应用来说，Vue 带来的好处远远超过其他。

> Single File Components was an absolute game changer for structuring and maintaining our repository. Being able to just buy in to the official pieces of the framework having an official state management system. We’re having confidence that these things are going to work together—it’s all part of the collective vision.”

> 单个文件组件绝对是构建和维护我们库的不二法则。Being able to just buy in to the official pieces of the framework having an official state management system.（这个不会翻呀，哪位帮帮我）我们相信这些事情会一起工作——这都是集体愿景的一部分。

With Vue.js in place, Scott finds it easier to collaborate with his remote team.

有了 Vue.js，Scott 发现与远程团队合作起来更加容易了。

> What we love about Vue is that it has an incredible ease of use and a low barrier to entry while simultaneously having the ability to scale up with comparable (if not better) power, speed, and abstrac- tion to other component libraries, he points out.

> 他指出，我们对Vue的热爱在于，它具有难以置信的易用性和低的入门门槛，同时具备拓展能力，与其他组件库相比，有相当的(如果不是更好)能力、速度和抽象性。

> We’re a fully remote team of 15 developers and we rely heav- ily on Slack, Jira, and GitHub. However, it’s actually easier to collaborate in Vue, because it’s not so different from our legacy code—there’s still declarative templating and everything that we are used to.

> 我们是一个完全由15个开发人员组成的远程团队，我们非常依赖 Slack, Jira 和 GitHub。然而，在 Vue 中更容易进行协作，因为它与我们的遗留代码没有太大的区别——仍然有声明式模板以及我们习惯的所有内容。

> Secondly, the ease of writing CSS now is amazing. It made such a tremendous benefit for us. We have many developers speaking different languages with different coding styles. Coming up with the names relevant only for markup in a particular file without worrying about the global namespace. The ease of use is just wonderful.

> 其次，编写 CSS 的便捷性令人惊叹。它给我们带来了巨大的利益。我们有许多开发人员说着不同的语言使用不同的编程风格，他们只需针对特定文件中的标记来命名，而不需要担心全局名称空间的名称冲突。使用方便的感觉是如此美妙。

As Vue has lent great support to the Chess.com team, they will definitely continue working with it in the future.

介于 Vue 给 Chess.com 团队提供了巨大的支持，未来他们无疑将会继续使用它。

> We’re all in with Vue.js right now! As I said, right now our process is twofold: essentially re-architecting our components and moving from Angular 1. Therefore, we’re implementing it two totally separate ways simultaneously. That’s elating.

> 我们现在都在用 Vue.js！正如我说的，我们的工作分两部分：重构我们的组件，从 Angular 1 迁移。因此，我们同时用两种完全不同的方式实现，这是值得骄傲的。

![1509690042(1).jpg](https://ooo.0o0.ooo/2017/11/03/59fc0ac62efa9.jpg)

### Clemenger BBDO
### Clemenger BBDO

Clemenger BBDO is a full service agency offer- ing a full suite of capabilities including brand strategy, integrated creative development, CX, digital services, CRM, PR, design, shopper and activation.

Clemenger BBDO 是一个全方位的服务机构，提供包括品牌战略、综合创意开发、CX、数字服务、CRM、PR、设计、顾客和激活的全套功能

In the last 12 months the agency has been named World’s most creative agency at Cannes Lions and D&AD.

在过去的12个月里，在戛纳广告奖和创意奖上，它被评为世界上最具创意的机构。

We decided to pick Vue.js be- cause it was answering all the requirements we had to cover for our projects, while offering a comfortable development environment for our team. It’s so close to native JavaScript, that it’s extremely easy to start working with it.

我们决定选择 Vue.js 因为它满足了我们的项目提出的所有需求，同时为我们的团队提供了一个舒适的开发环境。它非常接近于原生 JavaScript，因此很容易使用它。

> From Sylvain Simao, Technical Lead at Clemenger BBDO Melbourne.

> Sylvain Simao, Clemenger BBDO 技术总监，墨尔本

**CHALLENGE**

**挑战**

Projects with short lifespans (4 to 12 weeks) done by different people.
Working with animations and transitions.
Need to load and work fast on mobile devices.

项目周期短（4 到 12 周），由不同的人开发。

使用动画和过渡效果。

移动设备上加载和运行速度要快。

**SOLUTION**
**解决方案**

Using Vue.js with a pre-render solution for static pages.
Building ES6 modules rather than framework specific code.

对静态页面使用 Vue.js 的预加载方案

构建ES6模块而不是框架特定的代码。

**OUTCOME**
**成果**

Delivered several successful interactive campaign experiences. within strict deadlines.
Digital projects ready for high traffic volumes.
Quick onboarding and project setup.

按时交付多个成功的互动活动。

高流量的数字项目。

快捷的入职培训和项目初始化。


#### Challenge
#### 挑战

Most of the projects Clemenger BBDO works on are campaign websites. It’s mostly frontend with a little backend magic—most projects use the serverless approach, API, AWS services, and the like.

Clemenger BBDO 大多数项目是网站设计。他们大部分是前端的（包含小部分后端），大多数项目使用的是无服务器的方式、API、AWS 服务等。

Working on different projects simultaneously under strict deadlines, Clemenger BBDO had to devise a standardized solution that would significantly ncrease development speed and be flexible enough to workacross very different experiences.

由于同时需要开展多个有着严格工期的项目，Clemenger BBDO 必须设计出一套标准的可以显著提高开发速度，且要有足够的灵活性，可以用于不同的项目之中的方案。

> As technical lead, one of the main things I need to keep in min is the ability of my team to deliver high-end, quality projects within short time frames. We are an advertising agency, which means that a 3-month-long project is a really long one, Sylvain explains.

> 作为技术领导，我需要记住的一件事情是我的团队在短时间内交付高端的高质量项目的能力。我们是一家广告公司，这意味着一个为期3个月的项目真的很长，Sylvain 解释道。

> A fast-paced environment means that we need people to be able to jump quickly into new tools. Sometimes we also need to work with external contractors, so the perfect solution for us was something easy to learn and start working with. Vue gives us a lot of flexibility in terms of workflow—for example being able to work with already known preprocessors for HTML and CSS is a big plus.

> 快节奏的环境意味着我们需要人们能够快速地投入到新的工具。有时我们也需要与外部承包商合作，所以对于我们最完美的方案是那些很容易学习和用于工作的东西。Vue在工作流程方面给了我们很大的灵活性——例如，能够与已经知道的 HTML 和 CSS 的预处理器一起工作是一个很大的优势。

On client projects, Sylvain and his team worked with a variety of different JavaScript frameworks.

> I feel like we’ve tried all of them! Sylvain laughs.

> 我觉得我们都试过了! Sylvain 笑道。

> We’ve tried frameworks like Angular, React, and Riot.js, but Vue is the one we fell in love with. Vue offers simplicity and robustness at the same time. For us it’s a breath of fresh air among the others. It has a rich ecosystem out of the box, and the fact that it’s incrementally adoptable makes it the perfect tool for the type of work we have to deliver on.

> 我们尝试了一些框架，比如 Angular，React，和 Riot.js。但是 Vue 最终得到了我们的青睐。Vue 即简单又不失健壮。对我们来说，这是一缕新鲜的空气。它有一个丰富的生态系统，而且它是一个渐进的可采用的工具，使它成为我们所要交付的工作类型的完美工具。

Interactive campaign websites are challenging in many ways.

交互式网站设计到处是挑战。

> You have to deal with SEO, accessibility, and extended browser support—but also deliver on animations, transitions, and very interactive interfaces in general. Combining those is definitely the most challenging aspect of our work.

> 您必须处理 SEO、可访问性和浏览器兼容性，但同时也要实现一般的动画、转换和很多交互界面。这些无疑是我们工作中最具挑战性的方面。

#### Solution
#### 解决方案

Due to its smooth learning curve, Vue.js makes it easy to work with new developers or external contractors.

由于其流畅的学习曲线，Vue.js 可以很容易让新开发人员或外部承包商使用。

> We’ve noticed that Vue.js is great in terms of onboarding new people. Why? The learning curve is really smooth and it’s really close to vanilla JavaScript, Sylvain claims.

> 我们注意到 Vue.js 在培训新手方面表现很不错。为什么？因为学习曲线非常平滑，非常接近原生 JavaScript，Sylvain 说。

> For us, as a business, it’s really awesome. People get up-to-speed really quickly and we can deliver more efficiently. One other remarkable point is the incredible quality of the official documentation and resources available for Vue. It probably deserves an award for the most comprehensible framework documentation!

> 对我们企业来说，它真的很棒。人们可以很快获得最新的速度，我们可以更有效率地交付。另一个值得注意的一点是，Vue 的官方文档和资源的质量令人难以置信。它可能应该得到一个最容易理解的框架文档奖!

For every website Clemenger works on, it’s important to make it visible for bots for successful SEO.

对于每一个 Clemenger 服务的网站来说，重要的是 SEO。

> For that specific problem we do pre-rendering for all our pages. Most of the time, when we have a new project that requires Vue.js, we start from a boilerplate that we’ve built on top of the official Vue webpack template. Then, we use libraries like PhantomJS or Prep to render static snapshots of the pages. The last step consists of serving those pages to robots, which can easily be achieved by targeting the user agent with Nginx or Lambda@Edge, Sylvain elaborates.

> 对于这个特定的问题，我们为我们的所有页面做预渲染。大多数时候，当我们有一个新的项目需要 Vue.js 的时候，我们从基于官方 Vue webpack 模板构建的样板开始。然后，我们使用像 PhantomJS 或 Prep 这样的库来呈现页面的静态快照。最后，通过使用 Nginx 或 Lambda@Edge 等用户代理工具，很容易将这些页面提供给爬虫。

Sylvain uses Vue.js to deal with animations and transitions.

Sylvain 使用 Vue.js 来处理动画和渐变效果。

> Right now we are changing our way of approaching animations. Since the release of Vue’s most recent version, there is now a lot more flexibility with the transitions. We now have a more granular access to the transition hooks, that makes it possible to trigger third-party libraries and deliver on complex animations, while still using Vue at the core. I’m trying to push my team to move to that model.

> 现在我们正在改变我们实现动画的方式。自从 Vue 的最新版本发布以来，现在的渐变效果有了更多的灵活性。我们现在有了一个更细粒度的转换钩子，这使得可以触发第三方库并实现复杂的动画，同时核心仍使用 Vue。我正努力推动我的团队走向那种模式。

For Airbnb’s campaign website—“Until we all belong”—Vue.js was the technology of choice.

对于 Airbnb 的活动设计--“Until we all belong”，技术选型是 Vue.js。

![1509690301(1).jpg](https://ooo.0o0.ooo/2017/11/03/59fc0bc9c12ea.jpg)

> The project is designed as a single page application, based on Vue and webpack at the start. For better efficiency, the web views were hosted in Amazon S3 buckets, which means that we couldn’t use any server-side rendering. Every part of the UI and every page have been built using Vue single file components. In this kind of website, where we are anticipating major traffic, performance is key, and that’s why everything is loaded on-demand. In one of our projects we were recording 6,000 visitors per minute—it was a big buzz. We need to be ready for that, Sylvain explains.

> 该项目最初设计为一个单页面应用，基于 Vue 和 webpack。为了提高效率，web 页面托管在 Amazon S3 bucket 中，这意味着我们不能使用任何服务器端渲染。UI 的每个部分和每个页面都是使用 Vue 单个文件组件构建的。在这样一个预期会有大流量的网站上，性能是关键，这就是为什么所有东西都按需加载。我们的一个项目记录到了每分钟 6000 个的访问量——相当大了。我们需要做好准备，Sylvain 解释道。

> Vue.js can be a lifesaver in such cases. For the Airbnb project there were big image assets in the background that we needed to load and animate. For that purpose, we’ve used Vue-router to declaratively list assets or data that required pre-loading, and VueX to keep track of those on every page. The project was also challenging in term of interactions, but we’ve managed to deliver the website within 6 weeks.

> 在这种情况下，Vue.js 是救星。对于 Airbnb 项目，背景中有很大的图片资源需要加载以及应用动画。为此，我们使用 Vue-router 来声明需要预加载的资源或数据，而 VueX 则负责跟踪每一页上的内容。这个项目在交互方面也很有挑战性，但我们在6周内就成功推出了这个网站。

![1509690342(1).jpg](https://ooo.0o0.ooo/2017/11/03/59fc0bf296b5a.jpg)

#### Outcome
#### 成果

Delivering projects in a timely manner is much easier with Vue.js.
使用 Vue.js 来按时交付项目要容易得多。


> We wouldn’t be as fast if it wasn’t for Vue. Mostly because of the simplicity of the API. We’ve recently worked on a prototype for a hybrid app built on Angular 2, the syntax is elegant but the learning curve is steep and doing simple things takes time. With Vue you can prototype really quickly and that’s probably its greatest strength.

> 如果不是 Vue，我们就不会那么快了。主要是因为 API 的简单性。我们最近开发了一个基于 Angular 2 的混合应用程序的原型，语法很优雅，但学习曲线很陡峭，简单的事情也需要时间。有了 Vue，你可以快速地实现原型，这可能是它最大的优势。

With Vue.js, the Clemenger team is able to tackle a wide range of different projects

有了 Vue，Clemenger 团队能够处理各种不同的项目。

> We now have quite a few projects built upon Vue.js. Airbnb’s Until we all belong, a campaign for marriage equality in Australia, was recognized with a number of industry awards, including AWWWARDS and CSSDA. Another project—Meet Graham which introduce the only person designed to survive on our roads, Graham. Within the first week, the project recorded more than 10 millions page views and it got immersive recognition and media coverage. It was highly acclaimed and received numerous awards, including the Grand Prix at Cannes Lion 2017. One of our most recent project is Snickers Hungerithm, where we’ve decided to rewrite the campaign app using Vue.js for the global rollout. Hungerithm is a hunger-algorithm that monitors online mood using tweets. When anger goes up, Snickers prices goes down in real-time.

> 我们现在有相当多的项目建立在 Vue.js 之上。“Airbnb’s Until we all belong”，一个澳大利亚的婚姻平等活动，已经获得了一些行业奖项，包括 AWWWARDS 和 CSSDA。另一个项目--Meet Graham which introduce the only person designed to survive on our roads, Graham。在第一周内，该项目记录了超过 1000 万的页面浏览量，并获得了身临其境的公认和媒体报道。它备受好评，并获得了众多奖项，包括 2017 年戛纳国际电影节大奖。我们最近的一个项目是 Snickers Hungerithm，这次我们决定用 Vue 重写活动应用用于全球推广。Hungerithm 是饥饿识别算法，可以通过 tweet 来监控在线情绪。当饥饿度上升时，士力架的价格就会实时下降。
