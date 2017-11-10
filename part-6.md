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
客户对当前的用户体验给出了正面反馈。

#### 挑战

Codeship 是由 CNN, Red Bull 和 Product Hunt 等公司在 2010 年推出的 CI 平台。 他们的技术栈中包含了 jQuery 和 CoffeeScript，他们为全球开发者建立了一个成功的平台。

但随着时间的流逝，这个团队意识到是时候该去找一个新的技术去支撑更久远的发展以及促进更复杂东西的建设。

> 给你们看一个场景 —— 大量的客户在他们的日常操作中依赖着 Codeship。当我们正在开发一个新功能时，通常可能需要四个月的时间，不知为何，这样总感觉不太好，就好像我们正在从顾客那里拿回什么东西。但如果我们花两个月的时间去开发功能, 就反过来了，这往往意味着两个月的痛苦并且对客户不负责。快速而可靠的提供产品对我们来说至关重要。Roman 这么说。

![1509692542.jpg](https://ooo.0o0.ooo/2017/11/03/59fc15158019e.jpg)

> 我们拥有能够完整接收终端输出的页面作为我们用户的可读日志,这样他们就可以看到什么样的测试通过了以及测试的信息。像我们之前的产品使用 jQuery，因为一些变得越来越复杂的原因，不得不将它砍掉,对比很明显。Roman 反映道。

> 接下来的六个月里面我们使用了 Angular 1。 仅仅是因为我们对它比较熟悉。

公司切换到了 Angular 而且适应的很好。然而随着服务的增长，我们发现坚持使用它从长远的角度来讲是不太可能的。

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

> 当时我对 Vue也没有太多的经验，我对框架中涉及到的技术了解十分有限。但是，从 Vue 开始似乎毫无费力，我很快就意识到这是一个针对困扰我们大多数问题的解决方案。只用了一个晚上左右，我就用 Vue 重构了一个关键部分并试图使用大量的 Loglines 作为概念验证。然后我对所有的代码做了CPU性能分析，这件事立即向我的团队证明了 Vue.js 已经给我们带来了巨大的性能提升。我们将渲染时间从30秒缩短到了7秒左右。Roman 回忆到。

![](https://ooo.0o0.ooo/2017/11/03/59fc15add61e8.png)



概念验证在手，Roman 和它的员工终于可以开始向 Vue 过渡了。

> 我们曾经尝试move the proof of concept and replace what we had with Vue。这里头的实际风险非常小。我们有一个系统对于用户来说正处于崩溃状态，所以，还会有更糟糕的事情发生吗？Roman 笑道。

> 我通过花了一个礼拜的时间重构并重写页面，然后将它发给用户来获取反馈来快速验证工作的可行性。只过了一天的时间，我们就发现过去困扰我们的问题全部都消失不见了，甚至是在有 15 Mb 日志呈现的情况下。在渲染时间在 30 到 40 秒之间（我们正在努力进一步减小这个数字），应用在所有的浏览器上都能够出色的运行并且没有被我们记录到任何一次崩溃。

![](https://ooo.0o0.ooo/2017/11/03/59fc15e8cc1c8.png)

抛弃验收测试使整个测试部分变得更加愉快和可靠。

> 我们抛弃了验收测试，开始考虑我们可以拿走什么，并使用 Jest 和 Vue 来测试。我们在 Vue 中使用多个组件，甚至是复杂的页面，但是只能通过 Jest 进行测试，因为我们有快照并验证渲染 HTML 是否是我们想要的。Roman 解释道。

#### 产出

一些很少做前端的工程师现在感觉有能力去接触一些代码片段了。

> Angular 和它的结构、模块、模型和控制器，以及几十个其他东西。。引入了不必要的高度复杂性。对于这些工程师来说，大部分名词听起来就像是奇怪的魔法一样。但是当他们真正地看到 Vue.js 的时候，他们能感觉到自己有能力去马上深入研究它。这对于我们公司来讲是一个非常大的胜利，Roman反映道。

Vue.js 帮助 Codeship 组织他们的代码并优化用户体验。

> 它可以帮助我们更快的交付所需功能，用户不需要为了他们需要的或者期望的东西来等待数个月的时间，他们非常喜欢这一点。我们的页面中有一个是基于 jQuery 运行的，它的结构非常奇怪。我们将它基于 Vue 重构了。现在，它提供了更加细化的体验和更友好的 UI 交互效果，因此，它显著地改善了用户体验。人们总是这样告诉我们。

> 使用 jQuery 的时候，代码非常混乱，难以和维护。而使用 Vue 的时候就不一样了，你可以利用它组件的强大功能和它的生态系统，比如 Vuex。我们现在正在做的是页面状态管理，这是我们以前从来没有完成过的，至少没有以这样一种干净的方式完成。

对于 Codeship 来说， Angular 测试是一个非常痛苦的过程。而用了 Vue.js，他们知道他们的代码是牢固的。

> Vue.js 认真地升级了我们的测试协议。Jest对我们来说是一个比较聪明的测试工具。但是有了 Vue 之后，我们觉得我们又更多的方法来控制应用的各个方面，Roman 阐述道。

> 我可以运行 15 个执行特定操作的测试。这样的方式可以让我轻松地识别代码中的断点。在以前的验收测试中，我没办法这样做，因为这需要消耗很长的时间。得到的结果不值得我们付出那么多的精力。单元测试在这方面反而更好。在代码方面，我知道它是牢固的，因为我们以全新的方式对它进行测试，结果令人难以置信。

### GitLab

GitLab is an open core, integrated solution for the entire software development lifecycle.

> Every framework will struggle in certain areas. With Vue.js, every struggle will be your own, not Vue’s. It’s just a perfect framework.
>
> From Jacob Schatz, Frontend Lead at GitLab

**CHALLENGE**

Difficulty with implementing complex features and maintain cur- rent ones.
Large Rails + jQuery application that was hard to scale.
Insufficient app speed.

**SOLUTION**

Gradually introducing Vue.js to GitLab to be used along with jQuery.
Using Vue.js for all applicable new features and migrating old ones. As needed, without doing a complete rewrite or refactor.
Using webpack to create optimized bundles.

**OUTCOME**

Easier maintenance of a unified style guide within the whole codebase and code architecture.
Highly improved time and cost efficiency.
Improved user experience leading to better sales thanks to the ability to implement more sophisticated features.
Improved page load times by reducing asset size.

#### Challenge

After six years on the market, GitLab has established itself as a wellknown solution for developers hailing from thousands of companies. Only two years back, most of its code was still written in Rails and jQuery.

By 2015, the company had no frontend developers on staff and that set- up worked really well. Rails devs were writing frontend code and doing a fantastic job. Yet, the company’s plans for the future required a new solution.

> When I came in I saw that we have these individual jQuery things which were very simple, but for more complex things that we wanted to do, the really big ideas that we wanted to achieve, we would need something else, Jacob explains,

![](https://ooo.0o0.ooo/2017/11/03/59fc19771d8ba.png)

> jQuery is fantastic, but it creates potentially more bugs as you’re responsible for literally every state change.

To meet their goals, GitLab started looking for a new solution.

> We checked Backbone, which I had previous experience with, we obviously looked at React, but also Knockout, Ember, and all those different frameworks. I wanted to do a small project using each. By then I didn’t even bring up Vue.js at all! Jacob recalls.

Testing all these frameworks helped Jacob identify their advantages and drawbacks.

> Backbone has a lot of tools to get stuff done and a good structure, but you’re still in the same boat as with jQuery. With React it scared me a bit to get involved with a framework that depended on a big company. Also, it didn’t seem to scale well for me. I really liked Mi- thril! The only problem is that it’s not pretty to write at all. If they could put a couple of extra layers of niceness on it, I’m sure people would start adopting it.

Another big challenge was to make a mature switch to a new technology. It was a bit risky, and thus had to be well executed.

> In GitLab, we have tons of code. When I joined, there were already eight thousand lines of JavaScript in our codebase. I obviously didn’t want to do something that would be a complete rewrite. We actually still have some chunks of jQuery here and there.

#### Solution

After testing a few frameworks, Jacob still didn’t have a perfect match on his hands. It was only after he wrote a pretty big project with an early version of Vue.js he realized that he may have struck gold.

> When I had this one project together, I knew it was something we could write a lot of code with. It wasn’t just about writing a simple to-do app. When you get to work on this large application— that’s where all problems actually start, Jacob explains.

Before GitLab started diving into Vue.js, they needed a proof of concept.

> Phil Hughes [Sr. Frontend Engineer at GitLab], created a proof of concept where we took a major feature that we were doing—issue boards. Phil wrote that using Vue.js and it was immediately apparent that we got a tremendous amount done in a small amount of time! Without all those bugs which typically came with jQuery, Jacob says.

![](https://ooo.0o0.ooo/2017/11/03/59fc19cb934bd.png)

Vue.js supports the approach evangelized by Jacob within his team—it- erate small and create proofs of concept.

> We constantly have 4 or 5 proof of concepts going on, he says.

Using the same approach, GitLab introduced webpack to be able to split the assets into smaller chunks downloaded by the browser and thus improving the app load time.

> We created a small proof of concept to see if webpack was even feasible. When we found out that it was, we went the whole way and end- ed up writing and entire Trello application in Vue. And replacing the billion-dollar industry in one month. Good job, Phil! Jacob laughs.

One feature of Vue.js turned out to be the most useful out of all—reac- tive templates.

> It’s a very, very simple thing that Vue does. One of the first things I programmed in GitLab was to take the issue page, and when you clicked close, you had to refresh the page. And now when you click close, it just changes the status of the merge button, changes the status of the button below. It does all those things automatically. In jQuery, there was a ton of code. At least 30-40 lines to make sure that the buttons were in the right state. With Vue.js it was literally one line of code. The view always reflects the current situation, Jacob explains.

> And now that we use Vuex, it can be done better than before. The state management stuff made a HUGE difference.

With all its advantages, Vue turned out to have one drawback.

> Currently, there are 15 developers at GitLab. With frameworks like Angular you kind of work in the same way together. Vue is much more open, and so we had to create documents explaining how we write in Vue.js. What patterns you’re going to follow. Still, it’s something that we’ve solved. The openness of Vue is also its beauty, but you need to make sure everyone’s on the same page.

**[VUE.JS STYLE GUIDE BY GITLAB](https://docs.gitlab.com/ee/development/fe_guide/style_guide_js.html)

#### Outcome

> Scaling up the application and introducing new features would be possible with jQuery, but it would be much harder to maintain.

> What we do right now would require a tremendous amount of code and a lot more organization. Vue has a lot of these problems solved, Jacob says.

> With something as reactive as Vue.js, you give it a variable, and it’s going to bind it into the DOM directly and take care of everything else. Especially in Vue 2.0 with its virtual DOM. We wanted to increase our performance, and it was one way to simplify our workflow.

Thanks to Vue.js, GitLab can iterate quickly and improve their usability.

> We can finally focus on usability and UX, where before we were fo- cusing on little tiny things and code. Now we think about the much bigger picture.

Vue.js is so open and accessible that it’s pure pleasure for GitLab frontend developers to deal with it on a daily basis.

> Vue, in contrast to other tools, does not follow any strict guidelines. It’s open and that’s fantastic. I like everything what it does right now. Of course, it’s got the most amazing documentation you can imagine. It’s really straightforward to get started with it and onboard new people.

Vue.js helped GitLab improve time and cost efficiency.

> We know for a fact that our development is faster. That’s an easy thing to see. From the sales perspective, those nicer UX features we’re creating bring people to GitLab and make it a much more desir- able product. People love the new things we put in there with Vue.js. We increase the user experience, and so we increase sales.

Jacob agrees that they will definitely use Vue.js in the future.

> We’re all set! We have other challenges now. Currently, we’re trying to improve our process and speed up our testing. Vue.js solved so many problems for us that we’re definitely keeping it for the future.
