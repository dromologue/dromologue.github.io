---
layout: post
title: The Lazy J Curve and How to Stop Over-Designing
date:  '2016-09-12T03:21:16+01:00'
tags:
- Essay
excerpt: An essay on how to actually define what a MVP is for large applications with extensive functionality required in order to just be 'viable'. 
---

In this article, I propose a way of thinking about how much design up front is necessary in large system implementations.
It is common cause in the agile community to talk about the need to avoid anticipating a final solution in all its detail. Instead, we are advised, we need to balance delivery with discovery — incrementally delivering features, making them available for feedback and being open to discovering what we were not expecting both in terms of the customer experience and the technical implementation.   
   
 However, many large systems — particularly those that require a large set of standard features in order to deliver a minimum viable product — need some non-trivial amount of design to occur before delivery to customers. How much is enough? I introduce a simple model called the Lazy J Curve to explain the behaviours behind traditional large project planning and then use this model to derive the dynamics behind ‘just enough’ planning and design for large projects.

## Large Projects and the Unknown
If I look back on large projects that I have been associated with and consider how much time is spent defining what is known versus what is anticipated I find an interesting pattern. When implementing a large banking program, such as a core bank replacement, much is known of what constitutes the minimum required for a bank to function. For instance, we need current accounts, savings accounts, perhaps some kind of lending both secured and unsecured. In mature industries, projects of this kind rely a great deal on the experience of practitioners to define the ‘current’ state.   
   
But I have also seen a great deal effort spent on anticipating the implications of those new ideas or technologies, now grafted onto the present model. To use a banking example once again, we obsess over how to adjust customer onboarding processes to take advantage of new channels, and we try to learn from disruptive payments methods to reduce the cost and increase the penetration of our payments products.   
   
For ease of exposition, let’s call the first group of known requirements, the Hump and the second group of anticipated requirements, the Tail.   
   
When we look back on a project that has these attributes it is often difficult to separate out the (elapsed) time spent on either the hump or the tail. But in talking to team members, their stories will inevitably be about the effort spent on the tail. We find that the work of documenting the hump proceeds in a (mostly) orderly manner and with a fairly well understood schedule. The best example of this is to be found in consulting companies that do this sort of thing for a living. Any senior consultant will likely have done half a dozen of these projects, efficiently documenting the basic processes required for (for instance) customer onboarding. 

The work in the tail is largely unknown before the project begins and as such the team discovers new and unexpected complexities that then require effort to sort through. Sometimes this might result in the idea being shelved and a less complex idea implemented. The process of deciding to abandon work in a large project has a high overhead in itself. In some cases, the complexities might be thought central to what is new and competitive about the product or proposition and thus is pursued doggedly.  
   
In both these cases, a great deal of time is spent in understanding what could go wrong or put the project deadline / cost etc. at risk. This entails efforts spent in further anticipating a range of options that have little basis in the experience of the project participants. Effort expended, I find, is far greater in the tail than in the hump. This may be diagrammed as shown below where the total area under the curve is effort:

![][image-1]

## The tail and the hump
As the diagram shows, we expend a great deal of effort on what we know to be important (to our customer) and what we know will result in failure (of the system). What the diagram only hints at though is the extent of the effort spent on anticipating what might be valuable to a customer and those areas of system function that might fail under certain circumstances. This case is represented by the tail, running off the page for as long as we let it. In my experience the tail is far longer than this scale shows.
The unknown and Priority
In an ‘ideal’ case, what should we focus on? The graph below shows a hypothetical (and largely arbitrary) line that may be used to separate the important OR likely to fail from the unimportant or not known to fail. Wherever this line lies in reality is a job for the economists. For our purposes, it is sufficient to posit that there is some partition of the total effort spent that adds more value than the other.

![][image-2]

## Investment Priority
We can think of effort spent above the line as being of higher priority than that below the line. The location of the line gives us a useful definition. The functionality entailed by the effort above the line may be thought of as a minimum viable product. In my experience, an MVP needs to capture enough of the basic requirements in the application’s domain to attract new users, but so much as to delay release while we tail-gaze.   
   
 We still have a problem though. How do we know that what we work on after delivering the MVP is worth the effort? Is it possible to avoid tail-gazing? Many projects seem to avoid this trap. How do they do it?
The Lazy J Curve
I propose that we can focus on priority and function such that we stay above our hypothetical line of value throughout a project, but it needs some outside guidance.

![][image-3]

## Lazy J Curve
The graph above is achieved by transforming the initial curve by placing it along a new x axis — the investment priority line. It shows some interesting properties.
+ The hump is defined as being before a point specified as the feedback inflection point. This is the point at which we begin to actively acquire feedback from running an MVP.
+ Before feedback, not all of the work we do is of uniform importance. I don’t want to pretend pseudo-science so the shape is illustrative only. However, it is clear that as we proceed towards what we think is good enough to release not all features are of equal importance.
+ Why does the curve trend upwards after the feedback point? The only input, after we have dealt with the known features, that will ensure we do not dip down below the investment line must be something that ensures we are expending effort on what is valuable. This is feedback. Feedback will be from customers on which features resonate and from operations on how the platform as a whole is performing.
+ What is intuitively attractive about this curve is that the long tail is consistent with agile experience. Your ability to stay profitable as you move into less familiar technical territory, driven by scale concerns, compliance and security etc., is balanced by your increased refinement on a product level of what your customer wants and needs.

I call the result, the ‘Lazy J curve’. Use it. 

[image-1]:	/images/j3.jpeg
[image-2]:	/images/j2.jpeg
[image-3]:	/images/j1.jpeg