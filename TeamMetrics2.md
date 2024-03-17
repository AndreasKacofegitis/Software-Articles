<link rel="stylesheet" type="text/css" href="./custom.css">

# Practical Software Metrics for Teams
  

The most effective, productive, and engaged teams that I've worked with have used many of the metrics in this article.  While it wasn't appreciated at the time, we did use metrics to drive our behaviours to improve our practice, our processes, and our behaviours. Conversely, the one organisation that resisted the building of systems to promote these metrics, interestingly, was the lowest performing organisation I've witnessed.  Is there a strong correlation between the well-inteding use of metrics and team performance?  I think so.  Regardless, employing some of the following metrics in your organisation will, if well-selected, at least not hurt.

Many of the below metrics require the actual data to back them.  It isn't the objective of this article to demonstate how to achieve this, and I generally assume that you have the data at hand.  If you don't, and there were many times that I didn't, the path to discovering the information was very fruitful and enlightening in and of itself.  Often this was hard work, and sometimes required specific development time and effort.  And a great deal of persistence. But always worthwhile.

My desire is that this article makes you think, and hopefully, that you act.  Whether you agree with my points or not, I'd consider you taking one single action in your workplace a success.

Please keep in mind that I've only lightly tread on each of the following points; most of  these are topics that are broad and deep, and often don't have only one single interpretation.  Ideally they would be elaborated upon further, but I'm very mindful of the saying "I'm sorry I didn't write less, but I ran out of time" (a contortion of Mark Twain's quote).  Regardless, this article is plenty long enough, so for what it's worth; I'm sorry I didn't write less, but I ran out of time :).  I'll look at a deeper dive into a selection of topics some time in the future and as feedback, or my whim, guides me.  Thanks so much for reading.



- [Practical Software Metrics for Teams](#practical-software-metrics-for-teams)
  - [Metrics Categories](#metrics-categories)
  - [What is a metric?](#what-is-a-metric)
  - [Metrics for team performance](#metrics-for-team-performance)
    - [How to use these metrics](#how-to-use-these-metrics)
  - [Features: Preparation and Completion](#features-preparation-and-completion)
    - [Amount of Ready work: The beginning of the funnel](#amount-of-ready-work-the-beginning-of-the-funnel)
  - [Done Work: The end of the funnel](#done-work-the-end-of-the-funnel)
  - [Delivery metrics](#delivery-metrics)
    - [Predicatablity](#predicatablity)
    - [Project burndown - daily chart](#project-burndown---daily-chart)
    - [Quantity](#quantity)
    - [Consistency of Quantity](#consistency-of-quantity)
    - [Size variation](#size-variation)
    - [DevOps](#devops)
      - [Commit activity](#commit-activity)
      - [Automated tests](#automated-tests)
      - [Environmental efficiency - Time to production](#environmental-efficiency---time-to-production)
      - [Release cadence](#release-cadence)
      - [Release punctuality](#release-punctuality)
      - [Regression test cycle time](#regression-test-cycle-time)
    - [Process and Bottlenecks](#process-and-bottlenecks)
    - [Quality, Reliability, and Confidence](#quality-reliability-and-confidence)
      - [Bug count](#bug-count)
      - [Bug severity](#bug-severity)
      - [Speed of response](#speed-of-response)
      - [Rollbacks and fixes](#rollbacks-and-fixes)
      - [How many Support Tickets have been raised against a specific feature/release?](#how-many-support-tickets-have-been-raised-against-a-specific-featurerelease)
      - [Helpdesk sentiment](#helpdesk-sentiment)
      - [Helpdesk staff scheduling](#helpdesk-staff-scheduling)
      - [Release confidence and staff scheduling](#release-confidence-and-staff-scheduling)
  - [Communication](#communication)
    - [General comms metrics](#general-comms-metrics)
      - [Whiteboard design](#whiteboard-design)
      - [Distraction balance](#distraction-balance)
      - [Peer programming](#peer-programming)
    - [Meetings](#meetings)
      - [Length, frequency and purpose](#length-frequency-and-purpose)
      - [Meeting Positivity](#meeting-positivity)
  - [Softer team metrics](#softer-team-metrics)
      - [Team temperament (the imposter of triumph and disaster)](#team-temperament-the-imposter-of-triumph-and-disaster)
      - [Attrition of people](#attrition-of-people)
      - [Team Flex, Eagerness and Embracing change](#team-flex-eagerness-and-embracing-change)
      - [Leadership and Positive resistance](#leadership-and-positive-resistance)
      - [Greater than the sum of its parts and masking of weaknesses](#greater-than-the-sum-of-its-parts-and-masking-of-weaknesses)
      - [End user empathy](#end-user-empathy)
    - [Control and Protectionism](#control-and-protectionism)
- [Conclusion](#conclusion)
- [Appendix](#appendix)
  - [What is a High Performing team?](#what-is-a-high-performing-team)


## Metrics Categories
Metrics for software development, fall into the following overlapping categories:

1. To measure team performance (the topic of this article)
2. To measure the success or effectiveness of major, or significant, features
3. To ensure software, infrastructure, and key services are running smoothly

This article focuses on "team performance" metrics.

## What is a metric?

The word metric has its origins in the Greek language; derived from the word "metron" (μέτρον), used in a variety of contexts, but broadly meaning to 'measure', or to 'count'.  For the purposes of this article, we'll use the term to mean something that can be measured, and also have a number attributed to it as a result of the measurement.


## Metrics for team performance
<center>
<img width="70%"  src="./General images/meticsHeader.drawio.png">
</center>
Teams are the hallmark of your success; it's always people and I hope that it will always be people who are the pivot between success and failure.  The immediate thought of gauging team effectiveness through metrics may seem a little contrived and even a pointless managerial, bureaucratic, exercise.  Consider though the statement "I lead a high performing team".  And then ask "By what estimation do I believe that my team is high performing?".

### How to use these metrics
Firstly, I need to strongly emphasise that I'm a little bit wary of metrics because they can _easily be mis-used_.  These should be taken with a very large dose of context and also in combination with each other, and also other metrics and observations that you may think, or be aware, of.  This is to say that it wouldn't be a good idea to take just one, or even three, of these metrics and to use them solely to determine the strength of your team.  That would be a mistake and almost certainly give you a poor estimation, either to the upside or the downside, of your team's performance. 

On the other hand, to attempt to track all these metrics suggested below, is itself probably unwise too.  It's probable that you already use, at least, a few of these metrics. But if you read the below and find some metrics that would be beneficial to your workplace, choose 2 or 3, and go from there.  The below is not a prescription, so please don't treat it as such.  Treating this as a prespription will likely cause more issues that you're currently experiencing :).  

Metrics are not the panacea of the determination of team success.  They are simply guides and points for consideration and should always be treated as such.  Simply saying that one is healthy because their heart rate is low at rest is most certainly not a sign of perfect health.  An economy with a very low rate of unemployment says nothing of productivity.  Likewise, metrics in software, of productivity say, are firstly, vague indicators, and secondly don't capture the full picture of team 'goodness'.

In addition, it's worth noting the importance of educating stakeholders on the appropriate use of these metrics. This educational effort should target the functions, departments, or groups that actively consume these metrics.  Metrics as "Information radiators" is the concept to pursue.  This is in stark contrast to utilising them as punitive tools to admonish teams with.

And lastly; many of these metrics aren't necessarily publishable on a dashboard as are, say, Key Services metrics.  The [Communication metrics](#communication), for example, aren't well suited to publication.  The [Project burndown](#project-burndown---daily-chart), however, is something that should be posted to the team and wider.  Consider your approach carefully through the lens of incentivasation - beware what you incentivise as you may just get what you're asking for.



## Features: Preparation and Completion

### Amount of Ready work: The beginning of the funnel

_Metric: How many weeks of ready work are in your backlog?  Approximately 2-4 weeks of ready work is good._

I very much like this metric because it is often a good indicator of healthy productivity, and that teams know what their immediate goals are.  Work not being deemed as Ready will be implemented less efficiently, and less accurately than otherwise.

Ready work means that a feature is understood by the development team such that they can implement it without guesswork; workflows and their nuances are understood, UX is ready, the requirements are understood, the use cases, the key Personas, and also the value of the feature. Ultimately it is up to the team to determine what ready means to them and negotiate this with the Product Owner/Manager while ensuring that the departmental goals and business strategy are honoured.  A useful question "Why is this piece of work useful to the client?" can help to uncover work readiness.

>Productivity is downstream of work readiness.

>Quality is downstream of work readiness.

If a team exhibits low productivity, it is advisable to look first at the 'the beginning of the funnel'.  This is a rule of thumb I will employ often.  The same stands true for quality.  Remember, not all teams are the same; some deal well with the uncertainty of 'less-ready' work, but many definitely do not.  This is why 'ready' should be negotiated on a per-team basis.

Can you begin work that is not well understood?  Yes, you can.  Although typically unintentional, this is a very common approach.  The down-side of this is that it will likely increase your development time.  This is not an invitation to step back to waterfall development, but it is an invitation to ensure that you and your team understand the intention, the scope, the requirements, of your feature increment before you get your tools out and start building.

But how much ready work is necessary?  Just enough - enough so that the team know that they can progress on to the _next set of work-items_ and have a quick conversation to clarify some fine-grained detail, and then begin the implementation in ernest.  Work items further out on the scheduling timeline don't need to be, and shouldn't be, super-refined.  Think of Work Readiness as a narrowing scope where the nearer the scheduled work item gets to the current iteration, the more refined it should be.  Having all items in a backlog ready is not much better than zero items in the backlog ready; the problem is different, but both cases cause great innefficiencies and delays.

If you have no items in your current iteration that are deemed ready, your immediate job should be to ensure that these items are ready.  It is likely that this is the most important and useful thing that can be done to ensure productivity and accuracy. 

How ready are your teams?  Count the total items in the current iteration and determine which of these items are/were Ready.  All items in the current iteration should be ready (although for teams that prefer, they could refine thier work on a weekly basis in order to keep the information more current and pertinent).  A further 2 weeks should be nearly ready and planned, and a further month or two should be scheduled, but not completely ready. 

<center>
<img src="./General images/RequirementsScopeOfUncertainty.png" width="60%" />

<em>The closer to being worked on, the more ready your work should be.  Agile is about making progress with imperfect information.  As the work gets closer, the less imperfect we expect the information.</em>
</center>

A word to the wise; don't expect perfection of Readiness; expect best effort. Questions regarding fine-tuning of requirements will always arise during implementation and this is OK.  However, if the team isn't aware of all the workflows that the feature will achieve, doesn't understand UX, doesn't understand architectural concerns yet, and the potential value of their work, then that item is probably not ready.


## Done Work: The end of the funnel

Good teams know when work is complete because they have a firm grasp of the requirements, and they also have a firm grasp of the testing necessary to ensure that the work is of sufficient quality.  They also have a solid process regarding check ins and branching policies, documentation, and publishing their work to the agreed environments.

For example, Done may mean: code is reviewed and merged from the feature branch into develop, implementation available and tested on Test Environment, all known issues are fixed (there are no known issues), sufficient automated tests written and passing, manual testing completed and passed, implementation marked as satisfactory by the end user representative, release notes written.


_Metric: Does your team have a common understanding of what Done means?_

_Metric: What percentage of your completed work needs no further steps or work to get it into the hands of the customer?_


## Delivery metrics

Strive for predicatability of delivery.  Teams that achieve a **predicatable cadence** such that each period they regularly deliver a **good volume of features** such that you can **plan out the near and medium term future**, are doing well. (A period is up to you to define and can be as granular as you want to make it).

### Predicatablity 
An easy key indicator, or measure, is found in your ability to plan the near future; can you predict with some confidence, a team's ability to deliver work in the future?  Are you able to meet key delivery dates?  Are you able to commit to specific implementations or integrations for your customers or 3rd party integrators? 

_Measure: Can you plan work with confidence into the near future?_ 

Okay, this isn't a metric per se, but this is a measure of confidence that could be charted on a 1 to 5 spectrum, where 1 is poor confidence and 5 is great confidence.  Every month chart this to give you a telling metric.

### Project burndown - daily chart
Large projects with firm deadlines are still a thing and often for good reason.  Similar to a scrum sprint burndown, or a release burndown, I like and prefer, a burndown for the entire project.  This indicates (indicate is the operative word) the amount of work remaining to be completed at a given date.  And this tally of amount of work remaining is tallied at a regular interval; every week, or every day for example.

<center>
<img src="./General images/ProjectBurndown.drawio.png" />
</center>

Tracked over time, this can be helpful for numerious reasons, but the major one is to indicate the likelihood of meeting the delivery date. 
Burndowns are useful because they can raise confidence, or otherwise, of realistic delivery dates.  Of scope uncertainty.  Of productivity also.

This is a key metric to share with the team and stakeholders to keep them informed.  

Some projects can last over a year and having information about how they are tracking is very useful; critical in fact.

Other useful metrics that are useful to include in burndowns are:
- scope change
- amount of work completed
- re-estimated work

The above diagram illustrates these metrics.  Scope change can be gleaned by considering the following: if there is no scope change in a project, there should be an equal drop in the amount of remaining work as there is an increase in the amount of closed work.  However, if you see that the amount of closed work is trending well, but the amount of remaining work to do is flat-lining or similar, this is very likely due to scope changes, unforseen work, re-estimations to the upside.  This is the case shown in the diagram where the "Closed" trajectory is not mirrored by the "Open" trajectory.

_Metric: How much work is remaining to complete in your current projects?_


### Quantity 

<center>
<img width="60%" src="./General images/QuantityWorkItemsPerPeriod.drawio.png" />
</center>

What is the count of features per period that you are delivering?  If you have varying sizes of feature implementations, you can always tally per category e.g., 1 large feature, 2 medium, and 5 small features, plus 8 bug fixes.  Consider tracking this as an accumulating metric alongside your project burndown(s).

### Consistency of Quantity 
To be predictable you don't necessarily need consistency of quantity of features, you need moreso reliability to deliver the project; this is because when there is a push to complete a project, this push results in an increase (usually) of work completed.  This necessarily breaks, and should break, the consistency pattern because you really do not want to push full steam all the time.  But having a measure of consistency helps you to understand what you can deliver in a given situation.

<center>
<img width="60%" src="./General images/QuantityConsistencyWorkItemsPerPeriod.drawio.png" />
</center>

Are you delivering a consistent number of features each release cycle?  There may be many different reasons for not doing so, such as inconsistent feature sizing, such as an insufficient pipeline of work that is not ready for implementation, such as team capability and capacity, but if you can tally the number of delivered features as per above, and do so over a period of time, you have a nice illuminating metric.

I'll repeat that I'm uncertain if consistency of production is the goal.  It is the metric itself that is useful.  I'll leave it to the reader to muse on the virtues of consistency, or otherwise.

_Metric: Quantity over time._
<br/>
_Measure: Categorise and tally work items that a team works on broken into small, medium, or large chunks._ 


### Size variation
_Measure: How consistently sized are the work items in a typical iteration?_ 
<center>
<img width="60%" src="./General images/SizeVariationWorkItemsPerPeriod.drawio.png" />
</center>

I'm in favor of small work items with little variation in size, when possible.  This allows for more predictability, ability to get the work 'Ready',  a higher 'completion rate' and feeling of productivity, better quality through better testability, and of course, better _predictability_.  It also probably means that the team has enough understanding of the work to create a small enough work item.  There are downsides, such as managing of work items is more cumbersome, difficult to see the forest for the trees, and a sense of 'false-decomposition', but these can be mitigated by well-intending, eager teams, tools such as storymapping, associating work items with high-level epics, and a keen constant eye on the backlog.

_Metric: What is the size variation of your work items?  The **average** will tell you the sizing over a group of workitems, and **standard deviation** will tell you how highly spread around the average the work items are.  You want a low spread; a low standard deviation._

### DevOps
Remember that the following metrics are intended to be indicators of high performing teams, and not necessarily of a good, healthy DevOps process; although the two conceptual domains overlap significantly.

#### Commit activity
Over a period, this is a short cut indicator towards developer productivity.  Look for and encourage short sharp, small, and constant commits.  These are indicative of a pragmatic, process oriented team.


#### Automated tests
Failing unit, integration and UI tests are an important indicator and metric, and should always be treated seriously and fixed, disabled, or deleted (reserve deletion for redundant tests), as soon as possible.

_Metric: What is the code coverage for your products?_<br/>
_Metric: Are there tests failing today, and if so,which ones?  How many?_<br/>
_Metric: How many days have these tests been failing for?_<br/>

Another metric related to automated tests is the _time of the team to react to a broken test_.  It may not be the case that all your automated tests form part of the CI pipeline that forces all tests to pass in order to deploy the build to an environment.  Some automated tests, especially ones that require some time to run, sit outside CI and run asynchronously.  These ones can be left unfixed for some time where teams are either unaware, or not correctly incentivised.  The behaviour of jumping on to a failure immediately is a positive indicator.

_Metric: Time to react of a failing automated test?_


#### Environmental efficiency - Time to production
How long does it take to push a fix or feature to production?  Ideally this should be minutes, but it is still not uncommon to hear about environment gateways (think traditional Ops), configurations, environment health, build queues, testing cycles, social policies, that make pushing to production a far lengthier process.

How does this affect team performance?  If the team can't push changes to an environment without waiting hours for a build queue to complete (this used to happen especially in legacy systems), for example, they are impeded by a significant bottleneck whose downstream effects are very significant.  Simply put, a slow push to prod is just very difficult and time consuming to work around. Quality often suffers greatly as a result.

_Metric: How many minutes, or hours, or days between code commit and a push to production does it take your team?_

#### Release cadence
How frequently do you release to production?  While this is still a relevant metric for Continuous Delivery shops, it is more applicable to more traditional organisations. Release frequency is related to quality and a sense of timeliness and focus for a team.  It may very well be that end user agreements/contracts or preferences do not allow for continously changing software to be delivered every week or month.  However, goals of internal release to staging can avoid the problems that are associated with releasing very large chunks of work over long periods of time.  Without delving too deeply here, one of the most significant problems with releasing infrequently is that quality suffers; often greatly.  There is just too much to test in one regression test.  Again, this can be mitigated with the use of internally, more frequent, delivery targets.

_Metric: How frequently do you release your software?_

#### Release punctuality

_Metric: Release punctuality days = Release date - Intended release date_

Your target for Release Punctuality days is zero.

If your release puntuality is a significant issue, and your Intended release date does not follow a regular cadence, one month per release for example, then your first step should be to agree on and target a reasonable cadence of release, if possible.  Irregular release cadence can be a significant contributor to missed release dates.  This is because hitting a release date is a behaviour learned; and it is worth learning this behaviour before progressing on to more ambitious ways of working.

A resistance for more ambitious release dates, say, even monthly (although some may find this target amusing, many organisations regard this as reasonble, and even hard to achieve) is justified commonly by the exucse of 'insuffient time to build a set of features'.  Another excuse is that 'lengthy and onorous regression cycles' are too cumbersome.  Interestingly, some teams resist due to the belief that more time is needed to ensure a quality release. Fortunately, there exists a robust positive correlation between a regular and timely release cadence and release quality. Frequent releases facilitate constant testing and reduce code churn per release, leading to improved overall quality.  A discussion on this topic with your peers will often end up with an understanding that greater investment in automated tests and more investment in deployment environments that are conducive to reliable testing (recreatable, emulative of production) is necessary.


#### Regression test cycle time
It's not uncommon to observe regression test cycles lasting for several days, extending to over a week or more. This prolonged duration is often a compounded result of low *Environmental Efficiency* (as explained earlier).

A protracted regression test cycle is not indicative of a high performing team. Several factors contribute to this, including the likelihood that developers are committing untested code and features while regression testing is ongoing. Also, bugs identified and then fixed during the regression cycle may not undergo thorough testing. Additionally, an extended regression test cycle points to inadequacies in the breadth, robustness, or trustworthiness of automated tests, and likely a complete lack of performance tests. Notably, the risk of human error during regression testing increases with the duration of the cycle. For a large product, I like to target the maximum time of one half day for one person for a manual regression test cycle.

_Metric: What is the duration of the regression test cycle for your product(s)?_


### Process and Bottlenecks

Work items stuck and piled up in the testing column is a good metric to monitor.  And that goes for workitems piling up in any column. The (all but contrived) illustration below illustrates a bottleneck in the Sign-off column, for example. Questions to ask could be:

  - Throughput: How many days from starting to Done do items stay in each process column? 
  - How many items vs team members are in Progress at any point in time?
  - How often does this pattern occur?  Is this a one-off, or does this occur every iteration?


There are good ways to remedy this, but we'll leave that out of the scope of this article, but as a quick pointer, [a read of basic Kanban principles](https://www.qwant.com/?q=kanban+wip) will take you a long way.

<center>
<img src="./General images/scrum.png" width="60%" />
</center>

    
### Quality, Reliability, and Confidence 
How solid are the features that you have delivered?  

#### Bug count
How many bugs have been identified since your push to production? (Continuous Delivery shops may want a tally of all recorded bugs instead here, or bugs recorded per week, or per month for example). How many bugs are picked up during the testing phase?

#### Bug severity
What is the nature of these bugs?  How crictical are they? A count of critical bugs above zero is cause for action. 

#### Speed of response
If an urgent bug is broadcast and it is immediately jumped on, you know that you're on to a good thing.  If the bug languashes and it needs to be followed up multiple times, a team meeting needs to be set up regarding its priority, hmmmm... well, you know... _Time to first response i.e., from initial broadcast of an important bug is a good measure._

#### Rollbacks and fixes
How often do you need to patch fix?  How often do you need to roll back a change?  

#### How many Support Tickets have been raised against a specific feature/release?  
These are important metrics and are useful to contrast against the Quantity metric as well as the [Readiness metrics above](#amount-of-ready-work-the-beginning-of-the-funnel).  A high Quantity metric indicating a large volume of features that is coupled together with a low Quality metric (I mean that you have a large volume of bugs per feature) is not great, but it beats a low Quantity _and_ low Quality metric.

<center>
<img src="./General images/QualitySpeedMatrix.png" width="60%" />
</center>

#### Helpdesk sentiment
Lots of bugs in a just-released product, time after time, will cause helpdesk to begin fearing your releases. Helpdesk's confidence in your release is a great measure, but if you need an actual metric, look for _"number of support tickets raised as a consequence of the release"_, and then map these tickets raised over time.

Another metric is to map this helpdesk sentiment over time. 1 - very positive ---  5 - very negative. 

#### Helpdesk staff scheduling
Are helpdesk scheduling staff each release cycle to cope with the incoming calls?  Or are they feeling easy and happy about the new features?  _Support tickets raised by Helpdesk (that relate to the new release) plotted over time_ are a good measure for this (just as is a good conversation with Helpdesk/Support staff).

#### Release confidence and staff scheduling
A warning sign is when an abundance of the development team are allocated on-call during a release to production in an effort to counter the onslaught of potential bugs that will arise.  By all means, you should stand vigilant, but beware if your confidence in the quality of your environments and releases causes you to fret and stand-by an innordinate number of your development team as a mitigation exercise to poor quality.  

_Metric: number of issues found in production within 5 days of a release cycle should work here_.  Reducing this to zero would be a goal.  
_Metric: number of staff on-call for a release deployment._    

## Communication  
Communication within and between teams is vital.  Between roles and seniority levels.  During planning, problem solving, solutioning, design.  This isn't a comprehesive coverage of communication metrics, but simply things that I've considered and looked at in the past.

### General comms metrics

#### Whiteboard design 
When involved concepts need to be discussed; involved designs, resolving difficult bugs, educating about business logic or existing architectures, do people in the team migrate towards a whiteboard, pick up a pen (or mouse) and share scribbles?  This is typically something I promote and like to see happen often because it generally leads to quicker outcomes.

_Metric: How often do people gather around a whiteboard?  Never? Not good.  I can't think of an actual number here, but I'm tempted to say once for each major feature._

It would be useful to determine a corresponding metric and communication medium for remote teams.  I don't have one yet.  I'm tempted to equate virtual whiteboards with physical ones, but I can't say (I don't know) that these are indicative of the same behaviour pattern.

#### Distraction balance
To me, it is good to see a hive of activity; busy pairs of people sitting at a computer to solve a problem, groups of people in a meeting room for 10 minutes to confirm a nuanced solution.  This is probably a contraversial one, but the measure that I look for is going from a quiet environment to one where a pin could be heard dropping, people interact seldomly in the office, and if they do, using online chat tools, to one where I begin to get people murmoring about the office being a bit noisy and that they are finding it difficult to get thier own work done.  I then tend to adjust and wind the interaction dial back slightly to 'a couple of notches' below that threshold.

_Metric: How many times a week do people ask for help or gather to help someone?  Every time they write a line of code 'aint great either.  Take the metric as an observational count (don't get people to record this for you because that's just silly) and compare week for week what the level of interaction is._


#### Peer programming
One of the most productive (and fun) teams that I was involved with had two of the developers almost exclusively peer programming.  Both were talented seniors, but their mix of skillsets and approaches, and willingness to collaborate meant that they were able to achieve more together. Most people that I talk to about this topic treat it with smiling skepticism, but doing this well and doing this correctly can be a great weapon.  I understand that this is not for everyone, but people do need to be able to, at least time-to-time, share a desktop and a keyboard and solve a problem together.

A side-note here; I would promote and drive the peer programming concept when a team member stubbornly insists, day after day, that they don't need help even though it's clear that they do.  It's a good form of collaboration, and performed well can be a wonderful learning exercise.

_Metric: How often do people sit together to code a solution?  0 : it is worth promoting peer programming as a tool for the right occassion._


### Meetings
Meetings are structured and organised gatherings of people to exhange an idea and reach an outcome.  Another definition of meetings is that they are a time-efficient alternative to individuals taking their own route to what is otherwise the end-result.  They are very useful tools, but it is unfortunate that this is not always the case with meetings.

#### Length, frequency and purpose
Short and sharp, or long and circular?  I know which I prefer. We all know what painfull meetings look like.  There are several flavours of bad meeting, but you know it's bad when you hear yourself utterring "that's an hour of my life that I'll never be able to claim back".

As a side-note, the below are meant to be points of reflection, not meta-data that you should collect for each meeting every day. _Do not_ document every single meeting with regards to this meta-data; and don't task someone to do this for you (please).  Practically, perhaps choose a week or a two-week period.  Look at your calendar to remind yourself of the meetings that your teams have partaken in. Choose a couple of the below metrics e.g., How many meetings over-run the scheduled time?  And how many meetings fulfilled their intended purpose?  Spend 5 minutes to evaluate each meeting against these questions.    We're after useful indicators rather than precise measurement so that you can make adjustments to your meeting practices.

_Metric: How much time are teams involved in meetings during a typcial week?  Count the hours._

_Metric: How often is a meeting started by framing the expected outcome?_

_Metric: How many hour-long meetings are teams involved in during a typcial week?_  

_Metric: What is your default meeting duration?_

_Metric: How many meetings over-run their scheduled time?_

_Metric: How often do team members complain about not having enough time to do work for having to attend meetings?_

_Metric: How often do meetings not fulfill their intended purpose?_

_Metric: How many of the team members understand the purpose and the intended outcome of the meeting?_

_Metric: How often do you have a meeting to discuss the very same thing that you did a few weeks before?_


Meetings should have a purpose and an intended outcome.  These need to be stated at the beginning of the meeting.
Having a time constraint is a positive thing; not a negative.  Having not quite enough time is better than having too much time (usually).  People will work a bit harder and more deliberately to achieve an outcome.

The fault with most meetings is that they're too long, not too short.  So, it is worth attempting an experiment with scheduling shorter meetings.

Some good rules of thumb that I've found are;
 1) Don't be afraid of 15 minute meetings. 
 2) Two or three 30-minute meetings in a week can be a lot more effective than one lengthy 2 or 3-hour meeting.

<center>
<img src="./General images/MeetingTimes.png" width="60%">
</center>

Repetitive meeting topics going over the same ground can be partly remedied by documenting the meeting content and outcomes so that they can be referred to, by having a strong meeting facilitator who politely refers to the previous meeting notes, and also sticking to the meeting purpose.

#### Meeting Positivity
There is a vibe in positive meetings that can be measured in smiles per minute.  I'm joking. But we've all witnessed people who draw the energy out of the room. And we've all been part of positive meetings that are upbeat and productive without being contrived.  I don't take a metric here, but one I do often think of after a meeting is: 
    
_'How many questions were asked?'... I guess this is a metric of sorts..._  
    
Zero questions means that either everyone knew everything already, or they were being spoken at, or they couldn't wait to get out of the room/didn't want to entertain an answer to their question, or didn't feel comfortable asking the question.  Having some good quality questions that enhance understanding and even expose interesting and pertinent discussion are good questions, and are indicative of an interested, and culturally engaged group. 

## Softer team metrics
#### Team temperament (the imposter of triumph and disaster)
This is a measure of a team's reaction to events, both positive and negative.  It shouldn't be mistaken for a measurement of team happiness, but moreso one of maturity.  Temperament can tell you whether a team is able to handle bad or good news, take the news in their stride, consider it, adjust, and then keep moving forward.  A highly oscillating temperament is not good. Over the top reactions are a sign of an immature team and can be an indicator of a leadership problem.  Regardless, the metric here is hard to define exactly, but can be graphed over time with respect to key events and the team's reaction to both positive and negative events: 
    - name the events over time and,
    - out of a scale of 2 to -2 rate the team's reaction.  Better yet, get the team to evaluate themselves. 
    - 2s indicate a strong emotional reaction, 
    - 1s a light emotional reaction, and 
    - 0, none.  
    
Annecdotally, I performed this exercise recently with my 10 year old favorite girl to highlight that some of her reactions were, shall we say, a little over the top.

Generally speaking, avoiding 2s is beneficial.  This contrived example below is interesting in that it shows a strong reaction to negative events.  What to do about this?  I apologise, but that's an involved topic for another discussion.

<center>
<img width=60% src="./General images/TeamTemperament.png">

<em>This team exhibits a strong negative temperament.</em>
</center>


 #### Attrition of people 
 How often do people leave your team/organisation and what are their reasons for leaving the team.  Is there a team that people don't typically want to work in and why is that?  A timeline of people leaving, the team that they have left, and the main reason for leaving can be quite revealing, especially within a large department, and drawn over a lengthy period of time.


#### Team Flex, Eagerness and Embracing change 
This may be a controversial measure, but I will often move people to form new teams, or join an existing team, in order to experiment with the balance of right people to get the job done.  Personalities, experience, eagerness, need for change, accuracy, mindset and attitude, speed, are some of the reasons that it is worth tinkering.  The measure isn't how often, but rather, how accepting are people of this movement?  Looking back at the past, it is one reasons that we've had some success in large project delivery; where teams could be flexed, shaped and changed.  If the culture is healthy, then this kind of thing isn't a big deal but moreso becomes a way that people feel they add real value as their strengths are harnessed.  Notwithstanding the downsides of this approach, I've found this kind of movement a weapon of a high-functioning software development workshop.



 #### Leadership and Positive resistance
  How many leaders exist in a team and how do they manifest themselves as leaders?  Does each team leader inspire confidence in you such that; you can have a difficult conversation with them?  Do they accurately and transparently reflect the remaining work and do they have a strong commitment to get the job done well?  Do they forsee issues with accuracy and talk about these?  Do leaders push back positively to you?  Do they push back in a way that helps you adjust your course of action? 

If you look at your entire software development department, or even within a team, do you see many leaders, not just team leads, but leaders in different areas; cultural, quality, architecture, domain expertise, product experts, problem solving leaders, etc; people who are listened to and respected, people whose sphere of influence spans across teams and departments?  How many of these people exist in your team, or team of teams?  If your answer is very few, then this is something to work on:
- your culture may be problematic; and not resulting in the kind of environment that encourages  people to grow or share these talents. 
- there is a lack of experience and confidence in your team

_Metric: List your leaders and what function they fulfill.  What is the ratio of leaders to total number of people in your team?_

What constitutes a good number of leaders? I don't have a great answer without getting into some detail with regard culture, but consider the following:
1) each development team needs at least one strong leader, 
2) as well as a backup leader. 
3) it is good to think of good Product Owners, Architects, UX desigeners, Test leads, as good, influential, leaders.

So, as a rule of thumb, having a good team lead, and a good backup leader in that team, and also if you have good leaders across your major disciples eg., Engineering, Domain expertise, Architecture, UX, Product, you should be in a reasonable position.

And lastly:
_Do you have a person that could replace you in your role?_

#### Greater than the sum of its parts and masking of weaknesses
 An important indicator that I see emerge out of good teams is how often team members cover for each others' weaknesses, such that the team rarely exposes these weaknesses.  This is a good sign of a great team culture.  It is difficult to measure, I'm sorry, but can be identified during standups and interaction between members offerring to help one another on specific tasks, sometimes stepping outside their own roles to offer advice or help.

It's great to see when a team member suggests to another, in a selfless fashion, that they'll work with that person to peer program this next diffcult part.

Imagine the opposite situation whereby nobody in the team is covering, whether purposefully or not, for anyone else.  Teams end up working as individuals, rather than collectively.  Each weakness is exposed.

You can simply take note of when these actions occur.  Purposely tallying and publicising this kind of information seems to gamify it to the point of meaninglessness, unfortunately, and I would stay away from that temptation.

#### End user empathy
This is one of the last metrics in this artcile, but it very well could be one of the first in terms of importance:

How involved are your teams with the end user?  Do they talk to customers?  How often?  How engaged are they?

Dissassociated teams from the end user are unlikely to understand the user's real desires.  They are unlikely to empathise with the end user's frustrations.  And they are less likely to be committed to urgency of delivery and a quality customer outcome.

_Metric: How often do your team members talk to customers over a given period?_


### Control and Protectionism

<!-- Undoubtedly the better teams that I've witnessed have a mix of specialists and generalists; whether in the technology stack, or the domain. 

The greater autonomy a team has, generally the better.  Although this notion of autonomy should not be mistaken for no direction.  Direction and autonomy are not mutually exlusive terms. -->

Control, in softare development teams, often comes in the form of protectionism.  Protectionism is exhibited by team members who 'own' areas of work such that no one else typically contributes to it.  An example is the developer who works on an area, noted for its complexity of design and/or domain complexity, and when other members of the team attempt to work in that area, the controller may say:

- oh no, you don't know enough to make changes there
- just leave that to me, I'll get it done faster
- it's too complicated
- the rest of the team doesn't know enough/ have the necessary skills to make changes

and the rest of the team may utter something like:
- only 'Bob' understands that area
- I've never worked in that area
- I just don't understand that area
- we'll need to wait until 'Bob' is free

and interestingly, the controller may also complain about the fact that:
- developers are not capable of making changes in the protected area
- developer throughput is slow and unreliable and of low quality
- the controller themselves is bottlnecked and unable to do their job for the many questions they are asked and so very many jobs they have to do

Consequentially, the odd metric that falls out of this 'controlling' behaviour is either idle developers, or developers not working on priority areas of work:

_Metric: How often are developers idle or working on non-priority areas of work for waiting for the 'controller' to finish?_

Of course, there are other reasons that people may be working on non-priority areas of work, and these are worth investigating; side-requests from other departments, pet-projects, stealth-ops, disengaged developers, etc.

Other exhibitions of control are the command/control ways of working.  This typically manifests as an experienced developer/technical lead who breaks out tasks for a work item and then assigns people to each task.  These task breakdowns can go rather deep and result in large overhead for the technical lead to research, disseminate, and then monitor the tasks.  Not that these ways are outrightly bad; they have thier place.  But they certainly do not scale well, and certainly don't promote teams that are able to problem solve problems in an innovative manner.  This command and control practice is the antithesis to autonomy. 

_Metric: How many of the workitem tasks that a team are working are set and administered by a central lead figure?_


# Conclusion

I've not used metrics to understand how much the team cares about the customer, about the pride they take in their work and the products that they work on.  This would be an interesting exercise, but I can imagine that it would be something like a function of some of the metrics discussed in this article.

>    "Facts are stubborn, but statistics are more pliable."  ~ Mark Twain

Keep this quote in mind.  Your preparation and use of metrics can easily turn into a misuse of these very metrics.  With firmness of conviction, persistence, and an educational stance of interpreting the metrics, you can avoid this misuse. In the past, ascertaining and evaluating these metrics has constituted more work than I care to admit.

I apologise for the length of this article.  "I'm sorry I didn't write less but I ran out of time".  I'm curious as to what metrics you have used in the past; please elaborate on your own thoughts either directly (andreas.kacofegitis@gmail.com) or post below.  The art here is not to know what to do, but also when and how you do it.  Instrumenting change is a fun and exciting challenge, but it's probably best to change a little at a time.  Good luck.




# Appendix
## What is a High Performing team?

The definition of High Performance team is a team that has a high level of productivity and resilience.

Achieving Results: The primary characteristic of a high-performing team is its ability to deliver tangible and measurable results that align with the organisation's goals and objectives. These results often surpass expectations and reflect the team's effectiveness.

Efficiency and Productivity: High-performing teams are known for their efficiency and productivity. They accomplish tasks in a timely manner without sacrificing quality. The team's output is consistently high, and members work together seamlessly to optimize their workflow.

Predictable Delivery: Teams are capable of understanding the value, the complexity and challenges, the risks, and the effort that is necessary to complete a project of work.  They are capable of asking good questions to uncover information that leads to the project's success, and of advising an appropriate strategy for success. 

Adaptable, Well practiced and Dynamic: High-performing teams are able to handle unfamiliar tasks with confidence, curiosity, and fervour.  They have the breadth of experience and are practiced in the patterns of both success and failure such that they are able to apply these patterns alongside their wisdom to achieve a successful result. High-performing teams are adaptable and can navigate challenges and changes effectively. They respond quickly to new information, shifting priorities, and unforeseen obstacles, maintaining a focus on achieving their goals despite external pressures.

Continuous Improvement: A commitment to continuous improvement is a hallmark of high-performing teams. They actively seek ways to enhance their processes, performance, and outcomes. Feedback is valued, and the team is open to making adjustments for better results.

Effective Communication: Communication is clear, open, and frequent within high-performing teams. Team members share information, ideas, and feedback openly. This effective communication ensures that everyone is on the same page and working towards common goals.

Collaboration and Teamwork: High-performing teams excel in collaboration. Members work together cohesively, leveraging each other's strengths and skills. There is a strong sense of unity, and individuals are willing to support one another to achieve shared objectives.

Leadership: Strong leadership is crucial for high-performance. Leaders within the team inspire, motivate, and guide members toward success. They provide direction, set clear expectations, and foster a positive team culture.

Commitment to Quality: High-performing teams prioritize quality in their work. They pay attention to detail, strive for excellence, and take pride in delivering high-quality outcomes. This commitment to quality sets them apart from average teams.

Innovation and Creativity: These teams are not afraid to think outside the box. They encourage innovative thinking and creativity, fostering an environment where new ideas are welcomed, and members feel empowered to explore unconventional solutions.

Positive Team Culture: A positive and supportive team culture is a key defining factor. High-performing teams value diversity, treat each other with respect, and create an inclusive environment where everyone feels valued and appreciated.
