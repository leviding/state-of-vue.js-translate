### Codeship

Codeship 是一个持续集成平台，它可以让你在云端放心地发布你的应用。在 Codeship 上的开源项目总是免费的。

> Vue gave us all the flexibility we needed, to do what we wanted to do. It offers a solid founda- tion that can be expanded any way we like and it’s not opinionated about tools we use in the pursuit of our objectives. That’s what I really like about it.
>
> From Roman Kuba, Lead Frontend Developer at Codeship.

**CHALLENGE**

Freezes and crashes inside the application.
Difficulty running unit tests with Angular.
Ambitious plans for new features and building new, complex things.

**SOLUTION**

Building a proof of concept and convincing other developers to give Vue.js a try.
Moving away from acceptance tests only.
Refactoring and rewriting pages.

**OUTCOME**

Not a single crash of the app since Vue.js was implemented.
Bulletproof, reliable, and easy-to-maintain code.
Positive feedback from customers satisfied with the current UX.

#### Challenge

Codeship, a CI platform used by companies such as CNN, Red Bull, and Product Hunt, launched in 2010. With jQuery and CoffeeScript in their stack, they built a successful platform for developers around the globe.

But as time went on, the team realized that it’s time to find a technology that would support further development and facilitate building more complex things.

> To give you some perspective—Codeship is used by a ton of customers who rely on it in their day to day operations. When we’re working on a feature for, let’s say, four months, it somehow feels bad, like we’re holding something back from our customers. If we spend two months fixing features, this in turn means two months of pain and uncertainty for them. It is absolutely crucial for us to be fast and deliver reliable products, Roman says.

![1509692542.jpg](https://ooo.0o0.ooo/2017/11/03/59fc15158019e.jpg)

> We have pages that basically show the complete terminal output as readable log for our users, so they can see what test went through and what output they have. It was clear very soon that something like jQuery, on which our product was running be- fore, wouldn’t cut it anymore because of the growing complexity, Roman reflects.

> We started working with Angular 1, which we used for the next six months. Why? Well, mostly because I was already familiar with it.

The company switched to Angular and it was a good fit. Yet, as the ser- vice grew, it soon became apparent that sticking with it would not be feasible in the long term.

> One of the things that we tried to improve was the performance. That was the biggest problem with Angular. The sheer amount of data we needed to present on the build page was way over An- gular’s capabilities. Customers were reporting serious issues with the app—the page was unresponsive, and some people were even expe- riencing freezes and browser crashes.

Roman, however, didn’t want to give up on Angular right away.

> Of course, we tried to optimize as much as possible. I even tried to move parts of the rendering out of Angular’s default list rendering and use plain JavaScript instead, but it didn’t work, Roman sighs.

> At some point, Angular was trying to grasp what was going on the page as Angular tried to keep track of its scope and ran the relevant digest cycles... That killed performance, regardless of whatever we tried to assuage the hit. There was no way it could have run smoothly.

Another significant challenge that Codeship faced was improving the testing process and making the app more reliable.

> With Angular, we still leveraged acceptance tests as much as possible. We basically ran user stories in the entire application. It was incredibly painful to run unit tests with Angular itself and test component, module or controller only. It was barely giving us the full picture we so badly needed, Roman explains.

#### Solution

The first step of transitioning away from Angular was getting the approval of the staff and the VPE.

> At first, it was a struggle to get everyone on board with with Vue. The team had never heard of it, whereas they knew of Angular 2 and knew that Google was throwing its weight behind it, and they knew about React, backed by Facebook, Roman says.

> In conversation with the team, usually the first question was about the size of Vue.js community—people wanted to know whether there was any chance of getting support should the need to do so arise. Because the majority of our staff has roots in backend, they wanted to stick with trusted names they heard of.

Roman decided to use his knowledge and research to convince them to move to Vue.js.

> I made some samples and an internal presentation to at least make them trust the decision and the reasons behind it,” he says. “If you read briefly through the source code of Vue, you’d quickly see that the code is not so hard to extend by yourself. It’s not a giant entity like Angular or similar.

Before Codeship jumped straight to development, they needed a proof of concept.

> By then I had little experience with Vue, my expertise in the framework was definitely limited. However, starting with Vue seemed effortless and I quickly felt that it would be the solu- tion to most of the problems that plagued us. In one evening or so, I rebuilt a crucial part of our rendering with Vue, and tried it against a large amount of Loglines as a proof of concept. Then

![](https://ooo.0o0.ooo/2017/11/03/59fc15add61e8.png)

> I did all the CPU profiling. That was the one thing that immediately demonstrated to my team that Vue.js has already given us a huge performance improvement. We cut the rendering time from 30 seconds to 7 or so, Roman recalls.

Proof of concept in hand, Roman and his staff could finally start the transition to Vue.

> We tried to move the proof of concept and replace what we had with Vue. The actual risk here was quite minimal. We had a system that was breaking for users, so... What was the worst thing that could happen? Roman laughs.

> I spent a week refactoring and rewriting the page and then shipped it to users for feedback, trying to get validation fast. After just one day we knew that all that problems that plagued us in the past were gone. Even with 15Mb of log rendered. With rendering times between 30 and 40 seconds (we’re currently working to decrease that number further), the app works splendidly across all browsers and we haven’t recorded a single crash.

![](https://ooo.0o0.ooo/2017/11/03/59fc15e8cc1c8.png)

Moving from acceptance tests made the testing part more pleasant and reliable.

> We moved away from acceptance tests and started wondering what we can take away from and use Jest and Vue tests for. We use mul- tiple components even for complex pages in Vue itself, but only test it through Jest for example, because we have snapshots and verify whether the render HTML is actually the one we want, Roman explains.

#### Outcome

Engineers who rarely do frontend work now feel empowered to touch pieces of code.

> Angular, with all its structure, modules, models, and controllers, and dozens of other things... introduces an unnecessarily high level of complexity. For these engineers, most of it sounds like weird magic spells. But when they actually saw Vue.js, they felt empowered to dig into it right away. That’s a pretty big win for our company, Roman reflects.

Vue.js helps Codeship organize their code and improve user experience.

> It helps us deliver features faster and our users love that they don’t have to wait for months for something they need or expect. One of our pages that was running on jQuery had this weird kind of structure. We moved it to Vue and rebuilt it. Now, it provides a more granular experience and interaction with the UI, and so it significantly improved the UX. People tell us about it all the time.

> With jQuery, the code would be very messy, hard to maintain. With Vue, it’s different, you’re able to harness the power of its components and start leveraging its ecosystem, like Vuex for example. What we do right now is page state management—something we have nev- er done before, not in such a clean way.

For Codeship, Angular testing was an incredibly painful process. With Vue.js, they know that their code is bulletproof.

> Vue.js seriously upgraded our testing protocols. We have Jest in place, which is a smart test runner for us. With Vue, we feel like we have way more control over every aspect of the app, Roman elaborates.

> I can run 15 tests that try to perform specific actions. Such an approach allows me to easily identify code breaks. This is not something I could do this way in an acceptance test due to the sheer amount of time it would take to run. And the result is simply not worth the effort. Unit tests are great in that respect. Code-wise I know that it’s bulletproof, as we test it in a completely new way and it’s incredible.

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
