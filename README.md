[![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)](https://generalassemb.ly/education/web-development-immersive)

# Instructions for Using the Project Issue Tracker

During project periods, you may find yourself stuck or needing help.
Never fear! The consulting team will answer questions and help you fix bugs.

To manage requests for assistance, the team uses GitHub's 'Issues' feature -
this allows us to address issues asynchronously in an intelligent way.

## Before You Create a New Issue (i.e. 'Due Diligence')

Before you add a new issue to the tracker,
the team will expect you to go through the following checklist;
this will help make the process more efficient
by allowing the team to spend most of its time on hard issues,
rather than easy ones.

### 1.  Run your linter

  It sounds obvious, but being consistent with this will save everyone a lot of
  time. Whether you use the linter built into Atom, `grunt nag`, `rubocop`, or
  something else.

### 2.  If you have tests, run them

  Test your front-end with `grunt test`; test your back-end with either
  `bundle exec rspec` (Rails) or `jasmine-node spec` (Express).

### 3. If you have an error message, read the error

  Error messages are great, because they tell you what's going wrong.
  Take note of
    (a) what type of error you have,
    (b) what file it occurred in, and
    (c) the line and character numbers at which the error occurred.

### 4. Use your debugger to see where the error appears

  Debugging tools exist for a reason! Drop in a `debugger;` (JS)
  or a `binding.pry` (Ruby) and see if you can figure out
  how far the program runs before it hits the error.
  This can also help you check the values of variables as you go.

### 5. Read through the documentation

  Every tool we use has some sort of documentation available.
  Many documentation sources even implements a search feature,
  so that you don't have to go digging. _**Read them carefully!**_
  The function signatures in particular are very useful
  since they explain what inputs a function is supposed to take;
  passing a function the wrong input value(s) is a very common error.

### 6. Search Google and Stack Overflow for your issue

  You're probably not the first person to ever encounter your issue.
  Try copying the content of your error message (in quotes) into a search bar;
  you might be surprised what turns up.

### 7. Ask a peer

  See if any of the other developers have encountered a similar issue -
  you are all working on more-or-less the same thing,
  so they may already have the solution to your specific problem.

### 8. Read/search closed issues

  Similar to the previous one, but in case other developers aren't around, you
  can actually sift through other issues and see if a solution exists by
  clicking on `Issues` and then `3 Closed` at the top.

## How to Use the Issue Tracker

Directions for each project can be found in a repo ending in `...-project`,
and this is also where issues relating to that project will be handled.

To create a new issue and request assistance,

1.  Go to the 'Issues' tab and click 'New Issue'.

1.  Create a title for your issue.

    Please try to use the following format:

    > "\[ language or framework you're using \] -
    > \[ short (< 80 chars) description of issue \]"

1.  Give a description of the issue you've got.

    Please try to use the following format:

    > Linter Output:
    >
    > \[ output from `grunt nag`/`rubocop` \]
    >
    > Issue Description:
    >
    > \[ what you were doing when the problem showed up \]
    >
    > \[ error message, if one exists \]
    >
    > \[ things you've tried to fix the problem \]
    >
    > \[ the last point at which the app was working \]
    >
    > \[ screenshots are helpful, but be sure to include actual code as well \]
    >

1.  Click 'Submit New Issue'.

## "What should I do while I'm waiting for assistance?"

If possible, work on something else!
Hopefully, you've been using version control effectively,
so you have multiple different branches for working on different features.
In that case, just switch to a different feature branch and start working.

Another possibility, if you want to keep working on the same feature,
is to use `git stash` (to temporarily store uncommitted changes)
and `git checkout` to go _back in time_ to a previous commit --
specifically, the last time everything was working.
Once there, you can create a new branch (or branch**es**) off of that commit,
so that you can experiment with other ways to solve the problem.

Whatever you do, don't sit around waiting.
Project time is limited, so try to use it as effectively as possible.

## [License](LICENSE)

Source code distributed under the MIT license. Text and other assets copyright
General Assembly, Inc., all rights reserved.
