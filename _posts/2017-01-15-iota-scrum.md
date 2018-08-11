---
layout: post
title: IOTA - The Missing Artifact in SCRUM
date:  '2017-01-15T08:10:16+01:00'
tags:
- Essay
excerpt: A new approach that enables you to target revenue driving customer behaviour 
---
 In my implementation of Scrum over the last few years I have found a particular artifact to be helpful in focusing activities on what really matters. This is called the IOTA model and in this essay I discuss its use.

# Principles

## Increments
For a particular sprint, we agree with the product owner which items on the backlog are most important. But in the rough and tumble of real life projects, there are complexities, impurities and confusion.
+ It is not always clear for a single sprint whether what is produced will be useful, rather than just the next set if items in an aging backlog.
+ How do we focus our efforts in the sprint should we not be able to deliver everything we thought we could? Sometimes a sprint goal is used to give this some definition. But how do we define the sprint goal formally?
+ Since we wish to keep our product increments small, how do we ensure that the assembled sprints produce a product increment that is useful and produces actionable customer and team feedback for the next increment?

I use an approach to planning both a sprint goal and the broader product increment, called *IOTA*. An IOTA model is a distinct artifact that should be produced as part of both sprint and product increment planning.

## Perspectives
Consider the context within which we develop software, build cars, or pave roads. My experience in building cars and paving roads is limited, but the principles of scrum work equally well for any task. Any of these tasks occur in a context. A useful way of looking at this context is from two perspectives:

+ **Learning** - How are we able to learn from our environment to improve what we build and how we build it. The classic reference here is the work on [double loop learning](https://hbr.org/1977/09/double-loop-learning-in-organizations) from Chris Argyris, Donald Schon et al.

+ **Limits** - what are the natural boundaries or limits to our control? We cant control everything and knowing / hypothesizing the boundaries, as complexity theory tells us, is sometimes all we can do. Being clear about the kind of action those boundaries entail  is critical. A great reference here is the [Cynefin framework](https://hbr.org/2007/11/a-leaders-framework-for-decision-making) from Dave Snowden.

I define two  axes to represent the poles of these perspectives and use them to identify four distinct questions that every sprint must ask:

- Theory <--> Action : How we learn by forming theories and testing them in the world.

- Inside-Out View <--> Outside-In View: our relationship to the world outside, as an actor in it or as a receiver of feedback from it.  Or, in other words, the context we can control and the context we can't. Inside-Out refers to our ideas and actions in the world. Outside-In refers to our thoughts and actions in response to the world.

## Components
By combining these perspectives, as the diagram shows, we define the four questions.

![](/images/iota_new1.001.png)

### What do we need to know about our next increment?
1. Define our *Assumptions* about it.
2. *Decide* what to build and what capabilities / features / things we need to provide to our customers or users.
3. Design our own *Conditions* required to suport what we need to build / learn etc.
4. Discern what the reaction was from our users based on achievement of defined *targets*.

### More precise definitions:
1. Assumptions are constraints that we are unable to change within the period of the next sprint AND are important in shaping what we build.
2. Capabilities are the jobs / tasks that we want to enable our users to perform. Often, these are described as User Stories. They are things that the user can see or experience.
3. Conditions are the capabilities WE need to continuously improve the capabilities we deliver to our users.
4. Targets are a formal, measurable definition of what success looks like for the increment.

## The Two Product Principle
Notice that we identify two kinds of capability. Those we develop for ourselves and those we build for others. I formulate a principle that I refer to as 'The Two Product Principle':
**"You always ship twice. Every time you ship you incrementally improve your customer product AND your internal capability to produce that product.**

This idea is fundamental to the IOTA model. Every product increment needs to not only make better products but also invest in internal capability so that product improvement is actually possible.  This is the essence of Kaizen; creating a continuous flow of improvement between ourselves and those for whom we manufacture.

# Practise 
This is all pretty theoretical. Let's create a practical example and walk through each:

Let's say we are building a component of a bank website that helps you budget effectively. (This isnt a good statement of a product or sprint goal, and we will explain why and clean it up later.)  I like to call this kind of statement a **Product Hypothesis**. It is high level and makes the assumption that customers want to budget, but what *effective* budgeting means is still undefined. It is the start of a dialogue with the customer and the team. Whenever you say to yourself, "wouldnt it be cool if I could....." you are expressing a product hypothesis. The IOTA model helps us test these hypotheses in small increments.

From a scrum perspective, the following questions would be asked during sprint planning and the sprint planning process would produce not only a pruned product backlog,  sprint backlog but also a consise statement of why we are build what we are building.

## Assumptions
I have run this model hundreds of times and the question that most often comes up is, "Aren't your assumptions really contraints?" The answer is, "it depends". The purpose of this step is to unpack the ideas we have formed about the context in which we build and make those that have a meaningful impact on what we build explicit. We want to make tacit knowledge explicit so that we can interrogate it.  See [this article](https://hbr.org/2007/07/the-knowledge-creating-company) by Ikujiro Nonaka for a seminal coverage of this idea. Sometimes tacit knowledge will describe a contraint and sometimes hide an opportunity. Let's look at both in this context.

Compare these two assumptions:

+  We assume that bank customers want to budget effectively so as not to run out of money at month end.
+  We assume that bank customers budget to enable saving.

These are not necessarily contradictory. However, the first shapes our response to the customer need very differently from the second. The second has a clear product implication for a bank, being the sales of savings accounts, while the second has more to do with the short term management of money day to day.

Consider a more operational assumption.

+  Help with the budgeting functionality will not be supported by the call centre until next year.
This obviously shaopes what we build and is an example of something we cant change soon and certainly could be considered a constraint.

For this example, let's use assumptions 2,3.

## Capabilities

I like to classify capabilities into the following types:

1. Features - Things you build for your customer to see and interact with directly. 
2. Signals - Things you build to collect information on your customers' use of the features. 
3. Enablers  - Things you build that will result in direct customer benefit later but not this sprint. 
4. Delighters - Things you build just because they are cool, make the site different or fun. 

So what are we going to build? Capabilities are features that the user can see or experience. We pull the following items from the backlog...(not in user story format)

1. Feature : A user can visualise their monthly transactions graphically.
2. Feature: A user can categorize their monthly transactions according to type (e.g. amazon, starbucks etc.)

*When then perform the first of 3 CHECKS.*

### **Check 1: Context:**

+  Do any of our capabilities contradict our assumptions?
+  Are our assumptions comprehensively served by our capabilities?

The first thing that comes to mind is that savings acounts dont seem to be referred to directly in anything we plan to build. Perhaps we add the following capability to remedy this:

+ Feature: *A user can see how much they are saving each month and, if not, we make explicit the fact they are not saving anything.*

Since we cannot expect any help in the medium term from the call centre, let's make explicit that,

+ Feature: *A first time user of the site should find it intiuitive to use this functionality.*


## Conditions
We now have a simple set of requirements. They still need to be broken down in more detail. But how do we work on ourselves?

A useful question to ask is, *"If we had to deliver the agreed functionality and then improve it while also adding the same amount of new functionality next sprint, how would we prepare?"* In my view there is nothing more important that velocity of throughput for a development team. Increasing velocity is the best indicator of team morale, product owner relationship function etc. Therefore, conditions should always include some reference to improving velocity in the future.

I like to explain conditions using the following story. Imagine you are working on a production line like the great Charlie Chaplin in [Modern Times](https://youtu.be/DfGs2Y5WJ14). You are responsible for tightening bolts. This is your product. The speed at which you are able to tighten the bolts without chaos ensuing (watch the video!) is your *condition*. This is a great example because it also shows that just wanting faster production without investing in improved conditions will usually result in chaos.

Returning to our example, we identify the following ways in which we can improve our conditions:

+ In order to better understand the transaction types, we will invest in some analysis with the data warehouse team to identify those types that are most frequent.
+  We will co-locate the team so that we can collaborate better, do pair programming etc.
+  We will research visualization frameworks to pick the medium / long term framework for our work. (for this sprint, we will probably just use what we know already.)

Now we check again.

### **Check 2: Capability:**

+  Do our conditions scale our ability to develop new capabilities?
+  Do our conditions respond effectively to our assumptions?

We don't seem to be in bad shape here. A simple iteration through the capability and assumption lists though shows that again, we are focusing on our app and not the existing functionality. Do we need to prepare for integration with the savings account functionality? Perhaps, we add the following:
+ Obtain interface tests for the savings account creaiton process from the savings dev team.

## Targets
So what? Why are we building this and how do we know its worth it? See this [article](https://hbr.org/2007/12/is-it-real-can-we-win-is-it-worth-doing-managing-risk-and-reward-in-an-innovation-portfolio) on the "Real / Worth / Win" screen for good ideas. I use it for sprint goal evaluation as well as product increment shaping.

My perspective on these questions is heavily shaped by Eli Goldratt. A nice summary of his thinking, combined with that of Boyd ( of OODA loop fame) is to be found [here](http://www.dbrmfg.co.nz/Strategy%20Constraint%20Management%20Model.htm).

We ask the question, "If this [increment] is to be considered sucessful what results will it produce?" Often, we will get answers like, 'users like it.' or 'there are no escfaped defects.' The first is undefined and also frankly useless. Customers need to do more than like it, they need to BUY it. As to escaped defects... success is not the same as the absence of failure.

This brings to the surface two complex questions:
+ Does the sprint result have to be immediately known or can we evaluate the sprint's effectiveness after some time (e.g. two sprints later) ?
+ How is the sprint goal linked to the product goal?

A sprint goal *must* have a relationship to the overall product goal. A product goal must have a commercial definition. It is useful to break them down in the following way:

### *A Product Goal:*
A statement of the commercial purpose of the product. E.g. "Our budgeting product will convert 5% of our customers to additional savings accounts by end of year."

### *A Product Increment Goal:*
A statement of how the next release of functionality will contribute to the product goal. E.g. "Smart identification of customer spending behaviour will allow us to better suggest saving targets for customers. The 80% who currently do not open savings accounts on the app, will reduce by 5% in the next quarter."  A product goal can therefore be broken into a number of increment goals. In practise, product increments often have a number of goals. For instance, we might have a goal of greater stability of the platform as well as (hopefully) a commercial target to meet. While the commercial goal is the most important and we *could* say that the stability supports the customer use of the platform, it would be artificial to say that stability is a child goal to 'savings account conversion.' There is no shame in having technical goals. There is only shame in having no customer oriented revenue / growth goals. A product increment ALWAYS results in customer feedback which shapes the next product release. 

### *A Sprint Goal:*
A sprint goal is the must-have functionality that you deliver if all else fails. There is a problem here though. Product owners are apt to describe everything as must-have. But the realisation of a goal as it is described on a backlog is open to a great deal of choice in design and implementation. So beneath the view of the product owner lies choice. The sprint goal enables us to make this choice. 

But the sprint goal is not just a prospective control measure, allowing us to adjust our focus during the sprint. It is also a powerful check on the scoping of the sprint before we even start. To see this we differentiate between *two components* of the Sprint goal:

1. *A target is the formal and measurable expression of a sprint goal.*
2. *An hypothesis is the argument behind the sprint goal itself.*

YOU NEED BOTH. 

For our example, a sprint goal might provisionally be stated as,

1. Target - 50% of customers get to recomendation phase without dropping out. 
2. Hypothesis - If customers receive a recommendation afer being shown their spending patterns they are more likely to save and our savings account usage will grow.

Let's dive into the hypothesis...

## Hypotheses 

**Format: IF  [we do something] THEN [Customer / User does something] SO THAT [We achieve something]**

There are many things we want to do in a sprint. For instance, in this sprint we may be implementing a new messaging technology to integrate with the likely ancient banking backend. This is a legitimate  goal. It's not very customer focused and if we have too many of these internally focused goals before the product increment is released we will likely be solving problems we have rather than our customers. See this [article](_posts/2016-09-12-designing) on the sins of over designing without feedback.  But we will often be working on projects where it is very difficult to get customer feedback on interim releases. However, if every sprint could be a product increment, that is the ideal target we want to get to. This is a great goal to track and work on in the *Conditions*  section of the IOTA.

Defining a sprint goal in hypothesis format is useful for two reasons:

1. It forces us to determine what kind of feedback we need from this sprint in order to validate subsequent sprints. This feedback can be internal (e.g. our engineers can't get the hang of these Kafka events) or External (customers complained that the user interface was too complex since the last change). All of this feedback is important for future sprint planning. **If you're not going to actively seek out feedback every sprint, and use this feedback to update your backlog, you may as well use waterfall because you're going to release crap anyway.** You can quote me.
2. It creates a very clear causal link between what we build and what we want to achieve which allows us to interrogate the priority of what we are building in the sprint.  

To see the usefulness of this, we introduce the next check:

### **Check 3: Coherence:**

1. If we do *not* achieve our target what *capability* would we aim to change? If the answer to this question is not crystal clear then we need to likely update the capabilities, or add detail to them, because we are not building to the target. Or, we have to change the target. 
2. What do we build to validate our hypothesis? 

Almost every time I have run this model with real projects, there is a mismatch in the level of detail expressed in the target and the sprint backlog (capabilities). The key idea is that we want to have an understanding of priority in the sprint backlog at an appropriat elevel of detail to guide priority by the team during development. 

At first glance, it seems clear that in our capabilities we do not have anything that tracks where in the process a customer stops. This is an example of a Signal.  We need to add a signal - "Track where users bail out."

Also, In order to validate our hypothesis we need to show that when customers are shown savings opportunities they axctually take them. This is central to our whole product goal. If we find that customers, on being shown the saving opportunity, dont take it, what would we change in our build? We could add a capability to capture the reason for not taking up the offer and save this as a simple log. 

**The $6 million question is whether after all of this checking we can still achieve this in the sprint time allocated.** Often, when we apply this model, the first time we check we find so many things missing, so much vagueness in undersdtanding the goals that we need to iterate the model again. This usually results in a narrower more focused scope that really targets what we are trying to achieve with this increment. In my experience I have found it not uncommon to re-run this model 5 times with a team just starting out thinking this way. The process unfolds incredible discussions between the team and the product owner, resulting in learning on both sides. The clarity you receive will more than make up for the time spent and using the techniques referenced [here](https://github.com/dromologue/ContinuousTransformation/wiki/ROAR-Model) - called ROAR - are very time efficient. 

# Progress
Let's imagine that we can do the work described and the team is on board. Where did we get to. The updated diagram below shows a single concise summary of everything we will do this sprint at a useful level of detail for talking to all stakeholders. 

![](/images/iota_new1.002.png)

I hope that you find this model useful. It will create greater clarity about what matters across your entire team. Please let me know your experiences or contribute to the repo [here](https://github.com/dromologue/ContinuousTransformation). 


