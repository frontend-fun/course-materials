---
waltz:
  title: Final Project Description
  resource: page
  published: true
---
Welcome to the Final Project! You are going to work in a group to create a large-scale piece of software. The end result
will be evaluated not only for its quality as an artifact, but also for its maintainability, potential for scalability,
and stability. You yourself will also be evaluated for your performance on your team and your use of appropriate
software engineering strategies.

You will follow an Agile development methodology, structuring the development into weekly Sprints. A Sprint will begin
with a Standup, and end with a Retrospective. Along the way, you will plan and document your progress using a Product
Backlog full of User Stories.

Technology-wise, we are going to use React and TypeScript, focusing on frontend web development. You will track your
development in Git, making small commits isolated to branches. Your final project will be continuously integrated and
deployed.

### The Project: UD CIS Scheduler

Every student at the University of Delaware is assigned an Academic Advisor who is meant to help guide the student to graduation. From the UD [Academic Advising webpage](https://www.advising.udel.edu/){: .inline_disabled}:

> Academic advisors _help_ students develop their academic goals, understand their degree requirements, and connect with
> appropriate university resources... Academic advisors _support_ students as they develop the skills and knowledge to
> make well-informed decisions regarding their academic and career goals.

The advisor's role is to help students become self-sufficient, and they aren't intended to make decisions on behalf
students. Ideally, by the end of their degree, students have chosen their own path to graduation, with minimal input
from their adviser. To facilitate their choices, students are often strongly recommended to construct a **Degree Plan**.

![A portion of an example, abstract degree plan for a CIS major](degree_plan_example.png)  
**A portion of an example, abstract degree plan for a CIS major.**

However, an open-ended field like Computer Science poses a unique challenge, since there are many possible paths to
graduation with different tradeoffs and opportunities. Indeed, many students come in with almost no knowledge of the
possible career directions and what courses support those paths. Further, the incredibly high student-to-faculty ratio,
along with already stretched faculty resources, exacerbates the situation. There is never enough time for busy faculty
to meet with their advisees.

Although there are many logistical and administrative barriers to success, at least one procedural problem might be
solvable with technology: many students struggle to put together a clear 4-year plan without a lot of prompting and help
from their adviser.

Your goal is to develop a web application that helps Computer Science majors at the University of Delaware to put together a Degree Plan to streamline their advising experience.

### User Stories

The following User Stories capture the necessary features for students using your application. Early on, we will create
personas for these user stories to help us think about the different kinds of students using our software.

  * Students can access the published site publicly through their browser
  * Students can see a table that shows a single semester of courses
  * Students can see a table that shows multiples semesters of courses
  * Students can see a list of all the degrees plans that they have made 
    * So a degree plan is a collection of semesters, and a semester is a collection of courses
  * Students can edit the course code, course title, and credits of a course in the plan
  * Students can clear out all the existing courses in a semester
  * Students can clear out all the existing semesters in a plan
  * Students can insert or remove a plan
  * Students can insert or remove a semester to their plan
  * Students can insert or remove a course in a semester
  * Students can skip semesters 
    * "I am not taking any classes in the Fall 2021 semester, but I am taking classes in Winter 2022 and Summer 2021"
  * Students can save their current degree plan and load plans between working sessions
  * Students are introduced to the application with a friendly message that clearly explains their goal and how they should get started
  * Students can visualize the unfilled requirements of their degree plan
  * Students can establish that a course fulfills a degree requirement 
    * "CISC220 is a required course for all degrees"
    * "The degree must have at least 3 technical electives
  * Students can establish that a course meets another course's prerequisite 
    * "CISC108 serves as a prereq for CISC210"
  * Students can move courses from one semester to another semester, or to a free-standing "pool of courses" to use later
  * Students can override course's info, but also reset a course back to its default information 
    * "CISC367 (the experimental course number) could be set to 'Introduction to Data Science' and fulfill a Technical Elective"
  * Students can export their plans as CSV files, suitable for sharing with advisers
  * Students can import their plans from CSV files, even after small modifications have been made

### Constraints

Your application is going to have the following constraints placed on it.

  * You must use React, and more specifically React Hooks. Class-based components are way passé. 
  * You must use TypeScript, with well-defined types. You are not allowed to use `any`, `unknown`, or other typeless types.
  * You must use branches, with the `main` branch always stable and continuously deploying.
  * You must use a linter, with any committed code passing all linting and formatting checks. You cannot override the linter or changes it settings.
  * Your application must be well-tested, with the `main` branch always passing all tests.
  * You must deploy your application via GitHub pages. 
  * The user experience matters. Your codebase matters. 

## Feature Prioritization

The list of features probably seems overwhelming at first.

DON'T PANIC.

As a team, you will meet each week to break off a manageable chunk of work for each sprint.

Your goal is to create a Minimal Viable Product. If you don't finish all the features, you should at least aim to finish
as many as you can.

We are interested in seeing you put in consistent work and progress. Although finishing the application is the goal, we
recognize that teams will end up in different spots. Have a healthy commit log and a consistently full project board,
and you shouldn't have to worry about your project's state at the end.

### Basic Setup

To get your repository set up, follow all the instructions carefully in this assignment: [Final Project Setup](Final%20Project%20Setup.md)

### Weekly Schedule

Starting from today, the course shifts to become largely project-focused, even more so than before.

Starting from Tuesday April 12th, class will follow this schedule:

  * First half of Tuesday Lecture: Team will complete a Sprint Retrospective 
    * Note that we do not have a Retrospective the first week. Instead, students will have an extra long Sprint Planning Session and more time to get help setting up.
  * Second half of Tuesday Lecture: Team will complete a Sprint Planning session
  * Thursday Lecture: Team will complete a Standup in class, and then be free to work on the project and get help from Dr. Bart.
  * Monday Lab: Teams meet as a group to get work and to get feedback/help from their TA. 
    * Note that lab attendance is still mandatory. You are expected to also be working outside of class, but we expect to still see you in lab. This is a good time to do your Retrospective and Review.
  * Homework due before next Tuesday Lecture: Team will complete a Sprint Review that describes the functionality they have achieved the previous week and a Sprint Retrospective reflecting on their team's progress.

### Grading

The Final Project is organized into 3 distinct grades: the weekly Sprint Events (25%), one MVP submission (10%), and the
Final Version submission (20%).

For the next month and some change, you will be expected to participate in weekly sprints. These include a Sprint
Planning session, Sprint Review, and Sprint Retrospective. The Planning and Retrospective sessions will occur in
Thursday Lectures, while the Review will be homework for your team. Details about the expectations and grading for these
events will be delivered in their respective Canvas Assignment and in-class. However, suffice to say, you can anticipate
that these will be a measure of your consistent effort and progress along the way. There are roughly five weeks, with
each weeks' collective events being worth 5% of the final course grade.

At the end of Sprint 4, you will be expected to make a submission of the "Minimal Viable Product" of your application. This assignment will be graded based on the quantity and quality of the features implemented, the quality of your codebase, and your adherence to best Software Engineering practices. Having a lot of features with a low quality codebase is just as bad as having a few features in a high quality codebase. Balance your time and avoid [technical debt](https://wiki.c2.com/?TechnicalDebt){: .inline_disabled}. The MVP submission is an opportunity to get some feedback on your application as we reach the end of the course. There will be both an individual and group component to the grade.

Prior to the end of the semester, you will be expected to make a "Final Version" submission. It will be graded similarly
to the MVP submission, just with slightly higher expectations and an increased percentage of the final grade.

You will also be periodically asked to complete a Peer Evaluation. This will give us independent information on how well
your teammates are working.

### Frequently Asked Questions

  * _"Instead of making this, can I make something else?"_  
No.

  * _"Isn't this just a spreadsheet? They give us a four-year form."_  
If the final version of your application offers nothing more than what a spreadsheet can give you, then you haven't
really created anything substantial. The real potential for this application lies in the extra information it can
provide - stuff like identifying requirements, prerequisites, and, most of all, a lot of default information.

  * _"Can I change group mates?"_  
Only in the most extreme circumstances. Learning to work with others is part of the course's goal! Remember, there is a
group and individual component to the grade.

  * _"My team mate isn't doing any work!"_  
Try to talk to your teammate and see if you can help them get back on track. Often, lack of productivity comes from fear
and not innate negative characteristics. Start by seeing what you can do to help them feel comfortable contributing to
the project. Help them find ways to learn the material (e.g., working with TAs, trying more tutorials). Remember there
is ultimately a group and individual component to the grade, and we will ask you to rate your teammates.

  * _"Can I turn off the linting rules?"_  
No. If you disable them, then your project will be completely rejected.

  * _"Can I turn off the type system rules?"_  
No. If you disable them, then your project will be completely rejected. Some special exceptions may occur, but you must
get our permission.

  * _"Can I turn off the tests/linter blocking me from pushing to main branch and deploying?"_  
No. Don't push broken, improperly formatted code to the main branch.

  * _"How much can students interact outside of groups?"_  
Be cautious working outside of groups. Sharing code may be plagiarizing. Instead, focus on sharing common help resources
(e.g., tutorials, stack overflow pages). Sharing of data (e.g., a well-formatted list of courses) should be fine too.

  * _"Are there any requirements for the user interface? Like does it need to be responsive?"_  
We have no specific requirements other than that usability matters. Your team can decide stylistic choices. Having a [responsive design](https://en.wikipedia.org/wiki/Responsive_web_design){: .inline_disabled} is certainly a nice idea, and fairly easy to do with Bootstrap. 
  * _"Do you recommend making mockups or design diagrams of our site?"_  
Yes! These may not be accurate to the final version of your site, but having the team get together and plan what the
application looks like is much more likely to lead to a better end product. You don't need a huge amount of detail -
make a "wireframe" diagram that shows off the important user interface elements.

  * _"What's the 'Data model'?"_  
When you sit down and make your application, you will need to think about the "Data Model". This is the core
representation ("abstraction") of the reality that your application is manipulating with its interface. For example,
part of your data model will probably be a "Degree Plan" which might be composed of a list of "Semesters", and
"Semesters" which will have a name and a list of "Courses". A "Course" might have a name, a number of credits, etc.
Often, this model exists in your codebase as Interfaces. Spend time developing your Data Model, and making sure your
team is on the same page about it. You will have to adapt it over the course of the semester, but the sooner you know
what it looks like, the better!

  * _"My team and I were wondering how the Sprint Reviews will be graded?"_  

This is a reasonable question, but a little complicated to answer. Here are some notes:

    * In addition to being graded for your participation in the Sprint Events, you will also be assessed on your progress via a Sprint Review. Every group is expected and encouraged to decide their own approach to their work. Necessarily, every group will end up with a different set of tasks that they set for a Sprint. Groups will make progress at different rates, based on their strengths.

    * There is no specific set of features that you must complete. I would be surprised if certain ones weren't tackled in the first sprint (e.g., putting a table on the screen), but it's not necessary to complete any particular subset for the first sprint. However, we expect you to make progress on tasks. The exact amount of progress varies between groups. Some groups might finish several smaller features, and other groups might finish a few much bigger features. Both groups could earn the same grade. However, a group that finished fewer, smaller features than other groups would probably receive a bad grade for that part of the rubric, if we thought they weren't making sufficient progress.

    * Keep in mind that breaking up large tasks is a part of this process - if you attempted only one task, and you failed to complete it, then you probably failed to break it up sufficiently. Break up complex tasks so that you can demonstrate progress within a sprint, and you don't have to return items to the Product Backlog.

    * We do not expect you to perfectly estimate the tasks correctly, especially in these first two Sprints. Groups are likely to over- and under- estimate the difficulty. However, we expect that variation to go down after the first few Sprints and you get a better handle on things.

    * Your group can also revise your Sprint Backlog during the Sprint, breaking up tasks into smaller ones, moving items back to the Product Backlog, or bringing in new items to the Sprint Backlog. Note, however, that the usual wisdom in Scrum is that if you finish early, you should help your teammates finish the current Sprint goals before trying to bring in new work. For instance, working on tests or helping debug.

    * For the first week, you might approach things mathematically. If your group estimates each task with a number, using something like "1" for 1 hour task, "2" for 2 hours, etc.; and you've scheduled out 6 hours of work over the course of the sprint week; then you could make sure that the total number of tasks adds up to about 18 hours (assuming three teammates), plus or minus. You'll probably find that things are wildly inaccurate from there, but it's at least a starting point.

### Change Log

  * 9/26 at 1:47am: Initial version created
  * 10/12 at 3am: Release version finished
  * 10/12 at 10:53am: FAQ updated with three new questions (about "design requirements",  "making mockups", and "your data model")
  * 10/15 at 3:20pm: FAQ updated with a question about grading sprints
  * 3/28 at 11:04am: New version for spring semester, making requirements more clear and updating dates.