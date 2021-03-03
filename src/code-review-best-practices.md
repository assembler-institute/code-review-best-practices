`#assembler-school`

# Assembler School: Code Review Best Practices

In this page you will see several best practices and tips & tricks on doing code reviews in way that is professional, mindful of your colleagues feelings and that it ensures that the code base of your team doesn't deteriorate in time.

## Table of Contents <!-- omit in toc -->

- [Assembler School: Code Review Best Practices](#assembler-school-code-review-best-practices)
  - [What is a code review?](#what-is-a-code-review)
  - [Key points to consider when doing code reviews](#key-points-to-consider-when-doing-code-reviews)
  - [Why are code reviews hard?](#why-are-code-reviews-hard)
  - [Leave a good description about the changes made in the Pull Request.](#leave-a-good-description-about-the-changes-made-in-the-pull-request)
  - [Automate the boring stuff](#automate-the-boring-stuff)
  - [Review time](#review-time)
  - [Try to keep reviews under ~400 lines of code](#try-to-keep-reviews-under-400-lines-of-code)
  - [Focus first on the higher level issues and then go deeper](#focus-first-on-the-higher-level-issues-and-then-go-deeper)
  - [Always try to include code examples in the notes](#always-try-to-include-code-examples-in-the-notes)
  - [Never use the word "you" in code reviews](#never-use-the-word-you-in-code-reviews)
  - [Frame feedback as requests or suggestions, not commands](#frame-feedback-as-requests-or-suggestions-not-commands)
  - [Notes should reflect software design principles and not opinions or personal preferences](#notes-should-reflect-software-design-principles-and-not-opinions-or-personal-preferences)
  - [Don't look for improving from a 5 to a 10](#dont-look-for-improving-from-a-5-to-a-10)
  - [Limit the review to the scope of the changelist](#limit-the-review-to-the-scope-of-the-changelist)
  - [Don't focus only on whats wrong with the code and appreciate what is done](#dont-focus-only-on-whats-wrong-with-the-code-and-appreciate-what-is-done)
  - [Resources](#resources)

## What is a code review?

A `code review` is an activity which usually involves an **author** of the code and a **reviewer** in charge of reading the author's code and deciding when the changes are ready to be merged in the projects code base.

Before the author submits a code review, the author must create a **changelist** that includes a set of changes to source code that the author wants to merge in to the team's codebase.

A review begins when the author sends their changelist to the reviewer. Code reviews happen in **rounds**. Each round is one complete round-trip between the author and reviewer: the author sends changes, and the reviewer responds with written feedback on those changes. Every code review has one or more rounds.

The review ends when the reviewer **approves** the changes. This is commonly referred to as giving LGTM, shorthand for "**Looks Good to Me.**"

[back to top](#assembler-school-code-review-guide)

## Key points to consider when doing code reviews

The main objective of doing code reviews is to make sure that the overall code health of your team's code is improving over time. It's not about showing off the skills or knowledge of a reviewer or author, it's about learning together as a team and improving the overall skill level and code quality.

- [ ] Reviewers should not be a barrier for integrating code into the code base
- [ ] Developers should be able to make progress and add new features to the app
- [ ] The overall code health should not deteriorate with each change
- [ ] Reviewers should favor approving a changelist if it doesn't deteriorate the overall code health
- [ ] There is no such thing as perfect code
- [ ] Code should improve the readability, maintainability and understandability of the overall system
- [ ] Are the main software principles being respected?
- [ ] Is the code too complex and over-engineered? If the author adds features or logic that is not currently needed, the reviewers should be vigilant and encourage developers to solve the problem that needs to be solved now and not include any premature optimization.
- [ ] Is the code tested?
- [ ] Are tests testing the wright thing?
- [ ] Are tests too complex?

## Why are code reviews hard?

When an programmer sends a changelist to be merged in the projects code base, they are very excited of the work they have made and think that their code is awesome. Then, the reviewer has to evaluate all the work that the author made and even suggest changes which might hurt the authors ego and pride.

It's easy to interpret criticism and take it personal thinking that you are a bad programmer. But that is not the best way to handle things. The changes are not a personal attack, its a struggle between the author and the reviewer to ensure that the code meets the teams standards and quality level.

It's important to let the author know that the job of the reviewer is not only to catch bugs and see whats wrong with the code of the author, but to help him/her to keep going and to integrate the changelist in a way that helps improve the overall codebase to ensure code quality and standards are met.

Furthermore, since everything is usually made in writing and not in a face to face conversation we need to take extra care of how we say things to not hurt the authors feelings when the risk of miscommunication can be high.

[back to top](#assembler-school-code-review-best-practices)

## Leave a good description about the changes made in the Pull Request.

Include screenshots, comments, issue link or `#id`, commands needed to setup the code, etc such that the code reviewer has all the context needed to be able to review the code.

[back to top](#assembler-school-code-review-best-practices)

## Automate the boring stuff

Humans should not have to check parts of the code that can be automated by tools. This includes formatting, linting and checking for bugs or misspelled variables, checking if the tests are running for the entire code base, running continuous integration, etc.

Us as developers should be reviewing much more complicated and higher level aspects of our code such as checking if the overall architectural design of the code is well thought of, if the coding standards of the team are being followed and much more.

Our time as developers is valuable and limited so we need to automate most of the boring and repetitive aspects of our code so that we can better spend our time on tasks that **tools can't check for us**.

We shouldn't spend time discussing whether to use spaces or tabs, we should define a style guide that our entire team uses and serves as a go-to when we don't know which direction to follow.

All these tools should ideally execute as soon as possible to catch all the issues and bugs that our code might have. This way our feedback loop is as short as possible.

**What are feedback loops?**

Feedback loops tell your team whether or not their development efforts are paying off. The faster and more detailed the feedback, the more information your team has to make corrections and improve the application.

Following this principle, as developers, we need automated tools that report any issues with our code **while we are writing** it so that we can **fix them right away and not latter** when tests report a bug.

### Linters

**Javascript**:

- [ESLint](https://eslint.org/)

**PHP**:

- [ ] TODO

**SCSS**:

- [ ] TODO

### Formatters

**Javascript**:

- [Prettier](https://prettier.io/docs/en/configuration.html)

**PHP**:

- [ ] TODO

**SCSS**:

- [ ] TODO

### Automated tools

Git Hooks that validate the code on each git event

- [Husky](https://github.com/typicode/husky)

Run linters on git staged files

- [Lint Staged](https://github.com/okonet/lint-staged)

Unit and Integration Testing

- [Jest](https://jestjs.io/)

End To End Testing

- [Cypress](https://www.cypress.io/)

### Style Guides

We shouldn't waste time debating whether to use single or double quotes, 2 spaces or 4 spaces or any other code style related arguments in code reviews. Instead, we should use a style guide that already exists –or create our own– that includes all the formatting rules for the languages we code our app with.

Some examples of Javascript Style Guides include:

#### Airbnb JavaScript Style Guide

- [Javascript Style Guide](https://github.com/airbnb/javascript)
- [React.js Style Guide](https://github.com/airbnb/javascript/blob/master/react)
- [CSS-in-JavaScript Style Guide](https://github.com/airbnb/javascript/tree/master/css-in-javascript)
- [CSS / Sass Style Guide](https://github.com/airbnb/css)

[back to top](#assembler-school-code-review-best-practices)

## Review time

Code reviews should be your top priority. Any time the code spends in code review is time wasted because the code isn't used in production and all the effort of the author is wasted.

When you receive a code review request you should start right away with it so that the author can know if any changes are required. The same principle applies to you as an author, when a reviewer requests changes, you should get to it as soon as possible.

**A single review round should not be any longer that one business day**.

If the reviewer can't respond quickly he/she should let the author know so that another reviewer can be assigned to take over.

[back to top](#assembler-school-code-review-best-practices)

## Try to keep reviews under ~400 lines of code

The ideal code reviews is between 10 to 100 lines of code or under an hour of. It could extend up to 200 - 400 lines of code but it is discouraged and you should try to get the author to divide it into several parts.

---

```text
10 lines of code = 10 issues.

500 lines of code = "looks fine."
```

Because Code reviews.

---

[back to top](#assembler-school-code-review-best-practices)

## Focus first on the higher level issues and then go deeper

Each review round should not have too many notes. Usually having 20-50 notes in a review means that there are too many changes being requested from the author.

Therefore, first wait for higher level changes to be solved before going for lower-level issues such as variable naming or clarity of code.

This is important because by the time the higher level notes have been solved, the lower level ones might also have been taken care of through refactoring.

[back to top](#assembler-school-code-review-best-practices)

## Always try to include code examples in the notes

Instead of just saying that the code needs improvements with a particular style of code or functionality, try to be more specific and even include code examples of how the author might solve the change that is requested by the reviewer.

One great example taken from [How to Do Code Reviews Like a Human | Michael Lynch](https://www.youtube.com/watch?v=0t4_MfHgb_A) is the following:

---

Imagine that you have a colleague who is not familiar with the list comprehensions feature of Python. They send you a code review that includes these lines:

```python
urls = []
for path in paths:
  url = 'https://'
  url += domain
  url += path
  urls.append(url)
```

Responding, "Can we simplify this with a list comprehension?" will annoy them because now they have to spend 20 minutes researching something they've never used before.

They will be much happier to receive a note like the following:

Consider simplifying with a list comprehension like this:

```python
urls = ['https://' + domain + path for path in paths]
```

---

This idea can be expanded to more than a single line of code. You can even include a demo repo showing the author how the changes could be implemented such as splitting a large function into smaller parts and adding a test for an edge case.

Try to not include more than two or three code examples per review round otherwise the author might consider that you are writing the code for them.

[back to top](#assembler-school-code-review-best-practices)

## Never use the word "you" in code reviews

Such that the author doesn't take the comments personally, we should always avoid the use of the word "you" and replace it with "we".

The changes that are included in the changelist should be focused on making the overall code base better and not on who made it. This shifts the focus from code made by a person that represents that person to trying to improve the code base.

The natural reaction of a developer that receives criticism for their work is to became defensive and protective of their code. By avoiding the use of "you" we ensure that they don't feel judged personally.

### Examples of rewording the feedback we give:

**_Replacing 'you' with 'we'_**

> Can **you** rename this variable to something more descriptive, like `signInUserData`?

becomes:

> Can **we** rename this variable to something more descriptive, like `signInUserData`?

"We" reinforces the team's collective responsibility for the code. The author may move on to a different company and so might you, but the team who owns this code will remain in one form or another.

**_Removing the subject from the sentence_**

Another way to avoid using "you" is to use a shorthand that omits the subject from the sentence by using suggestions:

> **Suggest renaming** to something more descriptive, like `signInUserData`.

Or by using [passive voice](https://en.wikipedia.org/wiki/English_passive_voice):

> This variable **should be renamed** to something more descriptive, like `signInUserData`.

Or phrasing it as a question, beginning with "what about..." or "how about...":

> **What about renaming** this variable to something more descriptive, like `signInUserData`?

[back to top](#assembler-school-code-review-best-practices)

## Frame feedback as requests or suggestions, not commands

In code reviews we should try to be much more gentle and nice than in real life to avoid framing the notes as requests such as:

> Change this code to something more readable

To requests that are more of a suggestion:

> Can we restructure this code so that it is easier to read?

[back to top](#assembler-school-code-review-best-practices)

## Notes should reflect software design principles and not opinions or personal preferences

If the code that the author wrote could be improved by following a software design pattern or principle you should include it as an example so that the notes of the reviewer are more constructive.

### Common principles

- [YAGNI](https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it)
- [KISS](https://en.wikipedia.org/wiki/KISS_principle)
- [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)
- [S.O.L.I.D.](https://en.wikipedia.org/wiki/SOLID)
- [Encapsulation](<https://en.wikipedia.org/wiki/Encapsulation_(computer_programming)>)
- [Functional programming](https://en.wikipedia.org/wiki/Functional_programming)
- [Fail Fast](https://enterprisecraftsmanship.com/posts/fail-fast-principle/)

When you give the author a note, explain both your suggested change and the _reason_ for the change, this way your feedback is always constructive.

Instead of saying:

- "We should split this class into two"

It's better to say:

- "Right now, this class is responsible for both downloading the file and parsing it. We should split it up into a downloader class and parsing class per the [single responsibility principle](https://en.wikipedia.org/wiki/Single_responsibility_principle)."

[back to top](#assembler-school-code-review-best-practices)

## Don't look for improving from a 5 to a 10

Rather than asking the author to improve in all the ways possible and going from a 5 out of 10 straight to a 10 out of 10 try to focus on small incremental increases of knowledge.

If you ask too much from the author his/her patience will drain out very quickly. Give them an opportunity to grow incrementally.

[back to top](#assembler-school-code-review-best-practices)

## Limit the review to the scope of the changelist

If during the review you as a reviewer see any opportunities for improvement in code that is not directly affected by the authors code you should not request any changes to it. The author is only concerned by the changes he/she made.

[back to top](#assembler-school-code-review-best-practices)

## Don't focus only on whats wrong with the code and appreciate what is done

Most reviewers focus only on what's _wrong_ with the code, but reviews are a valuable opportunity to reinforce positive behaviors.

You don't need to have a specific goal in mind to offer praise. Any time I see something in the changelist that delights me, I tell the author about it:

- "I wasn't aware of this API. That's really useful!"
- "This is an elegant solution. I never would have thought of that."
- "Breaking up this function was a great idea. It's so much simpler now."

If the author is a junior developer or joined the team recently, they're likely to feel nervous or defensive during a review. Sincere compliments ease this tension by demonstrating that you are their supportive teammate and not the cruel gatekeeper.

[back to top](#assembler-school-code-review-best-practices)

## Resources

[Learn more about code reviews](../README.md#resources)
