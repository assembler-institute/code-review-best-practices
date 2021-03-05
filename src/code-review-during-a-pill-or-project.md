`#assembler-school`

# Code review during a pill or project

In this page you will learn how to code review the pull requests made to a pill/project while you are working on it.

## Table of Contents <!-- omit in toc -->

- [Code review during a pill or project](#code-review-during-a-pill-or-project)
  - [First steps](#first-steps)
  - [How are new features added to a project?](#how-are-new-features-added-to-a-project)
  - [Authoring a pull request that doesn't require changes](#authoring-a-pull-request-that-doesnt-require-changes)
  - [Authoring a pull request that requires changes to be made](#authoring-a-pull-request-that-requires-changes-to-be-made)
  - [Resources](#resources)

## First steps

Before you write the feedback you should always make sure that you have read the [code review best practices guidelines](./code-review-best-practices.md).

Always remember to give helpful and constructive feedback. `#be-nice`

[back to top](#code-review-during-a-pill-or-project)

## How are new features added to a project?

At Assembler School we recommend that any new change made to a code base is done through [Pull Requests](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests).

This way, whenever you are working in a team you can review each others code before merging it into the `main` branch.

## Authoring a pull request that doesn't require changes

First we will see how to handle a pull request that the reviewer doesn't request any changes from the author.

### Pull request code review

In order to integrate your changes into the project you will first need to add your feature using a feature branch and then push it to the remote repo.

### Authoring a pull request

![Compare and pull request](/src/img/semantic-html/author/01-semantic-html-compare-and-pr.png)

Then, the Github UI should show you a button to create a pull request based on the feature branch.

Click on the `Compare & pull request` button to start creating the PR.

Once the new PR screen is opened you will need to write the PR title and description.

![Writing a pull request](/src/img/semantic-html/author/02-semantic-html-pr-open.png)

Then you will need to ask a reviewer to review your changes:

![Writing a pull request](/src/img/semantic-html/author/03-semantic-html-pr-add-reviewers.png)

Once the title, description, reviewer and any other options are added to the PR you can now create it by clicking on the `Create pull request` button.

![Creating the pull request](/src/img/semantic-html/author/04-semantic-html-pr-create.png)

Now, you PR has been created and you can review it and optionally edit any details if you missed any step.

![Pull request created](/src/img/semantic-html/author/05-semantic-html-pr-created.png)

If you take a look at the PR you can merge it until the reviewer that was assigned approves the changes.

![PR Blocked](/src/img/semantic-html/author/06-semantic-html-pr-blocked.png)

[back to top](#code-review-during-a-pill-or-project)

### Reviewing the pull request

The next step is in the hands of the reviewer now because he/she has to evaluate the changes and see if the PR can be integrated into the project.

For the next steps you will switch roles to be the reviewer of the pull request.

If the author of the PR assigned you as a reviewer you should be able to see the notification in the Github UI.

To start, click on the `Add your review` button.

![Reviewer side details](/src/img/semantic-html/reviewer/01-semantic-html-reviewer-side.png)

If you open the `Pull requests` tab in Github yo should see the PR that was just created.

![PR list](/src/img/semantic-html/reviewer/02-semantic-html-pr-created.png)

First, you will need to take a look at all of the files changed in the PR to see if it follows the coding standards of your team.

![Reviewer side details](/src/img/semantic-html/reviewer/03-semantic-html-changes.png)

Once you have reviewed the code you should add any notes about the PR and give the author your feedback.

![Writing the feedback](/src/img/semantic-html/reviewer/04-semantic-html-writing-feedback.png)

You can also click on the `Preview` button to see how the rendered markdown is like.

![Reviewing the feedback provided](/src/img/semantic-html/reviewer/05-semantic-html-feedback-review.png)

After viewing all the changes in each file, you can click on the `Viewed` button so that you know that you are done reviewing the file and move on with the next one.

![Set the file as viewed](/src/img/semantic-html/reviewer/06-semantic-html-file-viewed.png)

Once you are done with writing the notes of the PR you can now decide if you want to approve it, add a comment or request changes before it is ready to merge.

![Approving the pull request](/src/img/semantic-html/reviewer/07-semantic-html-pr-approve.png)

[back to top](#code-review-during-a-pill-or-project)

### Receiving the feedback from the reviewer

Now we will switch back to being the author of the PR.

If we open the PR details we can see that the reviewer has approved our PR with the following feedback.

![Pull request approved](/src/img/semantic-html/author/07-semantic-html-pr-approval-message-details.png)

Now we can see that we can merge the PR because the reviewer approved it.

![Changes approved merge options](/src/img/semantic-html/author/08-semantic-html-pr-approved.png)

If we click on the dropdown icon we can see the other options we have to integrate the PR.

![Merging options](/src/img/semantic-html/author/09-semantic-html-pr-merge-options.png)

Then you will have to confirm the merge to finish.

![Confirming the merge](/src/img/semantic-html/author/10-semantic-html-pr-confirm-merge.png)

As a last step you will have to delete the branch.

![Confirming the merge](/src/img/semantic-html/author/11-semantic-html-pr-delete-branch.png)

You can also configure the repository to automatically delete branches after they are merge with the following configuration.

![Auto delete head branches](/src/img/semantic-html/author/12-automatically-delete-branches.png)

Now if you open the `Pull requests` tab in the Github UI you can see that the previous PR isn't there anymore.

![Seeing the currently open prs](/src/img/semantic-html/author/13-semantic-html-pr-open-list.png)

However in the closed pull requests tab you will be able to find it and see its details.

![Seeing the currently closed prs](/src/img/semantic-html/author/14-semantic-html-pr-closed-list.png)

![Seeing the details of the closed pr](/src/img/semantic-html/author/15-semantic-html-pr-closed-details.png)

[back to top](#code-review-during-a-pill-or-project)

## Authoring a pull request that requires changes to be made

In this part we will see how to handle a pull request that the reviewer requests changes from the author before the PR can be merged.

### Creating the PR as an author

First, you will need to push the branch to the remote repo and create a PR just like before.

![Creating the pr](/src/img/form/author/01-form-create-pr.png)

Once you have created it you should see it in the pr list.

![Seeing the pr list as an author](/src/img/form/author/02-form-pr-list.png)

### Receiving the pr review as a reviewer

Now we will switch gears to become the reviewer.

Once that the author has requested your review, you as a reviewer will be able to see a new pr in the Github page.

![Seeing the pr list as a reviewer](/src/img/form/reviewer/01-form-pr-list.png)

And the notification that there is a new review request for you as a reviewer.

![Seeing the pr notification](/src/img/form/reviewer/02-form-reviewer-requested.png)

If you open the files changed in the pr you can write your feedback. In this case the reviewer requests changes to be made before they can be merged.

![Writing the feedback](/src/img/form/reviewer/03-form-writing-feedback.png)

Once you are finished with the review note click on the `Start a review` button.

![Starting the review](/src/img/form/reviewer/04-form-start-review.png)

Now the feedback should be added.

![Review added](/src/img/form/reviewer/05-form-feedback-added.png)

Now you will be able to finish the review by clicking on the `Finish your review` dropdown, then on the `Request changes` option and finally on the `Submit review` button.

![Finish the review](/src/img/form/reviewer/06-form-finish-review.png)

The feedback should now appear in the pr details.

![Finish the review](/src/img/form/reviewer/07-form-feedback-requested.png)

Once the feedback is added, the author should see it in the pr's details.

![Author read feedback](/src/img/form/author/03-form-read-feedback.png)

Then the author can choose to provide a first response.

![Author first response](/src/img/form/author/04-form-author-first-response.png)

In the next step the author has to solve all the requested changes and push the commit to the same branch from which the PR was initially created.

In this screenshot we can see how the author has pushed a new commit with the changes.

![Author response commit](/src/img/form/reviewer/08-form-author-response-commit.png)

### Review the updates made by the author

Now the reviewer can check that the updates made by the author are what he requested initially and provide a feedback.

![Reviewer responding to the update](/src/img/form/reviewer/09-form-responding-to-update.png)

Once the reviewer is done checking the changes in the file he/she can mark it as `Viewed`.

![Reviewer adding a review](/src/img/form/reviewer/10-form-finish-update-review.png)

Now the changes can be approved because the author solve them in the latest commits.

![Reviewer approving the updates](/src/img/form/reviewer/11-form-approve-update.png)

And the pr can be merged.

![Reviewer merge updates](/src/img/form/reviewer/12-form-merge-pr.png)

![Reviewer confirm merge](/src/img/form/reviewer/13-form-confirm-merge.png)

And as a final step, the pr's branch can be removed.

![Reviewer delete branch](/src/img/form/reviewer/14-form-delete-branch.png)

### Done 🎉

You now know how to code review the work done in your teams code base.

## Resources

[Learn more about code reviews](../README.md#resources)
