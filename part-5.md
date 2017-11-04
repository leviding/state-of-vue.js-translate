### Chess.com

Chess.com is the #1 destination for online chess. Every day more than a million games are played by chess players from all around the world and all skill levels. Chess.com is a fully remote team with 100 team members.

Chess.com 是排名第一的在线国际象棋网站。来自全世界各个地方各个段位的棋手每天要对弈超过 100 万局。Chess.com 是由 100 位成员组成的完全远程的团队。

> It was the first time I’ve read the entire documentation in one sitting. It was 1:30am in the morning. By the time I got to the end of it, I knew that Vue. js was something special. There was something unique about it. Something I’d never seen before.
>
> From Scott O’Brien, Lead UX Engineer at Chess.com.

> 这是我第一次一口气阅读完整的文档。现在是早上 1:30。当我看完时，我知道了 Vue.js 是个特别的东西。它有一些独特之处。一些我从来没有见过的东西。
>
> 斯科特·奥布里恩，Chess.com 首席用户体验工程师

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

> 我们已经知道使用 Angular 1 是一个巨大的性能瓶颈。它只会变得越来越大。从性能角度来看，我们网站的有些部分在一些遗留的硬件设备上已经变得无法使用。它是无法维护的，斯科特回忆说。


The challenge that Chess.com was facing was not only dealing with existing features, but also planning for future ones.

Chess.com 面临的挑战不仅是处理现有的功能，也包括对新功能的规划

![](https://ooo.0o0.ooo/2017/11/03/59fc0a031aef2.jpg)

> A lot of the discussion was about architecture because we knew we had a bunch of new features we are trying to add to keep people engaged to play more chess and try different ways of playing chess, Scott explains.

> 大部分讨论都是关于架构，因为我们知道需要加入很多新的功能以保证用户下更多的棋并尝试各种不同的下棋方式，斯科特解释说。

> I wouldn’t say it was out of reach with Angular, but it was very tough to do it well in terms of performance with those legacy javascript frameworks.

> 我不是说用 Angular 就做不了，只是用这些过时的 javascript 框架很难做到。

To improve the user experience, Chess.com required some real changes.

为了提高用户体验， Chess.com 需要做一些真正的改变。

> We knew we needed to take a leap. There was significant delibera- tion over which framework we wanted to move to from Angular 1. Of course, we considered the big players—Angular 2 and React.

> 我知道我们需要一个质的飞跃。对于从 Angular 1 迁移到哪个框架我们深思熟虑。当然，我们有考虑过两位大佬：Angular 2 和 React。

The massive infrastructure and ongoing product development requires a well-organized and quite big-sized team.

庞大的基础设施和持续的产品开发需要一个组织良好且规模庞大的团队。

> We have a collection of very different skillsets within our development team. Moreover, the team is fully distributed and international—we are all over the map. Any decision as big as leaping to another technology brings a lot of concerns.

> 在我们的开发团队中，有非常不同的技术栈。此外，我们的团队是完全分布式和国际化的。任何像技术迁移一样重要的决定都会引起很多人的关注

#### Solution

Choosing a framework backed by Facebook or Google, such as React or Angular, respectively, seemed to be a safer choice. Yet, the Vue.js community proved that the newcomer framework is definitely a contender.

> We were so performance-centric that we would probably go with a less developer-friendly framework if the benchmarks looked good. Seeing Vue.js win the rendering and performance benchmarks was mind-blowing, Scott explains.

> We were concerned that the entirety of Vue.js was built on Evan’s ideas and that the framework would live or die with him. We decided that as long as the community was rapidly growing and we believe they are doing something revolutionary, we wanted to take the leap and believe that other people will see the value in the future that we see now. So the big concern was if it’s going to continue to grow and I think that has been proven by now.”

One of the first things that Chess.com team had to work on was rewriting different pages from AngularJS to Vue.

> The process of rewriting is still going on today. It has been happen- ing for months at this point. The other mission that we had was essentially building our internal collection of reusable components, Scott points out.

![](https://ooo.0o0.ooo/2017/11/03/59fc0a6a4a369.jpg)

> I think it’s the most impressive thing we have been using Vue for— architecting a growing library of components, each with its own modular CSS, which will eventually comprise the entirety of user interface elements on our site. While one team has been using Vue to implement components, routes, and stores for particular product domains, another team has been working on our component library to be shared throughout the site with little to no concern for collision. Additionally, it has infused our product discussions with a greater sense of abstraction and reuse.

#### Outcome

For a big app like Chess.com, one thing about Vue brings more benefits than the rest.

> Single File Components was an absolute game changer for structuring and maintaining our repository. Being able to just buy in to the official pieces of the framework having an official state management system. We’re having confidence that these things are going to work together—it’s all part of the collective vision.”

With Vue.js in place, Scott finds it easier to collaborate with his remote team.

> What we love about Vue is that it has an incredible ease of use and a low barrier to entry while simultaneously having the ability to scale up with comparable (if not better) power, speed, and abstrac- tion to other component libraries, he points out.

> We’re a fully remote team of 15 developers and we rely heav- ily on Slack, Jira, and GitHub. However, it’s actually easier to collaborate in Vue, because it’s not so different from our legacy code—there’s still declarative templating and everything that we are used to.

> Secondly, the ease of writing CSS now is amazing. It made such a tremendous benefit for us. We have many developers speaking different languages with different coding styles. Coming up with the names relevant only for markup in a particular file without worrying about the global namespace. The ease of use is just wonderful.

As Vue has lent great support to the Chess.com team, they will definitely continue working with it in the future.

> We’re all in with Vue.js right now! As I said, right now our process is twofold: essentially re-architecting our components and moving from Angular 1. Therefore, we’re implementing it two totally separate ways simultaneously. That’s elating.

![1509690042(1).jpg](https://ooo.0o0.ooo/2017/11/03/59fc0ac62efa9.jpg)

### Clemenger BBDO

Clemenger BBDO is a full service agency offer- ing a full suite of capabilities including brand strategy, integrated creative development, CX, digital services, CRM, PR, design, shopper and activation.

In the last 12 months the agency has been named World’s most creative agency at Cannes Lions and D&AD.

We decided to pick Vue.js be- cause it was answering all the requirements we had to cover for our projects, while offering a comfortable development environment for our team. It’s so close to native JavaScript, that it’s extremely easy to start working with it.

> From Sylvain Simao, Technical Lead at Clemenger BBDO Melbourne.

**CHALLENGE**

Projects with short lifespans (4 to 12 weeks) done by different people.
Working with animations and transitions.
Need to load and work fast on mobile devices.

**SOLUTION**

Using Vue.js with a pre-render solution for static pages.
Building ES6 modules rather than framework specific code.

**OUTCOME**

Delivered several successful interactive campaign experiences. within strict deadlines.
Digital projects ready for high traffic volumes.
Quick onboarding and project setup.

#### Challenge

Most of the projects Clemenger BBDO works on are campaign websites. It’s mostly frontend with a little backend magic—most projects use the serverless approach, API, AWS services, and the like.

Working on different projects simultaneously under strict deadlines, Clemenger BBDO had to devise a standardized solution that would significantly ncrease development speed and be flexible enough to workacross very different experiences.

> As technical lead, one of the main things I need to keep in min is the ability of my team to deliver high-end, quality projects within short time frames. We are an advertising agency, which means that a 3-month-long project is a really long one, Sylvain explains.

> A fast-paced environment means that we need people to be able to jump quickly into new tools. Sometimes we also need to work with external contractors, so the perfect solution for us was something easy to learn and start working with. Vue gives us a lot of flexibility in terms of workflow—for example being able to work with already known preprocessors for HTML and CSS is a big plus.

On client projects, Sylvain and his team worked with a variety of different JavaScript frameworks.

> I feel like we’ve tried all of them! Sylvain laughs.

> We’ve tried frameworks like Angular, React, and Riot.js, but Vue is the one we fell in love with. Vue offers simplicity and robustness at the same time. For us it’s a breath of fresh air among the others. It has a rich ecosystem out of the box, and the fact that it’s incrementally adoptable makes it the perfect tool for the type of work we have to deliver on.

Interactive campaign websites are challenging in many ways.

> You have to deal with SEO, accessibility, and extended browser support—but also deliver on animations, transitions, and very interactive interfaces in general. Combining those is definitely the most challenging aspect of our work.

#### Solution

Due to its smooth learning curve, Vue.js makes it easy to work with new developers or external contractors.

> We’ve noticed that Vue.js is great in terms of onboarding new people. Why? The learning curve is really smooth and it’s really close to vanilla JavaScript, Sylvain claims.

> For us, as a business, it’s really awesome. People get up-to-speed really quickly and we can deliver more efficiently. One other remarkable point is the incredible quality of the official documentation and resources available for Vue. It probably deserves an award for the most comprehensible framework documentation!

For every website Clemenger works on, it’s important to make it visible for bots for successful SEO.

> For that specific problem we do pre-rendering for all our pages. Most of the time, when we have a new project that requires Vue.js, we start from a boilerplate that we’ve built on top of the official Vue webpack template. Then, we use libraries like PhantomJS or Prep to render static snapshots of the pages. The last step consists of serving those pages to robots, which can easily be achieved by targeting the user agent with Nginx or Lambda@Edge, Sylvain elaborates.

Sylvain uses Vue.js to deal with animations and transitions.

> Right now we are changing our way of approaching animations. Since the release of Vue’s most recent version, there is now a lot more flexibility with the transitions. We now have a more granular access to the transition hooks, that makes it possible to trigger third-party libraries and deliver on complex animations, while still using Vue at the core. I’m trying to push my team to move to that model.

For Airbnb’s campaign website—“Until we all belong”—Vue.js was the technology of choice.

![1509690301(1).jpg](https://ooo.0o0.ooo/2017/11/03/59fc0bc9c12ea.jpg)

> The project is designed as a single page application, based on Vue and webpack at the start. For better efficiency, the web views were hosted in Amazon S3 buckets, which means that we couldn’t use any server-side rendering. Every part of the UI and every page have been built using Vue single file components. In this kind of website, where we are anticipating major traffic, performance is key, and that’s why everything is loaded on-demand. In one of our projects we were recording 6,000 visitors per minute—it was a big buzz. We need to be ready for that, Sylvain explains.

> Vue.js can be a lifesaver in such cases. For the Airbnb project there were big image assets in the background that we needed to load and animate. For that purpose, we’ve used Vue-router to declaratively list assets or data that required pre-loading, and VueX to keep track of those on every page. The project was also challenging in term of interactions, but we’ve managed to deliver the website within 6 weeks.

![1509690342(1).jpg](https://ooo.0o0.ooo/2017/11/03/59fc0bf296b5a.jpg)

#### Outcome

Delivering projects in a timely manner is much easier with Vue.js.

> We wouldn’t be as fast if it wasn’t for Vue. Mostly because of the simplicity of the API. We’ve recently worked on a prototype for a hybrid app built on Angular 2, the syntax is elegant but the learning curve is steep and doing simple things takes time. With Vue you can prototype really quickly and that’s probably its greatest strength.

With Vue.js, the Clemenger team is able to tackle a wide range of different projects

> We now have quite a few projects built upon Vue.js. Airbnb’s Until we all belong, a campaign for marriage equality in Australia, was recognized with a number of industry awards, including AWWWARDS and CSSDA. Another project—Meet Graham which introduce the only person designed to survive on our roads, Graham. Within the first week, the project recorded more than 10 millions page views and it got immersive recognition and media coverage. It was highly acclaimed and received numerous awards, including the Grand Prix at Cannes Lion 2017. One of our most recent project is Snickers Hungerithm, where we’ve decided to rewrite the campaign app using Vue.js for the global rollout. Hungerithm is a hunger-algorithm that monitors online mood using tweets. When anger goes up, Snickers prices goes down in real-time.
