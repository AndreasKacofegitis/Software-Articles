# Practical Metrics for Key Services and Software

Services and software are useless if they are not working as intended.  Actually, that's not quite true.  They're worse than useless.  Useless implies zero utility.  Worse than useless means that you are negatively affected by poorly functioning software or services.

What is the health of your key services, environmental infrastructure, and APIs?  How long would it take you to answer this question?  Honestly?

**Seconds** : skim this article and add to it to share your knowledge.

**Hours** : believe it or not, that's still not bad because it means that you know: 
1) which services are key, 
2) how and where to get the information,
3) that the data are reliable, 
4) and that you know how to measure system health.

You probably already know what needs to happen; it's just that you've prioritised other work.  Perhaps this article will help to re-focus you.

**Days+** : keep reading, you may learn something about where you should be heading.

## Behavior and mindset
There have been past situations where we realised the sporadic unavailability of services; not recognised as being sporadically unavailable until dynamic metrics were introduced to bring it to the attention of the development team.

Seeing this information is confronting and difficult.  But consider yourself fortunate that you now know and can do something about it.  Truly, this is a good way to look at things. You can now focus on resurrecting the service.  And you can work on finding a solution to it not going down again.

So, firstly be thankful that you know.

Secondly, strive to eradicate all the issues that are known.  Some issues will be critical, or nigh-critical and will need to be fixed immediately.  Fixing immediately versus fixing properly can often result in two different solutions.  Put this work on the backlog in accordance with your other priorities.

Thirdly, strive to meet any departure from a healthy metric with urgency and a positive understanding that you have avoided a great many users a great many annoyances.

### Fast feedback and happy customers

At one software development shop, I remember that we'd wired up a push notification system that sent a message to me, and two others, the development lead/architect, and the Product Owner, to notify us of any significant user issues with their mobile apps. The team was so responsive that upon recognising a user issue, they would call the affected individual, describe to them the problem, and then implement a fix and notify them of the deployment.  We had a lot of happy customers as we managed so often to turn a negative into a positive encounter.  How many times have you been called by a tech representative apologising for your inconvenience and managing an individual test build deployment for you? 

Our user base was a few thousand users and it may be reasonable for the skeptical types to question the scalability of this approach.  Don't take this as an instruction or a recommendation, but take from it the positive mindset and technical capabilities that the team had built to promote such mechanics and processes.


## Down-time events
Key services going down and not being available is critical and ultimately leads to user dissatisfaction, data corruption, and/or possibly broken SLAs (Service Level Agreements).  These are all bad.

_Metric: When did the service experience an outage?_

_Metric: How long did the service experience an outage?_

Create a table of these services and their relative information over time.


### Timeouts
Timeouts can be indicative of a poorly performing service.  Considerations such as CPU utilization, memory usage, data bandwidth/payload size, network connectivity, code efficiency, database query efficiency, poorly load-balanced services, and downstream service dependencies can all be factors. There are of course, more. Regardless, timeouts are frustrating and will usually result in a poor user experience.

Finding the source of the problem of a timeout can be a very complex exercise.

Importantly, it is useful to recognise that there are different ways timeouts can manifest and one must be curious to investigate even the seemingly innocuous timeout.

_Metric: When do these timeouts happen?  Date, Timestamp?_

_Metric: What is the duration of the timeouts?  How many seconds?_

### Total up-time as a percentage of the year
While these up-time metrics could be thought of as the opposite of the downtime metrics, the services that you may be interested in for both measures may not have a 100% correlation.

For example, your SLA may guarantee that you have four 9s uptime per annum for key nominated services.  These services need to have a recorded value against them of actual uptime so that you may take action if it is discovered that they are 'down'.  This value is of interest to you and of course your customers.

_Metric: For each key service, what is the total uptime in terms of percentage?_

_Metric: When and for how long were these services not operational?_


## Performance metrics for key services
Regardless of the service being available or not, your service being slow and sluggishly responsive can provide for a frustrating user experience, among many other untoward side-effects.
[TODO: Describe metrics expectations]

The following metrics are useful in their own right, but more so in correlation to each other.  Seeing patterns of behaviour requires information over time, both at the low-level and also at the high-level, and being able to dance and correlate metrics and information across all these.

Applications like Splunk and GreyLog are great for combining and parsing logs and metrics of different formats and pivoting to form views and correlations across time.

While these applications and metrics are exceptionally useful, what we're after here though, are individual key metrics that are indicators of good or bad performance that are worthy of further analysis, or commendation and congratulations to the development team.

### CPU load
Ideally, CPU load should stay below 80% to ensure smooth operation and prevent performance bottlenecks.

### Memory usage
Memory usage should stay under 70% to avoid paging and performance degradation.

### Performance Saturation
This metric reflects if your system is handling requests efficiently. Look for sudden spikes or sustained high values (above 80%) that might indicate bottlenecks.

### Queue lengths
Long queues (> 100 items) could suggest slow processing or overloaded services. Investigate further to identify the cause and optimize performance.

### Number of requests over time
Analyze traffic patterns to understand peak periods and adjust resources accordingly. Unexpected spikes might indicate anomalies or potential attacks.

### Trending requests and hits over time
Track changes in requests and hit patterns to identify emerging trends and potential issues before they impact performance.

### API response times
Aim for consistent and fast response times (ideally under 200ms). Slow responses can frustrate users and negatively impact conversion rates.


### Service warm up times
How long does it take for a service to go from cold to servicing a request and returning a response?  Is it dependent on other services and can these dependencies be graphed to determine bottlenecks in performance?

### API response times using parallelisation - saturation points
Analyze how response times change under increased load. Identify saturation points where performance begins to drop and optimize resources to handle higher concurrency.

## Usage metrics

### API endpoint usage metrics
Which endpoints are the most popular

### Data requests/API endpoint metrics


### Error rates
Keep track of the percentage of requests that end in errors. Aim for a low error rate (< 1%) to ensure service reliability and user satisfaction.
Raw numbers and percentage of requests that end up in Error.


## Page load times and site performance
Interactive load times are usually my preferred target here, and a secondary metric is to look at the complete page load time.  Interactive load times are what the user sees and measure the point to first interaction where the page appears to be functional but is still loading.

### Key Security incidents
Monitor and log significant security events, analyze their source and impact, and implement effective mitigation strategies.


### Vulnerability assessment scores
Regularly assess your systems for vulnerabilities and prioritize patching known security flaws to minimize attack risk.

## Deep dive on key services


### Key metric sources
Often metrics can be sourced from multiple measures; they are not just provided to you.  For example, you may have to troll through logs looking for patterns of behavior, or you may monitor queue lengths, error logging services, performance metrics can be attained through logs, etc.

[TODO: finish this off to show diversity of sources]

## Dashboards to drive minimal user disruption
Initially, I use a dashboard to display key services and information that, if in a bad state, warrants urgent investigation and a potential fix.  This can sound easy to achieve, but can be rather difficult to achieve; I've heard of more failed dashboards than successful ones.  "Oh we used to use a dashboard for key services and metrics, but we don't use it anymore." is a common uttering.

To make a dashboard pertinent and of high utility, the data needs to be accurate, simple, and the indicators must also be accurate. A dashboard that displays a number values, with each value on a background that displays as Green, Orange, or  Red.
- Red: critical/urgent, needs immediate attention and investigation 
- Orange: cause for concern, needs attention and investigation, but may not override other work
- Green: nothing to see here.

### Culmination of good metrics
The metrics discussed in this article can mostly be brought into a dashboard that illustrates environment health.  If you can use these metrics to drive a snapshot overview of whether your environments, APIs, key services, are healthy; then you are doing well.  Can you say that you are happy with the state of your key services at this point in time?  If you can't answer the question, how long will it take you to determine the answer?  Is this the most important system metric?

### Promote good behavior
Encourage a culture of immediate response to red alerts and continuous improvement of metrics. Celebrate achievements and share success stories to keep teams motivated.

### Avoid false positives and false negatives
False positives are inevitable, but unless they are fixed very quickly, the dashboard is destined to be thrown on to the 'we used to do that' bonfire.  You don't want a dashboard that displays Christmas tree light information; a number of metrics highlighted as red (critical/urgent) with the team deciding to not investigate the cause of these failures because they deem the metrics unreliable.

A good behavior is when a metric is displayed as red, the team _immediately_ jumps on to resolve the situation and ensure a green state.  Always.

Constrast the bad behavior where a metric is displayed as critical/urgent and the team ignores it because the metric is deemed unreliable and deemed as a false positive.

For a metric panel to turn red often requires a fine-tuning of the metric over time;  the question is "What is required to make the metric worthy of the development team's time to investigate it?"


So, if the metric is the state of a queue length, for example, you may set the metric to fire once it hits 1000 items on the queue.  Initially this seems like a decent value to you.  But you then discover that this queue length often reaches 1000+ items and is a false positive flag that your development team begin to ignore after a few times of investigating it.  This has down-stream effects of setting a behavior that eventually leads to team ignoring the dashboard alltogether.  So, therefore, if you carefully curate the metric to make it meaningful and accurate of its true state, red: critical/urgent, orange: struggling, green: nothing to see here.



Display on a monitor and choose up to 3 key data points, no more.  This can be hard to do as it is tempting to choose more metrics than fewer, but having more can send the key metric into obscurity.
