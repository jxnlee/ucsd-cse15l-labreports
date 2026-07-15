# Lab Week 8 - Code Review / It Works on My Machine

Discuss with your group:

![Image](assets/circles_vs_triangles.png)

Write down your answers (and why you chose them!) in your group's shared doc.

In this lab, you will review another group's code to give feedback, find new
bugs, and learn from each other.

The overall plan for lab is:

1. You'll have 30 minutes to work towards completion of your grading script from
   week 6, preparing it to be shared with another pair of students.
1. You will get a link to a repository from another group, download and work on
   the code for 30-40 minutes.
1. Your pair will meet with the pair whose code you reviewed/are reviewing, and
   you'll share feedback.
1. The feedback will be summarized as a pull request to your repository.

### Part 1 – Implementation Polishing

Make as much progress as you can on your grading script from [Week 6](../Week6/index.md#grading-script). Ask your lab tutor if you need help getting it into a good state.

To help guide your process, we've created a review Kahoot to help review bash concepts.
[Bash Review Kahoot](https://kahoot.it/challenge/09071020?challenge-id=0d166f0b-af02-41c1-af31-99d9c839a769_1684882612376)

Don't worry about perfection; focus most on it being able to run and grade some
of the sample submissions.

When you're happy with it, have one partner make a **new** repository on Github
named `grader-review-<username>` where `<username>` is one of your usernames.

To do this, navigate to any GitHub page and click the `+` button in the top right corner, as seen on the screenshot below. A dropdown menu will appear, and you will click `New repository`.

![Image](assets/github_new_repo_dropdown.png)

From there, a page will pop up which allows you to set some attributes of your new repository. The only thing you need to change is the name, as seen in the following screenshot. You do not need to alter any other settings, and can press the green `Create repository` button at the bottom.

![Image](assets/github_new_repo_page.png)

Now, we want this new repository to contain the version of your autograder that you want reviewed (This step
makes it so pull requests and issues will work in the last step later). To do that, you should navigate to your newly-created repository on GitHub.

Currently, it should be empty. You should see something like the screenshot below. We want to import your grading script code (which should exist in some other GitHub repo) into this repository. Click the `Import code` button circled in red below.

![Image](assets/import_code_to_new_repo.png)

After clicking the above button, a page will pop up which asks you for "Your old repository's clone URL". Here, you will paste the **_HTTPS_** url of the GitHub repository which contains your grading script to-be-reviewed. Click the green `Begin import` button and wait for your code to be transferred over.

![Image](assets/import_github_code_page.png)

Before sharing, we should also make sure that it will work for others, and
doesn't only work on your machine! All too often it's easy to write programs
that run our own laptop, but when someone else clones our code, it doesn't work
on theirs. This leads to the dreaded _it works on my machine_:

![Image](assets/works-my-machine.png)

We will standardize and say that _all the graders should run on `ieng6`_. So,
you should test your grader by logging into `ieng6`, cloning it, and running it
once there. If you get different behavior on a fresh clone on `ieng6` than when
you previously tested it, figure out what happened! Your lab tutor can probably
help, a few common issues are:

- Forgetting to add/commit a file (so someone who clones the repository doesn't
  have it). Check that all the files you need are there on Github.
- Having Windows-specific commands in a file that is then run on Mac/Linux.
  Check that classspaths use `:` and not the Windows-specific `;`
- Having differently-formatted files. Windows actually uses different newline
  characters than Linux by default. Check out [this
  article](https://blog.boot.dev/clean-code/line-breaks-vs-code-lf-vs-crlf/) for
  more on that issue.

Once you see the script run like you expect on `ieng6`, your grading script is
ready to be reviewed! Your lab tutor will manage assigning those submissions
between groups for review.

### Part 2 – Initial Review

Your lab tutor will provide you with a link to a repository for another group.

Make a _fork_ of it, clone it, and complete the following tasks. For each,
document it in your notes file:

- Run their grader on all of the sample student submissions from week 6. How does their
  output differ from yours? Do you think it's correct?
- Try running their submission on any additional submissions you designed during
  week 6. If you didn't do that during week 6, do it now – design a student
  submission that you think will cause interesting behavior on the grader you're
  reviewing.
- Read all the code in their submission. Note down:
  - Things you liked about the code
  - Any lines of code you don't fully understand
  - If there were problems running the sample student submissions on their
    grader, what a likely fix would be. Feel free to try making the fix yourself to
    see if it would work!
  - New things you **learned** from reading their code
  - Suggestions for improving the code that don't change it's overall behavior,
    just its style, readability, or performance

**Write down** all of this feedback in the notes file. You'll go over it with
the other group next. Think about how to give any feedback about issues politely
and professionally.

In all of this communication, remember to be polite, professional, and focus on
giving detail and clear writing. A huge part of the job of a working software
professional or researcher is _accurately communicating about code and system
behavior_, and doing so in a way that is about the system and not about any
specific person.

Some tricks for this: avoid statements that reference the _author_ of the code,
frame negative feedback as possible improvements or ways your expectations were
violated, and take responsibility as the reviewer for anything you don't
understand.

Examples:

- Don't say “You made a mistake here: ...” Instead say “On line 10 for this
  sample student submission I expect the condition to be true but it's false
  because XYZ.”
- Don't say things like “It seems like you were rushing to finish...”. Instead
  say “the script looks like it might be imcomplete – it works how I'd expect up
  to line 22 and then doens't have any code to present the error messages”.
- Don't say “It seems like you don't know about...”, instead say “On line 10-12,
  these 3 lines could be shortened into one line using `grep -r` instead of `find`
  followed by `grep`: ....”
- Don't say “This code is slow...” Instead say “This grader took 10 seconds to
  run for one submission. We think this is because... and if we change... it goes
  down to 2 seconds.” If you think it's slow but don't know why, take
  responsibility as the reviewer: “This grading script took 10 seconds which I
  think is a long time. I can't figure out why, though.”
- Don't say “This conditional is ugly:...” Instead say “I find it easier to read
  these conditions when they are written as .... because ...” If you don't have a
  good explanation to put after the “because”, how do you know it's a good
  suggestion?
- Don't say “You wrote lines 20-24 very confusingly.” Instead say “We had a lot
  of trouble understanding lines 20-24. It would help us to work through an
  example of how that part is supposed to work”

### Part 3 – Discussion and Pull Request

After you write this down, the lab leaders will help reorganize your groups so
you're talking to the group you reviewed (and who reviewed your code).

Go through the feedback you wrote down in the last step, and take notes on
clarifications and answers to questions you had.

Then, as appropriate, you should make **issues** and **pull requests** to one
another's repositories summarizing the feedback. Create these pull requests and
issues _together_ with the other group, this will help everyone understand
what's written down.

Make an **issue** if there's a problem or improvement to make that _you aren't
sure how to fix_. Make sure to include the failure-inducing input, context, and
symptoms! They'll come back to this in a future week and need all that detail to
help understand and fix it. The Github instructions for making an issue are here:

[Creating an Issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue)

Make a **pull request** if you have direct code update suggestions for the other
group. A pull request is a **Github** concept for sharing code edits with
others. To make a **pull request**, first make a fork of the repository you
want to submit the pull request to. Then, make the edits and commits you want to
make, and push them to your fork. Then the Github instructions for creating the
pull request are here:

[Making a Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)

Having an issue or pull request filed for your project is not a bad thing! In
the good cases, it means someone else out there in the world (or in your
company/institution) read your code, wants to help, and has something
constructive to say about it. Of course, you have control over the code, too, so
you don't have to accept their feedback as they wrote it. You can take it as
advice, ignore it, adapt it, put it off until later, and so on. But remember
that issues and pull requests are largely positive things – they are a sign that
your project has people paying attention to it, and they are a normal and common
part of managing a software system.
