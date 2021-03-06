# trules
Lorum estum umen drafterubus...  

## The challenge

In many respects, the biggest challenge in creating a software solution is in understanding exactly what needs to be created. Business asks Development to build something, but there are often misunderstandings about what it is that Business wants. Business needs tools that help them to be very clear and precise about what they need. Development needs tools to help them understand and clarify what Business needs. Trules attempts to meet these tooling needs.  

Business needs flexible tooling to help them describe their needs clearly. They need to be able to capture their needs naturally, in whatever order they prefer.

> The order in which the detailed requirements are captured doesn't matter.  
> The completeness, precision and accuracy of the requirements is what matters.  

Business must be able to review and validate the details that they have captured at any time, and must be able to communicate their needs to Development. Development in turn must be able to review and ask for clarification about the details. Refinement of the Business needs is a collaborative process that isn't complete until both Business and Development are satisfied that the requirements are complete and precise.

* The tooling must allow Business to gather and refine requirements in an unstructured manner.
* The tooling must help Business validate requirements.
* The tooling must support clarifying requirements for Development.
* The tooling must support formal agreement (between Business and Development) of requirements.
* The tooling must support ***changing*** requirements after formal agreement.

That last bullet point is a killer of project deadlines, but it's essential. Business needs can change at any time, and those changes can invalidate the requirements that Business and Development agreed to. Understanding exactly what changed is essential, and tools are necessary to quickly reach that understanding.

## Event Condition Action

We feel that it's often natural to describe detailed Business Software requirements in terms of **Event**, **Condition** and **Action** statements. In response to each Event, Conditions are evaluated and Actions are performed.

> Something happens...  
> In response, something is done...  

An Order is Received.  
In response, the Order is Fulfilled (prepared, shipped and billed).

"Something happens" (an Order is Received) is an **Event**. Events happen. Events occur at points in time.  
  
The "something" that "is done" (an Order is Fulfilled) is an **Action**.  Actions change things. Actions start at a point in time and end at a point in time (the start of an Action and end of an Action are Events). Actions may be simple, or may contain many other Actions (Processes are a special form of Action).  

Events and Actions take place in a wider **Context**. The context is made up of the **data** and **objects** that influence **decisions** about what to do. The context is the **state** of "everything that matters" (the Ordered Items are in stock, the Customer's Credit is good, etc.).  

> How did you become aware that an event happened?  
> What do you do in response to the event?  

How "you become aware that an event happened" is **Event Detection**. Detection comes in two flavors - You are either **notified** that an event occured or you **recognize** that an event occured. Notification puts the onus on someone else to send the notification. Recognition puts the onus on you to spot the event - to recognize that the state has changed and the characteristics of the state that indicate the event has occured. **Rules** that evaluate the state of the context are used to **detect the occurence of events**.  

What "you do in response to the event" is **Event Handling**. Actions are performed when Events are detected. **Rules** that evaluate the state are used to **determine what to do** in response to an event. The response to an event is **conditional** - based on **rules** evaluated in the state of the context at the time the event is handled (there may be a lag between the time an event occurs, the time that it is detected, and the time that it is handled).  

## Events
* Ad Hoc Events
* Scheduled Events (Expected?) - Process Events
* Unusual, infrequent events  

Some events are expected (perhaps even scheduled) to occur within a specific timeframe. If these events do not occur when expected, actions may be initiated. Expected events are often associated with processes. As a process progresses it is expected that certain events will occur.

An expected event can occur sooner or later than expected.
Some events are planned for, but are considered to be exceptions to the norm. For example, when an Order is Placed it is possible that it will be Cancelled, but not expected.


## Conditions
### Objects (that make up the context)
#### Current State
#### History
### Rules (that evaluate the context)

## Actions (including Processes)

