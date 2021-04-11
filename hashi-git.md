## What are the differences between git push, git pull, and git fetch?

A quick overview:
- Use `git fetch` and `git pull` to bring changes from a different repository into your local repository.
- Use `git push` to send changes from your local repository to a different repository.

`git fetch` and `git pull` both bring in changes, so let's look at them first. When you run `git fetch` you specify a target branch. Git collects any changes in the target branch that do not currently exist in your current branch, and adds these changes to your local repository. These changes are now available for you to preview, add to a new branch, or, most likely, merge into your current working branch.

`git pull` is a combination of two commands: first `git fetch` and then `git merge`. When you run `git pull`, git first fetches any changes from the target branch, and then git automatically merges these changes into your current working branch.

While `git fetch` and `git pull` both bring changes in, `git push` sends changes out. When you run `git push` you specify a remote repository and a branch to push your changes to. You can specify a remote repository and branch inline as part of your `git push` command, or by configuring your local repository settings. After running `git push` your changes will be available in the specified repository and branch.