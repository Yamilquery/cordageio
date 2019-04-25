# Segregate a context from a high-coupled-context in CQRS

In a CQRS project, sometimes we don't identify from the start our definition the necessary contexts. For that reason I decide to elaborate a mini-guide to segregate the responsibility of one particular context.

First of all, I want to share with you a GitHub repository in a particular commit in which you can see how I achieve successfully to separate a context from a high-coupled-context in a CQRS Elixir project.

https://github.com/cordageio/rigging



## 1. Modifying some files

We should modify (moving all the involved functions and renaming modules) at least 8 files from our high-coupled-context in which we want to abstract the responsibility of one context. Those files are the following:

- `lib/yourproject/application.ex`
- `lib/yourproject/router.ex`
- `lib/yourproject/high_coupled_context/high_coupled_context.ex`
- `lib/yourproject/high_coupled_context/supervisor.ex`
- `lib/yourproject_web/router.ex`
- `lib/yourproject_web/high_coupled_context/high_coupled_context_controller_test.ex`
- `lib/yourproject_web/controllers/high_coupled_context_controller_test.ex`

## 2. Moving some files

It should be necessary to move and rename the following files from the high-coupled-context to the new one:

Move from the high-coupled-context to the new one, all the involved:

- aggregates
- commands
- events
- projections
- projectors
- queries
- workflows
- validators



And that's it, good luck!
