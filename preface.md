## Preface

A few years back, Monterail was a well-established develop-ment agency, renowned for its Ruby and Rails expertise. Now, from today’s perspective, such a label feels a bit odd. We started with traditional Ruby multi-page app development, but pretty soon it became obvious to us that many of the practices and patterns changed as technologies evolved. Backbone.js was our first foray into JS frameworks in 2011, undertaken since we couldn’t just stay inert if we wanted to meet the market needs. We have been actively monitoring this dynamically changing world, and along the way we early-adopt- ed Angular JS and became experts on it. With the advent of the latest generation of component-based frameworks, our team has embraced all the major players in the field, including React (along with React Native), Angular (2 and up), and—most extensively—Vue.js.

## 序
几年前，Monterail因其在Ruby和Rail上的专业建树，还是一家享有盛誉的软件开发商。不过现在看来，Monterail和她的产品似乎有点过时了。当我们用Ruby开发传统多页面应用程序，越来越意识到，随着技术的进步和发展，许多的好的开发实践和范式已经变得不那好了。因循守旧是无法满足市场需求的，在2011年，我们选择了Backbone.js作为我们的第一款js框架。我们一直都积极地关注这个快速变化的世界，较早地采用了Angular JS， 而且对其非常精通。如今，新一代的基于组件的开发框架里，我们团队已经研究了React(包括React Native),Angular(angular2及以上)和使用最广泛的-Vue.js
### Familiar Does Not Mean Better
Before we started working with clients who requested an app written with Vue directly, we were talking to businesses who have never heard of it. Once they did, they were impressed with its openness and power, and wanted to include Vue in their technology stack.
We feel that most companies which choose more well-known frameworks make their decisions without having all the relevant informa-tion and simply adopt something that sounds familiar. They’re usually unaware that somewhere out there, there’s a technology which combines the advantages of Angular and React and adds an additional layer of niceness on top of it.
### 熟悉的不一定是好的
那些要求用Vue开发应用程序的客户在此之前，都没有听说过Vue。可当他们使用后，都对Vue的扩展性和能力留下深刻印象，并希望在他们技术堆栈中包含ue。
我们看到，很多公司那些选择出名的框架，他们做出了这样的决定，并非是因为全面考虑相关信息，而只是因为那些框架比较出名和耳熟而已。他们并没有意识到，名不见经传的Vue结合了Angular，React的先进的部分，并且更加友好。
### The Rationale Behind the State of Vue.js Report
### 为什么要做这份调查
With Vue in our tech stack we can efficiently deliver better productsit helps us drive our business and make clients happy, and so we believe it deserves all attention and love. With that in mind, we embarked on the journey to evangelize to developers and businesses and spread
the word about Vue. That’s how we ended up curating the weekly Vue-newsletter, organizing VueConf, the first international Vue.js conference in the world, and creating libraries like Vuelidate and Vue-multiselect.
<br>
当使用Vue后，我们能够更有效率地交付更好的产品，更好地推动我们的业务，使客户更加满意，我们相信:Vue值得关注并受到大家的喜爱。也就因为这样，我们决心开始向发者们和企业布道，把Vue传播到全世界；同样也是因为这样，我们策划了每周的Vue-newsletter,组织了全球第一次VueConf国际会议，创建了Vuelidate和Vue-mulitselect这样的Vue库。<br>
The report you’re reading is yet another milestone in that mission. It was created for three primary reasons. One, to provide a reliable source of Vue.js business use cases so anyone can get a sneak peek at how other companies use Vue.js. Two, to reach more individuals who have never heard of Vue and provide them with good reasons to give the framework a closer look. Three, to never, ever again have to convince our clients that Vue.js is a ready-to-use solution and has everything we need to build all kinds of applications.
<br>
你即将阅读的这份报告我们是布道与宣传Vue的另一个里程碑。报告有三个主要目的。1.提供可信赖的Vue商业使用案例，让任何人都能够一窥其它公司对Vue的使用；2.让那些没有听说Vue的人了解Vue，并让他们有足够的理由来更加仔细了解这个框架；3.让我们不再费力地说服客户Vue.js已经是一个成熟的解决方案，可以帮我们构建各类应用。

### Contents of the Report
### 报告的内容
The **State of Vue.js** report offers a business owners’ and developers’ perspective on Vue. We surveyed over than 1,100 specialists from 88 countries to find out their experiences with Vue, and what they like and dislike about it most. We dug even deeper, and interviewed six companies on what problems they wanted to solve with Vue.js. To give you an overview of its growth over the years, we described the story of Vue.js, also including a sneak peek of what’s coming next from Evan You, the creator of the framework himself.
Enjoy the read,<br>
**报告**展示了企业主和开发者是如何看待Vue的。我们调查了来自88个国家的1100多名行业专家，了解他们的对于Vue的使用体验，哪些特性是他们喜欢的，哪些是不喜欢的；继续深入，我们采访了6家公司，询问他们想用Vue.js解决哪些问题；另外，我们讲述了Vue.js的历史，包括框架的创建者尤雨溪对Vue.js未来的大致规划，让你对Vue的发展有一个全面的了解。
![](https://i.niupic.com/images/2017/10/31/fXsajR.png)

We would not be able to pull this report off if it weren’t for many amazing people who supported us along the way. They all were a tremendous help, sharing their knowledge and experiences, just because they wanted to give back to the community they’re part of.
<br>
报告的顺利完成得到了许多人的支持。他们分享他们的知识和经验，给予了我们莫大的帮助，仅仅因为他们想为社区贡献一份属于自己的力量。
Big thank you to Evan You, who was excited about the report from the very beginning and had our backs during the creation of this very piece of content. He also agreed to share invaluable insights about the future of Vue.js and supported our writing efforts.<br>
感谢Evan You（尤雨溪）。他从一开始就对这篇报告抱以热情，也在创建报告过程的各个阶段支持我们。Evan You（尤雨溪），分享了对Vue.js的未来的看法，并支持我们的创作工作。<br>
Evan, as well as Chris Fritz, Vue.js core member, were insanely helpful with analyzing the State of Vue.js survey results. Kudos for that. Because of our collaboration, we felt comfortable about the quality of the final product.<br>
感谢Chris Fritz，Vue.js的核心成员！对我们分析调查结果给予了很大的帮助。点赞！因为有了这样的合作，我们对最终的报告的质量非常满意。<br>
The case study part of the report would never come into existence if it weren’t for all those who agreed to spend their time sharing their stories. The warmest thank yous to Jacob Schatz, Sylvain Simao, Roman Kuba, Gilles Bertaux, Scott O’Brien, Erin Depew, Matt O’Connell, and Yuriy Nemtsov.<br>
非常感谢Jacob Schatz, Sylvain Simao, Roman Kuba, Gilles Bertaux, Scott O’Brien, Erin Depew, Matt O’Connell和 Yuriy Nemtsov.没有你们花费时间分享他们的故事，报告中的学习案例就不会存在。<br>
### Contributors
### 主要贡献者
![](https://i.niupic.com/images/2017/10/31/gLIe1Z.png)
