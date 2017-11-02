## Case Studies

One of the reasons for drafting the State of Vue.js report
was to provide a substantial body of evidence that Vue
is a mature technology, adopted by companies of various
shapes and sizes. Each presented case study proves that Vue is ready
for commercial usage. All six companies we interviewed had faced
the challenge of choosing the right framework, and they all decided
to go with Vue—even though they are in different stages of growth
and have different goals.

Before Codeship started working with Vue, their audience expe-
rienced freezes and browser crashes. They had a long list of users
who were dissatisfied with the performance of the app. Their story
is a great example how Vue can help build a reliable software, with
a bulletproof, easy-to-maintain code.

If you’re looking for a good illustration of how enterprise-level orga-
nizations use Vue.js, the Behance and Adobe Portfolio case study may
come in handy. Their team built two independent products in Vue from
the ground up—and they’re not going to stop there.

In the Livestorm case study, Gilles Bertaux, co-founder and CEO, de-
scribes how they created a profitable product starting from scratch.
Thanks to Vue and its reusable components, their development has been
faster and much easier.

Jacob Schatz, frontend lead at GitLab, explains why they decided to move
from jQuery to Vue.js and describes the main challenges they encoun-
tered along the way. Their focus on better UX resulted in a more desirable
product and therefore in increased sales.

Chess.com had to deal with hard-to-maintain legacy code in Angular 1.
With Vue.js, they found it much easier to collaborate within their fully
remote team of 15 developers. Chess.com is a platform with a massive in-
frastructure serving 19 million users around the world. In their case study,
you’ll find out how Vue.js solved many of their issues.

The last case study differs a lot from all the others. Sylvain Simao, techni-
cal lead at Clemenger BBDO Melbourne, explains how they use Vue.js for
projects with short lifespans—from 4 to 12 weeks. The biggest challenges
they encountered included tight deadlines, working a lot with animations
and transitions, and delivering highly-performative campaign websites.

### Behance & Adobe Portfolio

**Behance** is the leading online platform for showcasing and discovering creative work.
**Adobe Portfolio** is a custom website builder designed to enable users to showcase their creative work.

> We were a little hesitant since there aren’t all that many major companies using Vue out there. However, every time I’ve had any issues, it’s usually because I was overthinking it, and I was pleasantly surprised when it really was that easy to implement.
>
> From:
> Erin Depew Software Engineer at Behance
> Yuriy Nemtsov Software Engineer & Manager at Behance
> Matt O’Connell Software Engineer at Adobe Portfolio

#### CHALLENGE

Moving from homegrown solutions to community-supported technology.
Maintaining high user experience and performance.
Being able to share components between other teams and projects.

#### SOLUTION

Switching the Behance and Adobe frontend teams to Vue.js.
Using Vue.js to migrate the existing codebase.

#### OUTCOME

Comfort of converting the site at an unhurried pace, without having to do it from scratch.
Ease of integration with existing codebases.
High performance and cost effectiveness.

### Challenge

Adobe and Behance, a company under the Adobe umbrella, have been
leveraging the latest technologies and design thinking to create revolu-
tionary products that connect and empower the creative world for years.

The team had decided it was time to update to a community-support-
ed open-source framework since they were starting to hit the limits
of the homegrown technology that they were currently using.

> Before Vue, we were using a homegrown MVC framework
that leaned heavily on Hogan.js (mustache) and jQuery. Our frame-
work wasn’t able to render declaratively, forcing us to imperatively
keep the DOM in sync with the data. It also didn’t have the ability
to compose features into components, enforce a unidirectional
data flow, nor a comprehensive documentation. So, even though
it worked well for years, we were ready to switch to a framework
that would allow us to build features rapidly with fewer bugs, facil-
itate their maintenance, and allow for quicker onboarding of new
people, Yuriy explains.

![](https://i.loli.net/2017/11/02/59faea0ada687.jpg)


> Mustache specifically was important to us, because we were using
(and still are, for the majority of behance.net) the same templates
on the backend and frontend. The speed with which we can deliver
the first meaningful byte to the browser is significant to us and our
users. That same speed would be tremendously difficult to achieve
if we were to wait for the browser to download the JS, parse, com-
pile, and execute it, and only then display that project to the user.
We were also looking specifically for a framework with server-side
rendering capabilities, he says.

For the Behance team, the primary goal was to build a codebase
that’s easier to work with and a strong foundation for new features to be
added going forward.

> I think that one of the biggest challenges that we’ve faced
is that since we’ve decided not to “split” our codebase and start with
a clean slate, we had to spend a lot of time unraveling older code
to form new components. That trade-off between refactoring older
code to Vue while still maintaining the rest of the site and shipping
features has definitely been challenging, Erin elaborates.

> We also take performance very seriously at Behance, so we have been
very careful to make sure that we can keep our performance metrics
while converting over the codebase.

For Matt and his team, user experience was also an important factor,
one leaving much room for improvement.

> Regarding Adobe Portfolio, we started with nbd.js, which is a cus-
tom-rolled version of Backbone that was originally extracted from
a product we no longer have, called “Action Method Online.” From
there, we used that to build large chunks of the Behance network.
It had limitations for reactive systems, so we built the “reactive” part
of portfolio using Ractive, Matt adds.

> The biggest challenge thus far has been, just like in the case
of Behance, maintaining a fast user experience with complex user
data state management, while providing instant feedback on both
the content and styling of a user’s site.

### Solution

Rather than establishing new developer teams who would focus only
on Vue.js, both Adobe Portfolio and Behance retrained their existing
teams to use Vue.js in their day-to-day work.


> The vast majority of the team was here before we switched to Vue.
Once we made the decision, we needed a few small projects to cut
our teeth on. For us, that meant very small, frontend only features,
and a set of features that weren’t publicly accessible, like our
style guide. This way, we could learn how to use Vue, how to write
the tests, and to style the components relatively safely. Only then
did we feel comfortable enough to take on a larger project. That was
Behance Live, Yuriy recalls.

![1509617601(1).jpg](https://i.loli.net/2017/11/02/59faefebec94a.jpg)

> On Portfolio, our entire frontend team works with Vue—nine en-
gineers in total. Some of our backend developers are also starting
to pick it up as well. There are about eight frontend developers
on the Behance product who program in Vue, Matt explains.

> There is quite a bit of overlap between the two teams (Adobe Portfolio
and Behance). We share a lot of libraries and APIs between our code-
bases and feature roll-outs usually appear on and require collabora-
tion between both sites, Erin adds.

The Behance team encountered many challenges on their way
to determine how to structure the application in general, and how
to define the roles of different components.

> The vuex store was also tricky to structure for a larger application.
We decided to use namespaced modules. It wasn’t clear at first
whether there should be a single store-module per route/page or data
type (e.g., user or project). Creating route-specific stores meant
that the actions across routes wouldn’t be reused. Making them
data-specific was the best solution for us, with a top-level route
store-module that combines the modules that the route needs. The
solution is, however, still far from perfect, Yuriy says thoughtfully.

> To define roles of various components, we make a distinction between
a “page” component (the first component that the router points
to and the one that interacts with vuex) and a “dumb” component
(that solely sends properties down to child components and borad-
casts events up to their parents).

Using Vue.js for almost a year now, Matt and his team managed to build
or rebuild a bunch of features.

> At Adobe Portfolio, we started with the Manage Content feature—
the area where users can reorder, add, delete, and perform various
other actions on their portfolio site. As needed, we created reusable
UI components like select dropdowns, overlays, toggles, and drag
and drop lists, Matt says.

### Outcome

According to Erin, due to its progressiveness and great flexibility, Vue
is easy to integrate with Behance’s existing codebase.

![1509617746(1).jpg](https://i.loli.net/2017/11/02/59faf0615bbaf.jpg)

> I always say that every framework is just another tool. However, one
of the biggest benefits of using Vue, besides the speed and stellar
documentation, is how well it integrates into our existing codebase.
Unlike with other component-based frameworks, Vue has given
us the luxury of mounting our components onto our existing pag-
es, enabling us to slowly convert the site at our own pace instead
of going all-in.

> I’d say Vue exceeded our expectations. We were a little hesitant since
there aren’t all that many major companies using Vue out there.
However, every time I’ve had any issues, it’s usually because I was
overthinking it, and I was pleasantly surprised when it really was
that easy to implement, she adds, laughing.

> Currently, we’re planning on converting our entire Behance codebase
over to Vue, and, of course, recommending the adoption of Vue
to other Adobe teams.

In Yuriy’s opinion, Vue.js gives developers just as many possibili-
ties as other frameworks. In contrast to some frameworks, however,
it makes development easier and... less expensive.

> I wouldn’t necessarily say that Vue allows you do things that you
couldn’t achieve using a different framework. However, it was re-
ally difficult to squeeze proper SSR performance from React. Prior
to the Fiber rewrite (React v16), a page with a large component
tree would block the main execution thread, which, in turn, meant
that if it took 100ms to render one page, all of the other clients
of that Node server would just wait. So, we needed to either in-
crease the number of processes-per-server or the number of servers
to increase throughput. This was difficult to maintain and more
expensive than it needed to be. Vue’s SSR story is much stron-
ger. There’s caching and streaming built in. As a result, even
without spending a lot of time optimizing, the performance is good
on Behance Live, he says.

> Working with Vue.js definitely is different than with other frame-
works. Somehow you just tend to enjoy your life more.

![1509617816(1).jpg](https://i.loli.net/2017/11/02/59faf0a462160.jpg)
