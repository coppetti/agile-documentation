# Scrumban Ways of Working

Scrumban represents the best elements from Scrum and Kanban where the key concepts of a team  working together to complete work (Scrum) and the amount of work limited to an optimized amount (Kanban) are combined into a methodology for high throughput and visibility into the development process.

As with any methodology, every organization must continually review and adapt the process and make adjustments to improve their experience to find what works best for them. 

## Key Scrumban Terms
* Work Backlog – Equivalent to Scrum’s Product Backlog with minor differences for how 
Workitems are tracked.
* Workitem – The individual descriptions of functionality needed by the business that either
define enhancements or defects. In our ways of working, consider Work Items are User Stories/Epics
* Workline – The series of stages in the software development process that pull work from the 
Work Backlog and produce shippable business value.
* Stages – The common and discrete steps required to deliver software within an organization.

## Clear & Visible Stages of Execution
This concept is originally from Kanban and is a key differentiator from Scrum. The software 
development process is divided into discrete stages that are made very visible for anyone to see. This 
is known as the Workline (work + pipeline) and is represented in the real world by a Board showing 
the Workitems progressing with real, physical cards that can be moved around by the team 
members. 

## Pulling Work Based on Capacity & Limits
Pulling work according to capacity limits is also a key concept from Kanban. Each stage of the 
Workline has a limit to the number of Workitems that occupy each stage. This keeps the team 
members from working on too many things at once and eliminating waste by ensuring that one stage 
doesn’t produce more work than can be handled by a subsequent stage.

As Workitems are completed within a stage, they wait until the next stage has capacity to pull new 
items to be processed. This is true for all stages especially the first one where Workitems are pulled 
directly from the Work Backlog.

## Team Collaboration to Deliver Business Value
Within Scrumban, even though the discrete stages of software development are clearly identified by 
the Board and work is tracked through them, the entire team is expected to work together to complete 
Workitems. They may have specialized skills but they can all contribute to some degree and are expected 
to help out wherever they can when their capacity opens up. The team objective is to keep all stages of 
the Workline filled and Workitems progressing through them.

## Empirical Analysis to Improve
The concept of reviewing the development process and team performance is the same as with Scrum 
but in Scrumban the statistics kept on how Workitems transit the Workline are also analyzed to 
determine the optimal work in progress values used to control the flow of work.

## Getting Started

### Identifying Stages for the Software Development Processes
A visual representation of the development process is important so the first step is to identify the 
stages any work goes through from when the Developers start to when they finish. Theoretically 
there could be dozens of steps but if the Board has too many, it will look cluttered and Workitems 
will be constantly jumping stages within a day. It’s better to roll up many steps into discrete stages 
that may take a day or more to complete for each. 

### Creating the Kanban Board
The Kanban Board will be created in Jira with the following columns:

* Product Backlog
* To Do
* In Progress
* In Review
* Done
* Complete User Stories

Our workline has 2 different scenarios:
1. User Stories (Work Items)
2. Tasks

For User Stories, they start in the Product Backlog and, after all of its tasks met the Definition of Done, 
It must be placed on Completed User Stories.

For Tasks, they start on To Do, and after someone pick ups the task, it must have be placed on In Progress stage, after 
we met the acceptance criteria for it, open a pull request and place the task on In Review Stage. After reviewed and 
accepted (see Pull Request Guidelines), merge and place on Done.

### Defining the Initial Work-in-Progress (WIP) Limits
When you first start using Scrumban, the optimal WIP limits won’t be known. It’s not important to 
get the values perfect in the beginning because the best values will be more apparent after the team
has completed a number of Workitems and there are statistics available to review. A good way to 
start is to take the number of team members and divide by two. If the result is an odd number, round 
up. For example, a team of four would result in WIP values of two and a team of five would use three.
Apply the same number to all stages and see how that works out over time.

It may be a bit restrictive in starting projects where every team member needs to start doings tasks. In those cases
we could use WIP Limit = Team Members.

For experienced teams and contant evolving projects WIP Limit = 2 * Team Members.

### Kanban Card Contents
Kanban cards serve as a representation of the work items defined in the Work Backlog. They will not
have all the up-to-date information needed by the Developers and that’s not their purpose. They 
provide the team with a visual symbol of work and facilitate coordination between team members 
and status to the Product Owner.

The level of detail can vary but at a minimum, having a clear title representing the Workitem is good practice. 
Adding a unique  identifier will make it easier to look up the item in the Work Backlog for when the team needs 
additional details. 

A more detailed version, but still not a complete duplicate of what’s 
in the Work Backlog, might also include the Priority, User Story and space for recording statistics on 
the Workitem’s progression through the Workline (i.e. working hours). The dates can be filled in as the card moves 
between stages. The addition of the User Story provides the Developer with the context around the 
request as a reminder.

Whatever level of detail is included on a card, it is important to remember that it is not a substitute 
for the Workitem details found in the Work Backlog. The team should rely on the combination of the 
User Story and the Acceptance Criteria to ultimately define what should be created.

### Preparing the Work Backlog
The Work Backlog under Scrumban is basically the same as with Scrum. It is a collection of User 
Stories and Acceptance Criteria written and maintained by the Product Owner. These individual 
Workitems describe the business value desired.

To keep the collection organized, additional information is associated with each item:

* ID – A unique identifier (e.g. US#007) for easy searches and reference.
* Project – A label to group a set of work items together according to a theme or purpose.
* Title – A concise, action-oriented description of the business value desired.
* User Story – A description of who will benefit from the item, what exactly is 
wanted, and why it is wanted. The User Story provides the context behind the request and 
enables the Developers to understand the goal, and not just take orders.
* Acceptance Criteria – A list of the specific conditions required for the Workitem to be 
considered complete.
* Status – An indicator of the readiness of the Workitem, when it is being worked on, and the 
final disposition: to do, in progress, in review, done.

The key to having a useful Work Backlog is for the Product Owner to continually spend time 
“grooming” it. This includes adding new items, updating items, prioritizing, clarifying content and 
adapting to the needs of the Developers as he learns more about how they operate.

### Scope of a Workitem
Ideally the scope of an individual Workitem should be consistent with all other Workitems so that 
when the average throughput of the Workline is known, predicting when a particular item in the 
Work Backlog will be done is possible and somewhat accurate.

However, that’s not very likely as the scope of business needs can vary greatly. The Product Owner 
should make every attempt to break down business needs into the smallest possible size that still 
produces something that can be deployed or shipped and therefore provides value to the business. 

If the Product Owner is unsure about how to reduce the scope of a Workitem, then he can consult 
with the team during the Weekly Timeblock when they review upcoming items. They will be able to 
suggest how the item can be split along logical lines or execution steps to reduce the size and still 
deliver value.

## Establishing Reoccurring Meetings
Scrumban has only two standard meetings that provide the contact points necessary for the team to 
coordinate their activities (Daily Standup) and review their work (Weekly Timeblock).

### The Daily Standup (DSU)
The Daily Standup meeting is a concept borrowed from Scrum and serves the same purpose; to 
coordinate activities and identify impediments. A daily reoccurring meeting should be set up for 15-30 (fixed time)
minutes where the first half is focused on the team members updating everyone on what they did 
since the last meeting, what they intend to do before the next meeting, and any impediments that are 
blocking, or threaten to block progress on their work. The second half is for any 
discussions necessary to address questions or plan activities. The meeting should be held near the 
Board so discussions focus around work in progress and updates can be made publically. Ideally the 
meeting should occur early in the day, just after everyone has had a chance to get to work, reorient 
themselves, and think about what they’ll focus on.

### The Weekly Timeblock (WTB)
The Weekly Timeblock is a reoccurring meeting used for multiple purposes. It should be set up in the 
middle of the week (Wednesday are best) so as to avoid holidays and vacation days that typically 
occur at the beginning and end of each workweek.
Two to four hours is recommended and set to occur in the afternoon so any preparation work can be 
completed ahead of time. The team will use the time they need and leave the rest. Having a projector, 
screen, and ample whiteboard space will be conducive for any technical discussions and problem 
solving.

The first use of the Weekly Timeblock is for demonstrating any completed work. This is the time 
where Developers can show the Product Owner what was completed and get Acceptance. Completed 
work can be demonstrated outside of the meeting anytime but it is good for the team to have 
everyone witness the conclusion of work.

Once Workitems have been demonstrated, the team should reflect on how their development process 
is going, any tools they use, and review the data on how Workitems are flowing through the 
Workline. They should have frank discussions about any new innovation that should be reinforced or 
impediments to be overcome. Clear action items and their owners should be identified along with a 
target resolution date.

After the review of recent activity, the team should have a preview of upcoming Workitems the 
Product Owner is preparing. The Developers should seek to understand the intent of each item, 
asking questions and getting clarity so everyone is familiar with what’s needed. The Developers 
should also provide feedback on Workitem scope, structure, and the optimal execution order so the 
Product Owner can make any needed adjustments to content and priority.
