# Project burndowns

Large projects with firm deadlines are not a thing of the past, and for good reasons. Being a customer with expectations does not mean that they, nor you, are at odds with the concept of agility. 

Agile software development is about ensuring that quality software is delivered while appreciating that you have imperfect information, and the way to get more information is to test your current build iteration with users to ensure that it is on track to the nirvana of satisfaction: it is about discovery and experimentation in practice, where the next thing built is tested to ensure that it is indeed fit for purpose.

Customers, just as our organisations, have constraints, be they financial, 3rd party contractual agreements, or perhaps simply a strong desire to ensure that value is shipped.  And that by a particular date, it may be necessary to deliver said value to our beloved customers.

One such project that I was involved in required delivery on a given date at pain of a death; or to use another unfortunate analogy, the lopping of heads of the business.  The scope was pretty much fixed although there was ability to negotiate on the implementation of the features required.

Also, the scope was impossibly huge. And as one does in these circumstances, one begins by taking the smallest bite of this largest of elephants.  This first bite involved creating, what was at the time, a reasonably innovative concept: a Daily Project burndown.

Everyone hated it.  Or at least became annoyed; for quite the number of reasons which are descibed below in the Behaviours section.  I perservered, and as you may very well guess, we feasted on the elephant in its entirety; we succeeded.


## What is a project burndown?

A project burndown indicates (indicate is the operative word) the amount of work remaining to be completed at a given date.  And this tally of amount of work remaining is aggregated at a regular interval; every week, or every day preferably.  



<center>
<img  src="../General images/ProjectBurndown.drawio.png" />
</center>

## Purpose
Tracked over time, this can be helpful for numerious reasons, but the major one is to indicate the likelihood of meeting the delivery date. 

Burndowns are useful because they can raise confidence, or otherwise, of realistic or unrealistic delivery dates.  Of scope uncertainty.  Of productivity also.

Some projects can last a long period of time and having information about how they are tracking is very useful; critical in fact.  As a developer I worked on a project that lasted 2 years and 9 months!  Having this type of burndown would have been insightful and helped us to ask, and answer, some tough questions.

Moreover, a project burndown is simply a tool.  This tool can expose areas that need attention.  It can identify stagnation of productivity early so that this issue can be remedied.  Conversely, it can identify that good progress is being made and the schedule is sound.

## Common objections
Each time I attempt to distribute a project burndown in an organisation, I meet similar objections.  From now on, I'll simply refer them to this document :).  And then of course proceed to wake them up and engage in a discourse not too disimilar to the following:

- _You can't do that because burndowns don't work!_

    What do you mean by 'burndowns don't work?'

- _You can't do that because not all of the stories are sized yet!_

    Yes, we should attempt to size them all then.  A quick round of [affinity estimation](https://www.techagilist.com/agile/scrum/affinity-estimation-agile-estimation-method/) is a _fast_ and surprisingly good approach to estimate multitudes of user stories.

- _You can't do that because not all of the stories are accurately sized._

    Yes, well firstly, it is the nature of sizing.  Sizing is purely an educated estimate.  Secondly, as we progress and learn more, our sizing for particular works will change and we will reflect that as necessary.  Do you know of any that aren't sized correctly?

- _Sizing is unreliable! Many of our stories sizes do not reflect the ability to get them finished within a particular amount of time._

    You are likely correct, and I experience this a lot also.  But what I can tell you is that, on average over a large sample set, there is an average accuracy to story sizes; this meaning that some are estimated larger, some smaller, and on balance, sizing does work out about right.

- You can't do that because we don't have all the work defined yet!

    Cool.  Let's get busy and do our best to define it and estimate it.

- _You can't do that because the exec and stakeholders won't like the information.  They think we're sure of what we need to deliver and that we know how big it is, and they've been told that it's smaller than this chart suggests._

    **Transparency is critical**.  No matter how much you think that you may feel uncomfortable revealing this information, you'll feel so very much worse in a month when the story is worse.  Let's do ourselves a favour and not go for a slide on the slippery slope of false promises.  If they know that we're under pressure, they'll possibly be more inclined to help in certain ways.

These are the common objections.

## Audience
The audience of the project burndown are numerous.  

**The development team.**  Primarily, I use it for the team members involved in the project.  They really do need an idea of how we are tracking towards the deadline.  In my experience, there are always team members who ask for the burndown on the occassion that I forgot to send it out; this always makes my day.

**Stakeholders, and management, exec** should also be privy to this information.  This is something that it useful to show at a project review.  And failing that I would include the chart in an email with an few sentences of explanation.

**3rd party integrators, Customers** It is useful that these groups know how your project is tracking so that they can adjust their expectations.  I understand that sharing a Project burndown with a customer may be considered contentious and challenging.  Of course, it is up to you to share or not to share this information.  However, if you decide not to share, consider that it is a sign of something wrong in either their and/or your organisation.

When presenting this type of chart to an audience, some explanation is necessary to ensure that the chart is understood.  Also, it is very useful to provide an explanation of the typical patterns that they may see in the burndown and may feel worried about.  [These patterns are covered later.](#patterns-to-expect)


## Useful metrics to include in the chart
Aside from remaining work, other useful metrics that are useful to include in burndowns are:
- Scope change
- Amount of work completed
- Re-estimated work
- Number of work items completed
- Number of work items remaining

The [above diagram illustrates these metrics](#what-is-a-project-burndown).  Scope change can be gleaned by considering the following: if there is no scope change in a project, there should be an equal drop in the amount of remaining work as there is an increase in the amount of closed work.  However, if you see that the amount of closed work is trending well, but the amount of remaining work to do is flat-lining or similar, this is very likely due to scope changes, unforseen work, re-estimations to the upside.  This is the case shown in the diagram where the "Closed" trajectory is not mirrored by the "Open" trajectory.


## Promote good behaviour
Why I really do like the burndown approach is because it puts pressure in the right areas; to estimate as best as we can, to prepare the work as best as we can, and to regulate scope as best as we can.  Sometimes agile seems to get mistaken for unpreparedness, or procrastination, or laziness even.  But agile is not this.  Agile in a fixed timeframe asks the question; given that you have the constraint of time, and you know what the requirements are (at least broadly), what product can you deliver within these constraints?  Iterate to the most basic working implementation first and then iterate towards better versions should further time and resource allow.




The behaviours that emerge often the following:
- more fervour to renegotiate elements of the iron triangle:
    - ascertain true scope and also to reduce scope,
    - a renegotiation of the timeframe
    - a negotiation on resource allocation

- looking seriously at minimal, lean implementations that fulfill the requirements, 
- streamlining testing, development, UX, Product processes, 
- a push to make environments for Test, Stage, and Production, more reliable 
- team culture improves dramatically; team members help each other as they strive to solve difficult problems together; forged in the heat of fire, as it were. 
- stakeholders, exec, and the team asking questions that challenge the scope and implementation.  When the burndown indicates that the project deadline is at risk, it is curious how rational everyone becomes to think of ways to keep the implementation lean; both technically, architecturally, and how stakeholders soon realise that what they thought was needed, is actually a 'nice to have'.
- keeps the team focused and avoids extra work being 'slotted in', or handed to the team.  The conversation becomes a self-fullfilling one; "If we add a new feature into the backlog, are you OK with the deadline for the project being extended?"

These are the apparent good behaviours that I often see.


1. **Renegotiation of Constraints:**
    - The burndown chart encourages teams to reevaluate the iron triangle—comprising scope, time, and resources.
    - Teams become more proactive in:
        - **Ascertaining true scope:** Understanding the actual work required.
        - **Reducing scope:** Identifying non-essential features.
        - **Renegotiating timeframes:** Adjusting deadlines based on progress.
        - **Resource allocation negotiation:** Ensuring optimal resource utilisation.
2. **Lean Implementations and Process:**
    - Burndown charts promote a focus on minimal, lean solutions, in order to complete an implemention within the timeframe.
    - Teams prioritise essential features over nice-to-haves.
    - Streamlining processes becomes a priority, leading to efficiency gains: testing, architectural, development, UX, product processes.

3. **Reliable Deployment Environments:**
    - The pressure of deadlines drives teams to create robust testing, development, and production environments that are quick and reliable:
        - **build:** build times and a focus to reduce them, 
        - **known state:** data and services in known states are important to ensure that testing is accurate and any software regressions are highlighted, 
        - **deployment time:** regular releases and fixes are hampered when deployments require an inoordinate time.
        - **deployment methods, CI:** reliable deployment practices are employed to substitute latent, unrepeatable, risk-burdened deployments. 



3. **Improved Team Culture:**
    - Team members support each other during challenging phases.
    - Collaborative Problem-Solving:
        - The intensity of problem-solving and shared problem-solving strengthens team bonds.
        - When the burndown indicates challenges, teams rally together; leaders emerge.
        - Collaborative problem-solving leads to creative solutions.
        - Team members learn from each other’s expertise.
    - Burndown charts make progress visible to the entire team.
    - Team members become accountable for their contributions.
    - Transparency encourages open communication and trust.
    
7. **Adaptive Decision-Making:**
    - As the burndown line fluctuates, teams adapt their strategies.
    - Decisions are based on real-time data rather than assumptions.
    - A certain ruthless of decision-making and practice emerges when it is clear that the chance of success is not possible under the current strategy.

4. **Inquisitive Stakeholders and Executives:**
    - As the burndown line shows signs of risk, stakeholders and executives become more inquisitive.
    - They question scope and implementation, seeking ways to keep the project lean.
    - “Nice-to-have” features are reevaluated in light of time constraints.
    - "Must have features" are evaluated as "nice-to-have" in certain circumstances.

4. **Focused Workload:**
    - The burndown chart discourages ad-hoc additions to the backlog.
    - Teams stay focused on existing tasks, avoiding distractions.
    - Conversations shift toward considering the impact of new features on the project timeline.
    - Focus on Value Delivery:
        - Teams prioritise tasks based on value to the end user.
        - The chart highlights essential work, minimizing distractions.
        - Delivering valuable features becomes the primary goal.

3. **Risk Mitigation:**
Early deviations from the ideal line signal potential risks.
Teams can address issues promptly.
Risks are identified before they escalate.


<!-- 7. Transparency and Accountability:
Burndown charts make progress visible to the entire team.
Team members become accountable for their contributions.
Transparency encourages open communication and trust. -->

Many of the points above leads one to ask: "Shouldn't this already be happening?  This is obviously the correct practice."  Well, it's often not the case that our expectations aren't properly set; what we thing we need and what we actually need are two different things.  There's nothing quite like the stark contrast of reality to bring this to our attention.


Remember, the burndown chart isn’t just about ticking off tasks—it’s a dynamic tool that guides teams toward delivering the right product backlog items at the right time. 🚀 .





## Patterns to expect

Patterns to expect resemble a roller coaster.  The below burndown is illustrative of many and a description of each step is as follows:


<center>
<img  src="../General images/burndownTest.drawio.png" />
</center>

1. On project kick off, there can be a fervour to determine scope and requirements.  One can experience a large scope increase in this phase.
2. There is typically a level off in the first couple of weeks as the scope settles and CI/CD piplelines are built, security and architectures are visited and delivered.
3. A drop in amount of work as the architectural and CI initial work is completed.  And the team begins to gain momentum in completing work.
4. An rise in the amount of work as it is realised that the requirements are deeper or broader than initially envisaged.
5. A typical consistent increase in the Closed amount of work.
6. The plateau period were 'productivity is flat-lining'.  Actually this is not the case as you can see where work is still being closed:
7. The closed amount of work is offset by the recently added amount of work.  This scope change may be increased due to re-estimation to the up-side of existing work.
8. A steadying, a drop, and then another incline.  Typically due to forgotten requirements or due to unforseen technical complexities; APIs don't work as expected, datasets aren't what were originally was envisaged: base assumptions have been broken.
9. A steady drop.  Most unknown work is now known. This means that there is little to no scope change.  And difficult technical challenges have largely been resolved.


## Consider story maps
Synchronising your work with a story map tool such as storiesonboard.com can be a very helpful way to track progress.  They provide a two dimensonal view of what is a typical one-dimensional backlog that is difficult to interpret.  Zooming out on a storymap can help to shed light on the overall progress of the project.

<center>
<img src="../General images/storymapView.png" width="500"/>
</center>

## Limitations
Project burndowns are not a panacea and not a weapon to beat people over the head with.

They can lead to :
- Shortcuts, sacrificing quality for speed.  An example is where  thorough unit testing for a critical module is skipped in favour of getting the job done quickly.  Another example is when technical shortcuts  where functionally the work is complete, however, architecural rules have been broken; in the interest of expediency,perhaps not accessing data from prescribed services and connecting straight to a database for example.

    At times, taking shortcuts can be an appropriate compromise, but will need time for remedy after delivery.  Left unnattended, they can quickly become an embedded anti-pattern.  Often this time is not given to a development team as they move on to the next burning fire.

    One remedy for this scenario is to ensure that a 'tech-debt' workitem is raised for the repair work that must ensue after delivery.

- Uncomfortable conversations; burndowns are quite revealing and fronting up to have a conversation about why there is little apparent progress, work hasn't been defined yet, work has been re-estimated to a greater value, is difficult and confronting.  One may feel that they are dissappointing stakeholders, or that they are losing their reputation.  But I must re-iterate that this step shouldn't be avoided.  And stakeholders should be involved to proactively in adjusting scope or expectations when necessary.

    To help with the uncomfortable conversation, in my experience, it is almost always the case that your honesty is appreciated.  Also make sure to do your best to explain the burndown and research why it has arrived in its current state.  This expresses the importance of having project reviews where all stakeholders are involved.

- High pressure on the project teams.  Teams can feel unduely and stressed to deliver. 

- Individuals held to account.  It can be uncomfortable for those involved in the team as it becomes more obvious that there is a bottleneck and that there the person or persons required to remove the bottleneck are obvious.  This needs to be managed appropriately to avoid fingerpointing and playing the ill-fated blame-game.  A developer for example, not being perceived as being productive, can be remedied by others supporting this person, sharing the problem, and working together as a team.



## Sprint and release burndowns
I've not found sprint burndowns particularly helpful to track progress.  Not that I haven't used them, but if you want to know how a sprint is tracking, simply stand back from the whiteboard, or zoom out the online sprint board and you'll soon have your answer.

## When not to use Project Burndowns
For small pieces of work, they seem to lose their value.  Around three months and over they can be valuable.

## Conclusion
Project burndowns, while not a magic bullet, can be a powerful tool for guiding teams towards successful project completion. By providing transparency and encouraging positive behaviors, they can help navigate the often-challenging terrain of large-scale, deadline-driven projects. This article provided a solid foundation for understanding burndowns and their potential benefits. For those ready to embrace the transparency and focus they offer, incorporating project burndowns into their project management toolkit can be a wise decision.

Remember, successful implementation depends on tailoring the approach to your specific project and audience. Experiment, adapt, and use burndowns as a conversation starter, not just a reporting tool. With an open mind and the right approach, project burndowns can help you deliver value on time and on budget, even when the journey seems like a rollercoaster.

