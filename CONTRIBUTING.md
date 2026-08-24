# How to contribute

First of all, thank you for thinking about contributing! Here you'll find a set of guidelines
that apply to all Touchlab open source projects.

This is the default guide shared across Touchlab repositories. Individual repos may ship their own
`CONTRIBUTING.md`, which takes precedence over this one.

## Ways to help

### Creating an issue

If you've found a bug, please open an issue from the repository's
**Issues** tab and fill in the **issue template** carefully. The more complete your response, the easier
it is for us to address the issue and the less likely it is to stall.

Please don't use issues as a general Kotlin or KMP helpline; general questions are better asked in
Slack (see [Questions](#questions)). There may be a delay before we get to your ticket, so we ask
for your patience.

### Requesting New Features

Adding new features and functionality requires additional community discussion. For this reason we
ask that feature requests be submitted to the repositories Feature Request (or Ideas) Discussion forum 
before starting a PR and instead of through the repositories issue list.

Submitting feature requests as discussions allows us prioritize requests using discussions upvote system. 
Requests with a lot of community support are more likely to be considered. It also provides a distinction 
between defects (issues) which concretely fixable, and enhancements which may be valid but not prioritized.

### Submitting a pull request

If you'd like to contribute code, a good place to start is issues tagged **help wanted**. If
there are none open, pick an issue that looks like a reasonable fit for your experience with the
project.

If you're proposing significant changes or new features
please open a discussion before committing time/effort to the change so that we can discuss whether it's
something likely to be merged.

When your fix or feature is ready:

* Open the pull request against the repository's default branch and fill in the
  **pull request template** with as much detail as you can.
* Reference the issue/discussion number
* Keep the change focused. One concern per pull request; unrelated cleanups are easier to accept
  separately.
* Include tests for behavior you add or fix, where the project has a test suite for that area.
* Mention any platform you couldn't build or test locally.

All pull requests need a code review from a Touchlab team member, and are then approved, sent back
with comments, or declined with a reason. It might take some time before we get to it. Contributions are accepted under the same license as the project.

## Before submitting code

### Build and run tests locally

The repo's `README.md` is the source of truth for how to build it, which toolchain versions it
expects, and any setup a build needs. Whatever those commands are, we expect the same things of a
contribution:

* **Build it and run the tests before opening a pull request.** Don't rely on CI to find out whether
  your change compiles.
* **Use the build tooling the repo ships with** — the checked-in wrapper, lockfile, or pinned
  toolchain version — rather than whatever is installed globally on your machine. Version drift
  produces failures that have nothing to do with your change.
* **Cover every platform the project targets**, not just the one you develop on. Some targets need
  specific hardware or SDKs (for example, Apple targets need a Mac with Xcode). If you can't run one
  locally, run what you can and say in the pull request which platforms you didn't verify, so a
  reviewer knows what to watch.
* If a setup step isn't documented and you get stuck, open an issue or ask in Slack. A missing setup
  step is a bug in our docs, not a failure on your part.

### Formatting and static analysis

Match the conventions the project already uses. Most of our repos configure a formatter and static
analysis as part of the build, and the same checks run in CI — run them locally before you push, and
prefer letting the configured tool format your code over formatting it by hand.

Some existing files may not conform to the current standard. Please be careful about reformatting
them as part of your change — when a diff contains many reformatted lines, the actual change gets
lost during review. Don't reformat, rename, or clean up code you aren't otherwise touching. If a
file genuinely needs a formatting pass, keep it in its own commit or its own pull request.

## Response times

While we're proud of our open source projects, we only have so much time to contribute to them.
These projects are maintained alongside our client work, so treat the following as our intent rather
than a guarantee:

* We aim to acknowledge new issues and pull requests within about a week.
* Security reports and regressions in a recent release get looked at first.
* Quiet periods happen. If something has gone a couple of weeks without a response, a polite bump on
  the issue or a message in Slack is welcome and won't annoy us.
* Some repositories are maintained more actively than others. If a repo is in low-maintenance or
  archived mode, its `README.md` will say so — for those, expect responses to be slower and
  larger changes unlikely to be merged.

If your team depends on one of these projects and needs a firmer commitment,
[reach out to Touchlab](https://go.touchlab.co/contactkamp) to discuss support options.

## Questions

If you have any questions, please contact us in the Kotlin
[Community Slack](https://kotlinlang.slack.com/) in the
[#touchlab-tools](https://kotlinlang.slack.com/archives/CTJB58X7X) channel. To join the Kotlin
Community Slack, [request access here](http://slack.kotlinlang.org/).

For direct assistance, please [reach out to Touchlab](https://touchlab.co/contact-us) to discuss
support options.
