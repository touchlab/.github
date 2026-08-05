---
name: Bug report
about: Report a bug
title: ''
labels: ''
assignees: ''

---

The following template contains guiding questions that should help you provide as much helpful information as possible. 

You don't have to follow the template, you can just write the bug report and check this template to see if the bug report answers all the relevant questions. Don't worry if you don't know some answers; we will help you find them if needed.

## Questions:

### What is the problem?

For example:
- a crash
- a warning
- the generated code is incorrect, missing, etc.

Don't forget to describe the problem in more detail.

For crashes, please include the error message and the stack trace. (To get a stack trace from a Gradle task, you might need to use the `--stacktrace` parameter.)

### When does the problem occur?

For example:
- During the Gradle's configuration phase (for example, after syncing the project)
- During Kotlin Framework compilation (inside the link task that produces the framework)
- During other Gradle tasks (other than the link task mentioned above)

### How do we reproduce the issue?

If the problem is related or caused by some specific Kotlin declaration (a class, enum, function, etc.), please include an example of such a declaration.

### What versions of Kotlin and Gradle do you use?

### If applicable how is the library configured?
