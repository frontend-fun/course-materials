These are instructions for instructors to adopt our curriculum.

# Setting up the Assignments

We don't use github classroom for these. You just need to setup the GradeScope course in Canvas.

1) Open GradeScope in Canvas, and create a new course linked to this Canvas course.
2) Use the "Duplicate assignment" to make a copy of the upstream courses' assignments
3) Open each assignment page in Canvas, and choose to link to an existing assignment (matched to the duplicated copy you created previously)
4) Adjust all due date and lock dates for that assignment

# Modifying the Autograder

If you are just copying the assignments unchanged, then you shouldn't need to modify the autograder. However, if you do want to make changes, you can fork the `tasks-autograder` repo and then use the tools there.

# The Repos

Once you've been added as an Adopter, you have access to:

- The `frontend-fun/tasks-autograder` (private) repo holds the autograding logic. We put the test folders into `staging_main/tasks/`, and it will create an uploadable zip file for GradeScope, one for each task. We only have to upload those to gradescope once, since after that they'll just pull from this repository. <https://github.com/frontend-fun/tasks-autograder>
- The `tasks` repo is now up to date with the latest versions of react and my fancy build script. In addition to building and publishing the students code with less hassle (no more weird `GITHUB_TOKENS`, just turn on github pages and actions), it builds a "Quick Links" (accessible at `https://<repo-url>/quick`) page with links to the github repo, a gitinspector report, data dumps from the install/lint/build/test phases (even if one step fails), dumps md5 hashsums of the critical files (to help check for tampered instructor files). <https://frontend-fun.github.io/tasks/docs/quick-links.html>

# Posting Grades

You might already know this about Gradescope, but the grades don't automatically transfer until you click the "post grades to canvas" button on an assignment. Here are instructions, I just recommend doing it after the assignment is due.

1. (Within Gradescope), go to the graded assignment.
  1. Click Assignments at the left.
  2. Click on the assignment from the list.
2. Click on Review Grades from the assignment menu at the left.
3. Click Post Grades to Canvas from the menu bar at the bottom.
4. In the Post Grades to Canvas window, click (edit) under Linked Canvas Assignment.
5. The window will not change to a drop down list of your assignments in the linked Canvas course. This may take a few moments.
6. Click on the drop down menu and select the assignment in Canvas that this Gradescope assignment should post its grades to.
7. Click Link Assignment.
  1. You may need to repeat steps 1, 2, and 3 after linking the assignments.
8. Click Post Grades.
9. Wait until you see the message ✓ Grades successfully posted to Canvas!
10. Click Close.

These instructions are taken from <https://teaching.pitt.edu/resources/using-gradescope-with-can>
