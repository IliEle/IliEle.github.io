---
title: "Applying Agile: A practical guide for health data scientists"
datePublished: "Sept 23"
minutes: 95
weight: 6
tags: [Agile, Data science]
imageRef: /images/kelly-sikkema--nz-GTuvyBw-unsplash.jpg
---
In the fast-evolving landscape of health data science, the implementation of Agile methodologies can empower data scientists to tackle complex healthcare challenges with adaptability and agility. 
This guide introduces the main concepts of the Agile software development methodology and provides practical steps (highlighted in red colour) on how to apply the Agile mindset and methodology to digital transformation projects. 


# Agile Software Development Methodology

Agile was first introduced in 2001 by a group of developers who realised that the traditional linear waterfall approach of developing software had one big pitfall - it doesn't accommodate changes in what needs to be build. 

## Iterative and incremental model
Traditional development methodologies, like for example the waterfall and Prince approaches, begin with gathering all the requirements that's needed to be developed, then proceed to complete all planning, all development, then testing and finally deploying and maintaining the new system or tool. 

Agile is breaking up this linear process and follows an **iterative and incremental model**. Agile teams breakdown complex problems to small chunks and iterate through short cycles of Planning - Development - Testing incrementally building on what has been produced and deployed in the previous cycle. Agile teams deliver **value** in the form of working software early on in the project lifecycle by focusing on producing a Minimum Viable Product (MVP) and then iterate and incrementally deliver further analysis or functionality. 

Agile also introduces multiple opportunities of **reflection** and gathering feedback to accommodate for any changes in the immediate environment in which the new system will be embedded in. 

<a href="/images/agileguide/scrum-iteration.jpg" target="_blank">
  <img src="/images/agileguide/scrum-iteration.jpg" alt="Typical data science project phases in an Agile iteration.">
</a>
*Figure 1: Typical data science project phases in an Agile iteration.*

## Waterfall or Agile?
Projects that have a clear set of pre-defined requirements with no, or very little, prospect of change can follow a linear approach to development, i.e. systems that have to comply with policies and regulations that are not expected to change.  
Other data science projects with complex requirements and novel functionality that require adaptability and flexibility are more suitable for an iterative development approach that prioritises delivering value over following a contract. 

## The Agile manifesto and principles
The Agile manifesto has 4 rules and 12 principles that the Agile team has to abide with:

- Individuals and interactions over processes and tools
- Working software over comprehensive documentation
- Customer collaboration over contract negotiation
- Responding to change over following a plan

>That is, while there is value in the items on the right, we value the items on the left more. More information on the Agile Manifesto [here.](http://agilemanifesto.org){:target="_blank"} 

According to the Agile Manifesto, the 12 principles state:

1. Our highest priority is to satisfy the customer through early and continuous delivery of valuable software.
2. Welcome changing requirements, even late in development. Agile processes harness change for the customer's competitive advantage.
3. Deliver working software frequently, from a couple of weeks to a couple of months, with a
preference to the shorter timescale.
4. Business people and developers must work together daily throughout the project.
5. Build projects around motivated individuals. Give them the environment and support they need, and trust them to get the job done.
6. The most efficient and effective method of conveying information to and within a development team is face-to-face conversation.
7. Working software is the primary measure of progress.
8. Agile processes promote sustainable development. The sponsors, developers, and users should be able to maintain a constant pace indefinitely.
9. Continuous attention to technical excellence and good design enhances agility.
10. Simplicity--the art of maximizing the amount of work not done--is essential.
11. The best architectures, requirements, and designs emerge from self-organizing teams.
12. At regular intervals, the team reflects on how to become more effective, then tunes and adjusts its behavior accordingly.


## Agile as a mindset
Agile was first introduced as a software development methodology, but since then is being used as a project management methodology and more recently as a mindset focusing on small steps towards your end goal and embracing failing as long as we learn from it, adapt and proceed forwards. 

The following infographic describes five paradigms that helped me apply the Agile manifesto and rules and achieve an Agile mindset and way of thinking:

<div class="carousel">
  <img class="carousel-image" src="/images/agileguide/mindset1.jpg" alt="Image 1">
  <img class="carousel-image" src="/images/agileguide/mindset2.jpg" alt="Image 2">
  <img class="carousel-image" src="/images/agileguide/mindset3.jpg" alt="Image 3">
  <img class="carousel-image" src="/images/agileguide/mindset4.jpg" alt="Image 4">
  <img class="carousel-image" src="/images/agileguide/mindset5.jpg" alt="Image 5">
</div>
<div>
  <!-- "Previous" button -->
  <button class="button" onclick="prevImage()"><</button>
  <!-- "Next" button -->
  <button class="button" onclick="nextImage()">></button>
</div>

<script>
  let currentIndex = 0;
  const images = document.querySelectorAll('.carousel-image');
  const totalImages = images.length;

  function showImage(index) {
    images.forEach((img, i) => {
      img.style.display = i === index ? 'block' : 'none';
    });
  }

  function nextImage() {
    currentIndex = (currentIndex + 1) % totalImages;
    showImage(currentIndex);
  }

  function prevImage() {
    currentIndex = (currentIndex - 1 + totalImages) % totalImages;
    showImage(currentIndex);
  }

  showImage(currentIndex);

  setInterval(nextImage, 6500); // Change image every 6.5 seconds (adjust as needed)
</script>
*Figure 2: The five paradigms that help teams and individuals achieve an Agile mindset and an iterative and incremental way of thinking and working*

The transition from linear to iterative way of thinking and working can be challenging. An approach that helped me personally is by following this simple 3-task approach: 
1. Pick one simple task or item from your to do list that will take you closer to your goal
2. Take a step forward and complete the task
3. Look back, reflect, adapt and pick the next step. 

Click [here](/downloads/Agile_mindset_infographic.png){:target="_blank"} to download the infographic on the five paradigms on applying the Agile mindset. 

# Scrum framework
The Scrum framework helps teams implement the Agile manifesto (4 rules and 12 principles) by introducing a structured cycle, called **sprint**, of the following events and artefacts:

- **Product backlog:** a list of all the known user requirements to be built in the project.
- **Sprint planning meeting:** a meeting with the scrum team to prioritise and plan for the upcoming sprint.
- **Sprint backlog:** a list of all the user requirements that the team decided to implement in this sprint.
- **Sprint development:** the team works together to develop and test new functionality, optimise existing code and fix any found bugs.
- **Daily scrum:** a short meeting with the team to discuss progress of previous day, the plan for the day and any blockers that might need help with.  
- **Sprint review:** a meeting with the team and external stakeholders to reflect and sign-off the requirements that were implemented in the sprint. 
- **Increment:** all the functionality built and delivered in all previous sprints.
- **Sprint retrospective:** an internal meeting with only the scrum team to reflect on tools, platforms, workflows, progress, etc. 

<a href="https://iliada-eleftheriou.com/images/agileguide/scrum-framework-9.29.23.png" target="_blank">
  <img src="/images/agileguide/scrum-framework-9.29.23.png" alt="Source: Scrum.org">
</a>
*Figure 3: The Scrum rituals and artefacts in a sprint cycle of development, source: [Scrum.org](https://scrum.org){:target="_blank"}.*

The following video (9.07 min) provides a brief introduction to the Scrum framework. 

<div class="embed-responsive embed-responsive-16by9">
  <iframe width="560" height="315" src="https://www.youtube.com/embed/d5BwZ8IxPos?si=wZAMI2v6X-FA38WZ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>
*Source: Video produced by Dr Iliada Eleftheriou for, and edited by, Health Data Research UK (HDRUK), 2022. This video is part of a longer HDRUK course on applying modern information engineering for health data scientists. It's a free course (create an account) and is available [here.](https://hdruklearning.csod.com/catalog/CustomPage.aspx?id=221000379&page=Health-Information-Engineering-Pathway-Page){:target="_blank"}*


## The Scrum team: roles and responsibilities
Data science lies in the middle of three areas: mathematics and statistics, computer science, and domain expertise. The data science team lies in the intersection of these three areas and is usually formulated by the following roles:
- Product owner: 
  - understands the problem to be solved, and the domain area in which the data is created, and collected. The product owner has a clear vision of the end product and acts as the middle layer between the agile team and the stakeholders. 
- Scrum master: 
  - knows the process to solve the problem
  - the role of the scrum master is of a servant leader that knows the processes, rules and tools of the Scrum framework and facilitates the meetings happening in a sprint. 
- Development team:
  - has the **technical and domain experience** and is responsible for building the product right 
  - data scientists, software engineers, domain experts, data analysts, data engineers, user experience experts, testers, system architecture, information governance officers, health practiotioners, etc.

In recent years, we've seen the role of scrum master to evolve into tech lead, or product lead as teams now have a clear idea of how to implement the Agile mindset and the tools and practices of the scrum framework. New teams that are embarking on their Agile journey for the first time, will benefit by having a scrum master. 

## Project kick-off

> - Forming the project:
>    - Set goals, aim and objectives 
>    - Define the problem to be solved 
>    - Set outcomes, success criteria and if needed define key performance indicators
>    - What's the impact and value to be delivered?
>    - Consider any policies and ethical considerations
> - Form a team and assign roles: Identify the technical requirements of the team and make sure you have both technical and domain expertise in your team. 
> - Pick an appropriate software development and project management methodology
> - Decide on tools and platforms for collaboration. Some useful tools are: Slack for communication, Miro for brainstorming, Google drive for creation of documents, Git for sharing code, Teams and Zoom for meetings, Trello for organisation, etc.
> - Set the culture, ethos and values of the team. Ensure you all share a clear vision of the goal. 


## Requirements gathering

The following video (7.34 min) provides a brief introduction to gathering requirements in an Agile manner: 

<div class="embed-responsive embed-responsive-16by9">
  <iframe width="560" height="315" src="https://www.youtube.com/embed/O6QWBoVDZ7E?si=qbIxBOV1ORcvGRj_" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>
*Source: Video produced by Dr Iliada Eleftheriou for, and edited by, Health Data Research UK (HDRUK), 2022. This video is part of a longer HDRUK course on applying modern information engineering for health data scientists. It's a free course (create an account) and is available [here.](https://hdruklearning.csod.com/catalog/CustomPage.aspx?id=221000379&page=Health-Information-Engineering-Pathway-Page){:target="_blank"}*

> - Identify key stakeholders, these can be: 
>   - end users of the system to be built, people on the ground using the new AI predictive tool, clients, shareholders, clinical scientists, clinical teams, CIOs, researchers, etc. 
> - Start collecting requirements by organising (a combination of) the following activities:
>   - focus groups 
>   - questionnaires
>   - observations
>   - literature reviews 

The outcomes of these sessions can be summarised in the form of **Personas** and **User stories** - see sections below for more information. 

## Personas 

Personas are fictional characters that represent the various types of end users and stakeholders of the end product. Different stakeholders and groups of people have different needs, behaviours and goals. Different clinical or clerical teams might use the system in a different way, others for data entry, other for data analysis, create visualisations etc.

> - Create personas to capture the main types of end users
> - Identify their strengths, weaknesses, motivations and frustrations, demographic information and technical literacy. 

![An example of a persona template](/images/agileguide/persona_1.png)
*Figure 4: A persona template*

## User stories
A 'User story' is a simple but very powerful tool for capturing requirements from the perspective of our end users and stakeholders. They follow a very strict format that captures three key elements:
- The type of user
- The functionality they want 
- And why they need it - the value it will create. 

User stories don't capture **'how'** a functionality will be developed but **'what'** will be developed and **'why'** is needed. By following this structure, the Agile team ensures that all relevant types of users are considered, and functionality will deliver value avoiding spending time to deliver something that might not be needed. The technical team has the freedom and responsibility to decide what's the best approach at developing the functionality. 

![The structure of a user story](/images/agileguide/user_story.jpg)
*Figure 5: The structure of a user story*

**Epic user stories** describe too big slices of functionality and are very abstract. For example, 'As a Clinical Information Officer, I want a monitoring tool, so that I can see the processes running at any point of time in the digital services department'. 

> - Collect your requirements in the form of user stories. 
> - Link your user stories to the personas you created. 
> - Refine your user stories: Break-down Epic user stories into smaller slices of functionality.

## Kanban boards
'Kanban' is a japanese term for billboard and also describes a popular Agile framework that visualises all work items (everything that needs to be completed) on a single board, called a Kanban board. Kanban boards allow all team members to see the state of every piece of work at any time. 

A work item can be a user story describing the functionality to be built, an event (i.e. sprint planning), or a task/process (i.e. updating documentation, refactoring code, etc).

Work items in Kanban board are usually called tickets, or cards and are clustered in the following columns:
- **Product backlog:** An ordered list of all requirements (user stories) that are needed in the end product. It's a single source of all the requirements and is dynamic, it evolves as the product is formed. 
- **In progress:** contains work items that have been allocated to a team member and development has started.
- **Done:** contains work items that have been completed and await signed-off either in the form of testing, approval from stakeholders, or code review (pull request) from another development. 
- **Done done:** contains work items that are signed-off and deployed. 

Work items are assigned to team members who are the owners of the work and responsible for completing them. Items travel from left to right on the board and team members begin a new work item only after they have completed their assigned work items. Teams can have different definitions of 'Done' and 'Done done' functionality.

Note: The Kanban framework can be used in combination with the Scrum framework. Another column, called **Sprint Backlog**, is visualised right after the Product Backlog column and contains the work items that the team decided to complete during the sprint. 

There are several tools to help you create and manage your board online. Two of the most popular ones are [Trello](https://trello.com){:target="_blank"} and [Jira](https://www.atlassian.com/software/jira){:target="_blank"}. There are free versions of the tools and plenty of plug-ins to connect to your boards.

![A Kanban board example using the Trello tool.](/images/agileguide/trello_board.png)


> - Define what 'Done' and 'Done done' means in your team.
> - Decide how long your Sprint will be. A sprint is usually 1 or 2 weeks long depending on the size of the project and team. 
> - Set up your Kanban board. Create the columns that are relevant to your project. 
> - Add (or link) your personas to the Kanban board in the Personas column. 
> - Add your user stories or requirements in your Product Backlog column.
> - Set up your development environment (i.e. Anaconda distribution for Python), or if a codebase already exists, clone the repository on your local machine and set up Git to share code and collaborate with your team members. More info on collaborating with Git will be available soon. 
 


## Sprint planning meeting
Your team is now ready to begin the Sprints (cycles of planning, development and testing). The Sprint begins with the spring planning meeting in which the entire Scrum team plans what will be delivered at the end of the sprint. 

To do this, the team completes the following three activities: 
- **Product Backlog grooming:** 

The team revisits the product backlog and breaks down 'Epic' user stories into smaller, more refined user stories that describe a thin layer of functionality. The team also adds more details to the user stories and gathers intel on how they will be implemented. 

-  **Estimation:**

The team estimates the effort needed to complete every user story. Agile teams rarely use time (minutes, hours, days) to estimate user stories, instead they use a relative approach, called **story points**. Story points take away the complexity and pressure of time (for example, two days of development are rarely the same for everyone in the team) and provide a relative way of comparing the complexity of the functionality to be built. For example, a user story with estimated 4 story points is twice as big as a user story with 2 story points assigned. 

Strategies for estimation:
   - T-shirt sizes: A user story can be small, medium, or large. Small indicates a simple task at hand, whereas Large indicates complex work or uncertainty on how to achieve. 
   - Planning poker: Every team member assignes a number from the Fibonacci sequence to the same user story. Outliers are discussed and the team decides on allocating story points. An advantage of this technique is that everyone's perspectives are taken into consideration. 

-  **Prioritisation:**

The team prioritises user stories based on the needs of the stakeholders. 

Strategies for prioritisation:
   - Traffic light system: Red is very urgent (usually indicating bugs in the code or critical functionality), amber typically indicates high importance or high impact, and respectively green indicates low impact.
   - MoSCoW model: This model categorises work items in: Must do, Should do, Could do, Would be nice to do. 
   - Priority matrix: Prioritise the work items that are of high importance and low effort first, then high imprortance and high effort, and then low importance low effort, etc. 

![An illustration of estimation and prioritisation using a Trello card](/images/agileguide/trello.png)
*Figure 6: An illustration of estimation and prioritisation using a Trello card*

Tasks: 
> - Groom your product backlog: Refine your epic user stories into smaller thin functionality (i.e. create new user stories that describe smaller parts of functionality) 
> - Add more details in the user stories (i.e. formulas, algorithms documents, descriptions, personas, etc.) and highlight any questions you might want to ask your stakeholders. 
> - Break down your user stories into a series of tasks. 
> - Estimate your user stories: Decide which technique you will use (i.e. T-shirt sizes, planning poker, etc). You might have to assign story points to the t-shirt sizes so you can then create burn up/down charts. 
> - Prioritise your user stories: Decide which strategy you will use. 
> - Based on your estimations and prioritisation strategy, decide which user stories you will complete in this sprint.
> - Populate your sprint backlog (drag and drop the user stories in the Sprint Backlog column). Avoid having Epic user stories in your sprint backlog. 
> - Assign team members to each user story in the Sprint backlog column. 

Your team and Kanban board are now ready to begin the sprint. 

<!-- 
GIT - clone or set up your repository and IDE.
11.	Break down your user stories into tasks. 
11. Design your test cases. - acceptance criteria. 
14.	Decide on your git strategy (For example: consider having a development branch and then branch off to feature or developer branches. Test your functionality in the dev branch before merging to the master branch.)
15.	Create a burn up or burn down chart to track the progress and velocity of your team.  -->


## Sprint design, and development

Agile teams test early and often. One form of early testing happens even before we have written a single line of code. **Acceptance criteria** define when a user story can be considered completed, or 'done'. They are typically shown as a list or follow this simple template:

![Acceptance criteria](/images/agileguide/acceptance_criteria.jpg)

Acceptance criteria don’t offer a solution on how the functionality will be developed, but how it will be tested. 

> - Pick the user story you have been assigned.
> - Understand what the goal and value to be delivered. 
> - Break down your user story into more refined tasks. 
> - Design acceptance criteria. 
> - Pick a development strategy and start developing. 
>   - Pair programming 
>   - Ping-pong development
>   - Solo programming
>   - Mob programming
>   - Pomodoro technique

## Sprint testing

When designing our test cases, we usually consider the following cases:
- Valid cases 
- Invalid cases 
- Outliers 

There are several types of testing each testing various aspects of the codebase and project. Some of the most popular types of testing are [^1]: 

[^1]: The items in the list of types of testing have been expanded using generative AI tools. All the content has been evaluated and modified (wherever appropriate) by the author. 

Unit Testing:
- Purpose: Unit testing verifies the correctness of individual code units, such as functions or methods, in isolation. It is focused on ensuring that each unit of code works as intended.
- Scope: Isolating and testing small sections of code without considering the interactions with other parts of the application.
- Key Concepts: Test frameworks (i.e., JUnit, PyTest), test cases, test fixtures.

Integration Testing:
- Purpose: Integration testing ensures that different components or modules of the software work correctly together. It focuses on identifying issues that may arise when integrating these units.
- Scope: Testing interactions and data flow between integrated components.
- Key Concepts: Integration test suites, interfaces, data exchange.

Acceptance Testing:
- Purpose: Acceptance testing is performed to determine whether the software meets specific requirements and is ready for production deployment. It validates that the software satisfies business needs through completion of the acceptance criteria set against user story in the beginning of the sprint. 
- Scope: End-to-end testing of the entire system, often performed by stakeholders or users.
- Key Concepts: acceptance criteria, final validation.

Test-Driven Development (TDD):
- Purpose: TDD is a development methodology where developers write tests before writing the actual code. It promotes a cycle of "red-green-refactor," helping to design and verify code incrementally.
- Scope: TDD is applied at the unit level, writing tests for specific features or functions.
- Key Concepts: Red-Green-Refactor cycle, test-first development, continuous testing.

Behavior-Driven Development (BDD):
- Purpose: BDD extends TDD by focusing on the expected behavior of the software from a user's perspective. It promotes collaboration between developers, testers, and non-technical stakeholders through a non technical language called Gherkin that resembles the structure of a user story and can easily be read and written by non-technical people.
- Scope: BDD involves defining and testing behavior or scenarios for the software's functionality.
- Key Concepts: Gherkin syntax (Given-When-Then), feature files, executable specifications.

A/B Testing:
- Purpose: A/B testing is a method to compare two or more versions of a webpage or application to determine which one performs better in terms of user engagement or conversion rates.
- Scope: Typically used for assessing the impact of changes to the user interface or user experience.
- Key Concepts: Control group, variant groups, statistical analysis.

Black-Box Testing:
- Purpose: Black-box testing focuses on the functionality of the software without examining its internal code. Testers assess the software's inputs and outputs.
- Scope: Treating the software as a "black box," testing without knowledge of its internal workings.
- Key Concepts: Test cases based on specifications, functional testing.

Regression Testing:
- Purpose: Regression testing ensures that new code changes do not adversely affect existing functionality. It helps maintain the stability of the new tool.
- Scope: Re-testing core functionality and critical paths after code addition and updates.
- Key Concepts: Use of test suites, automated testing. 

Stress Testing:
- Purpose: Stress testing evaluates the system's stability and performance under extreme conditions, such as high loads or resource constraints.
- Scope: Assessing how the software handles extreme loads or challenging scenarios.
- Key Concepts: Load testing, performance benchmarks, system limits.

Usability Testing:
- Purpose: Usability testing assesses the software's user-friendliness and overall user experience. It focuses on ensuring that users can interact with the software effectively and intuitively.
- Scope: Evaluating the software's interface, navigation, user interactions and user journeys.
- Key Concepts: User feedback, user experience (UX), user-centered design.

> - Decide your groups testing strategy - which combination of types of testing are suitable to test the functionality that you will/have created in this sprint? 
> - Revisit the acceptance criteria you set in the sprint planning meeting and design your test cases. 
> - Create a test suite, if you don't already have one, and add new unit tests for the new functionality you have developed.
> - Run each test separately and make sure it runs.
> - Run the entire test suite to ensure there are no conflicts and that the components integrate with no issues. 
> - Run test coverage to identify gaps in your testing design.

## Sprint review and deployment
The team demonstrates completed functionality of the product they've built (also called the increment) during the sprint to key stakeholders and end users. This is an informal event in which the team gathers feedback on the increment, ensures alignment with the product vision and end goal, refines requirements and makes adjustments for the next sprint.

The outcome of the sprint review meeting is a revised Product Backlog that defines the probable Sprint Backlog items for the next Sprint. The Product Backlog may also be adjusted overall to meet new opportunities. 

>  During a sprint review: 
>  - The Product Owner explains what Product Backlog items have been “Done” and what has not been “Done” 
>  - The Development Team discusses what went well during the Sprint, what problems it ran into, and how those problems were solved 
>  - The Development Team demonstrates the work that it was “Done” and answers questions about the Increment 
>  - The entire group collaborates on what to do next, so that the Sprint Review provides valuable input to subsequent Sprint Planning 
>  - Review of how the wider environment or potential use of the product might have changed and what is the most valuable thing to do next.


## Sprint retrospective
The goal of this internal informal meeting is to reflect on how the team worked together in this sprint and identify actionable steps for improvement. The team reflects on: processes, team culture, outcomes, tools and platforms, etc. 

Strategies for retrospectives: 
- Start - stop - continue
- Sailboat retro

The outcome of the retro meeting is a list of actions, or changes that the team agreed to take on board in the next iteration.

> During the retrospective (also known as retro) the Agile team reflects on the three main questions:
>  - What went well?
>  - What could have gone better?
>  - What to change?

> Then, the team creates a list of actions/changes that unanimously decide to take on board in the next iteration. Each item is usually assigned to a particular team member and the team might also set a milestone if needed. 

<a href="/images/agileguide/retro.jpg" target="_blank">
  <img src="/images/agileguide/retro.jpg" alt="Agile retrospective structure">
</a>
*Figure 7: A board created with the Miro online tool to capture the structure of an Agile retrospective meeting.*

## Evaluation and write up 
See more information on the anatomy of scientific writing, and a template to help you structure your findings [here](/blogposts/scientific-writing){:target="_blank"}.


# Collaborating with Git
// More information on the use of Git will be available soon.  

# Spotted a mistake? 
Did you find this guide useful, or spotted any mispellings? Any feedback and ideas for expansion are more than welcome.  

<!-- # Download checklist
You can download a word document with a compiled checklist of all the phases described in this guide to help you form, manage and develop your new data science project. 
> [Download checklist](/downloads/Agile_checklist_V1_1.docx){:target="_blank"} -->

# Versions
<!-- https://www.tablesgenerator.com/markdown_tables -->

|     Version    |     Date             |     Updates                                                                                             |
|----------------|----------------------|---------------------------------------------------------------------------------------------------------|
|     V1.1       |     October 2023    |     Guide created.                                                                                       |
|     V1.2       |     October 2023    |     Updated and expanded Sprint Review and Retro.       






