`#assembler-school` `#code-reviews` `#best-practices`

# Assembler School: Code Review Guide

In this guide we will learn several best practices on doing code reviews. Bellow you can find several articles written by the Assembler School team and at the end of this README you can also find resources if you'd like to learn more about code reviews.

If you'd like to learn more about code reviews, in the [Resources](#resources) section you will find several videos and articles. The ones labelled as **_Highly Recommended_** are the ones you should see first and the ones labeled as **_Optional_** are there if you want to get a deep dive into the topic.

## Table of Contents <!-- omit in toc -->

- [Assembler School: Code Review Guide](#assembler-school-code-review-guide)
  - [Code Review Best Practices](#code-review-best-practices)
  - [Code Review Guidelines](#code-review-guidelines)
  - [What is a code review?](#what-is-a-code-review)
  - [Key points to consider when doing code reviews](#key-points-to-consider-when-doing-code-reviews)
  - [Resources](#resources)

## Code Review Best Practices

[Code review best practices](/src/code-review-best-practices.md)

In this page you will see several best practices and tips & tricks of doing code reviews in way that is professional, mindful of your colleagues feelings and that it ensures that the code base of your team doesn't deteriorate in time.

## Code Review Guidelines

[Code review guidelines](/src/code-review-guidelines.md)

In this page you will see a step-by-step guide of how to use Github to create a pull request and review the code with your team.

[back to top](#assembler-school-code-review-guide)

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

[back to top](#assembler-school-code-review-guide)

## Resources

### Linters

**Javascript**:

- [ESLint](https://eslint.org/)

### Formatters

**Javascript**:

- [Prettier](https://prettier.io/docs/en/configuration.html)

### Automated tools

Git Hooks that validate the code on each git event

- [Husky](https://github.com/typicode/husky)

Run linters on git staged files

- [Lint Staged](https://github.com/okonet/lint-staged)

Unit and Integration Testing

- [Jest](https://jestjs.io/)

End To End Testing

- [Cypress](https://www.cypress.io/)

### Airbnb JavaScript Style Guide

- [Javascript Style Guide](https://github.com/airbnb/javascript)
- [React.js Style Guide](https://github.com/airbnb/javascript/blob/master/react)
- [CSS-in-JavaScript Style Guide](https://github.com/airbnb/javascript/tree/master/css-in-javascript)
- [CSS / Sass Style Guide](https://github.com/airbnb/css)

### Videos

#### Highly recommended

- [Code Review Best Practices | JetBrains](https://www.youtube.com/watch?v=a9_0UUUNt-Y)
- [How to Do Code Reviews Like a Human | Michael Lynch](https://www.youtube.com/watch?v=0t4_MfHgb_A)
- [Buenas prácticas para hacer Code Reviews | Oscar Barajas](https://www.youtube.com/watch?v=z2WFjCwdIW4)
- [ Amazing Code Reviews: Creating a Superhero Collective | Alejandro Lujan • GOTO 2019](https://www.youtube.com/watch?v=ly86Wq_E18o)

#### Optional

- [ ] TODO

### Articles

#### Highly recommended

1. [How to Do Code Reviews Like a Human](./src/posts/how-to-do-code-reviews-like-a-human/index.md)
2. [How to Make Your Code Reviewer Fall in Love with You](./src/posts/code-review-love/index.md)
3. [Google Engineering Best Practices](./src/posts/google-eng-best-practices/index.md)

#### Optional

- [ ] TODO

[back to top](#assembler-school-code-review-guide)

## Curated by <!-- omit in toc -->

[Dani Lucaci](https://github.com/danilucaci)
