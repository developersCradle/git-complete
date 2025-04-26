
## Section 15: Rebasing: The Scariest Git Command?

Rebasing: The Scariest Git Command?

# What I Learned.

# What Really Matters In This Section.

- **Rebase** you don't need to use, but It's good to use.

- **Rebase** vs **Merging**, behaves differently.

# Why is Rebasing Scary? Is it?

- `Rebase` is either used a lot in a company or avoided by plague!

<img src="rebasing.PNG" alt="alt" width="600"/>

<br>

<img src="rebasingGoldenRule.PNG" alt="alt" width="600"/>

1. You need to know when **NOT** to use `rebasing`. There is **Golden** rule of rebasing.

<img src="gitRebaseDivide.PNG" alt="alt" width="600"/>

1. Rebase has **two** main ways of usage:
    - As **alternative** to **merging**.
    - As **cleanup** tool.

# Comparing Merging & Rebasing.

<img src="rebaseCanHelpWithThisOne.PNG" alt="alt" width="600"/>

1. There are **many** commits before we start working in our `feature` branch in the `master` branch.
2. Then we just start developing in the `feature` branch.
3. We want the `Feature` branch the commits from `Master` **at this time**!
    - This, so will **merge** commit in **purple border color**.
4. Once again we **want** stuff from the `master` branch.
    - We will **have** again the **merge** commit in the commit history!
5. There are many other **developers** working for the `master` branch, and it's **very** active. Do we really want all this **MERGE COMMITS** in our `feature` branch, which in the **end** does not say **anything** and the branch gets **muddy**.
    - In the **end** when the `feature` branch is **merged** into `master` branch, there **will** be **non informative to merge commits**, which does not say anything!

- Some documentation [Git rebase](https://git-scm.com/docs/git-rebase).

> [!IMPORTANT]
> Problem with `rebase` is that it will **re-write history**!

<img src="rebasing1.PNG" alt="alt" width="600"/>

1. **Merging** creates these **merge commits**.
2. **Rebase** re-writes the history as **one**!
    - ✅No merge commits✅.
    - ❌No time **stamps** when these were **originally** written ❌.
3. **Commits** from the `feature` branch will be added to **tip** of the `master` branch.

<img src="rebasing2.PNG" alt="alt" width="600"/>

# Rebase Demo Pt 1: Setup & Merging.

- History of commands for this demo.

```
# We init the repo for demo.
git init
# We create the website.txt.
touch website.txt
# We add the website.txt.
git add website.txt
git commit -m "init"
# We add some stuff to repo.
git commit -am "add some stuff"
# We are switching to feature branch.
git switch -c feat master
# We will be working our incredible feature.
touch feature.txt.
# We will be adding something to our feature.
git add feature.txt
git commit -m "beging feature"
# Here we have modified our feature txt in VisualStudio. We are at feat branch.
git commit -am "work on the feature"
# We are going back to master branch.
git switch master
# We add new work for the master branch.
# In this example, we add something for the website.txt and add it. We are at master branch.
git commit -am "add footer"
```



