`#assembler-school`

# Pills and Projects: Submitting a solution

In this page you will learn how to fork a project as a student and submit your solution.

## Table of Contents <!-- omit in toc -->

- [Pills and Projects: Submitting a solution](#pills-and-projects-submitting-a-solution)
  - [Forking the project](#forking-the-project)
  - [Creating the pull request with the solution](#creating-the-pull-request-with-the-solution)
  - [List of pull requests of previous solutions](#list-of-pull-requests-of-previous-solutions)
  - [Resources](#resources)

## Forking the project

First, you will need to create a fork of the base project from the Assembler School Github page.

In this example we will create a fork of the [pill-sass-clone-instagram](https://github.com/assembler-school/pill-sass-clone-instagram) pill.

Choose the account where you want to make the fork:

![Creating a fork](/src/img/pill-sass-clone-instagram/create-fork.png)

Wait for the fork to be completed:

![Creating a fork](/src/img/pill-sass-clone-instagram/forking.png)

[back to top](#pills-and-projects-submitting-a-solution)

## Creating the pull request with the solution

Then, you will need to add your solution of the pill or project by pushing the changes to the remote in your personal account.

Once you have pushed the changes to your forked copy of the pill/project you will be able to create a pull request against the original pill/project repo from the [Assembler School](https://github.com/assembler-school/) organization in Github.

In order to create the Pull Request you will need to click the Pull Request Button which will take you to the screen where you can create a pull request with the changes of your forked repo against the base repo in the Assembler School organization.

Click on the **_Pull Request_** button:

![Changes pushed](/src/img/pill-sass-clone-instagram/pr-create-first-step-highlight.png)

Then on the **_Create pull request_** button:

![Changes pushed](/src/img/pill-sass-clone-instagram/pr-create-before-step.png)

In the next screen you can write the pull request title and description:

### Solution Pull Request Title

In this example we can see that the Pull Request title contains the git message which is not correct.

The template we use in Assembler School to deliver a solution PR is the following:

```
Solution + YOUR FULL NAME
```

**Examples:**

```
Solution: John Doe
```

```
Solution: Ana Marks
```

Here you can see an example of an 😕 **_incorrect_** way of writing the pull request title.

![Changes pushed](/src/img/pill-sass-clone-instagram/pr-create-message.png)

For this step you must include a descriptive title and description about the Pull Request so that the reviewer can know what changes are being introduced with the pull request.

To learn more, see the following resources:

- [Writing good CL descriptions](https://google.github.io/eng-practices/review/developer/cl-descriptions.html)
- [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/)
- [Assembler School: Code Review Best Practices](https://github.com/assembler-school/code-review-best-practices/blob/main/src/code-review-best-practices.md)

### Example of a pull request description and title:

**PR Title**

```
Solution: Ana Marks
```

**PR Description**

```txt
Summarize changes in around 50 characters or less

More detailed explanatory text, if necessary. Wrap it to about 72
characters or so. In some contexts, the first line is treated as the
subject of the commit and the rest of the text as the body. The
blank line separating the summary from the body is critical (unless
you omit the body entirely); various tools like `log`, `shortlog`
and `rebase` can get confused if you run the two together.

Explain the problem that this commit is solving. Focus on why you
are making this change as opposed to how (the code explains that).
Are there side effects or other unintuitive consequences of this
change? Here's the place to explain them.

Further paragraphs come after blank lines.

 - Bullet points are okay, too

 - Typically a hyphen or asterisk is used for the bullet, preceded
   by a single space, with blank lines in between, but conventions
   vary here

If you use an issue tracker, put references to them at the bottom,
like this:

Resolves: #123
See also: #456, #789
```

To finish creating the Pull Request, you should click on the **_Create pull request_** button:

![Pull request created](/src/img/pill-sass-clone-instagram/pr-create-message-click.png)

Now, your pull request was created and waiting for feedback 🎉.

![Pull request created](/src/img/pill-sass-clone-instagram/pr-created.png)

[back to top](#pills-and-projects-submitting-a-solution)

## List of pull requests of previous solutions

Now you will be able to see the pull request you have just created along with the solutions of other students.

You can also see an example of a **_correct_** ✅ (`Solution: Pau Garcia Pellicer`) and **_incorrect_** 😕 (`feat: add the solution of the project`) solution pull request title.

![List of PR solutions](/src/img/pill-sass-clone-instagram/pr-list-of-solutions.png)

### Important things to consider

1. Never provide a solution PR before the due date of the pill/project
2. Always read all the instructions of the pill/project
3. Make sure you always follow software design principles and patterns
4. Don't copy the solution of you colleagues, you should always solve the pill/project by yourself
5. Be nice and give constructive feedback

[back to top](#pills-and-projects-submitting-a-solution)

## Resources

[Learn more about code reviews](../README.md#resources)
