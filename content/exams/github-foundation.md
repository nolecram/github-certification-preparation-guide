# GitHub Foundation

> These are **NOT real questions** from the exam but are designed to help you prepare and understand the certification topics.

## Skills measured

- [Understand repositories, branches, and commits](#understand-repositories-branches-and-commits) (30% of the exam)
- [Manage pull requests and resolve conflicts](#manage-pull-requests-and-resolve-conflicts) (25% of the exam)
- [Collaborate using issues and labels](#collaborate-using-issues-and-labels) (20% of the exam)
- [Use Git commands for version control](#use-git-commands-for-version-control) (25% of the exam)

## Understand repositories, branches, and commits

### How to create a new repository on GitHub?

<details><summary>show</summary>
<p>

1. Go to your GitHub account.
2. Click on the **New** button in the repositories section.
3. Fill in the repository name, description, and visibility settings.
4. Click **Create repository**.

</p>
</details>

### How to create a branch in Git?

<details><summary>show</summary>
<p>

```bash
git checkout -b <branch-name>
```

</p>
</details>

### How to commit changes in Git?

<details><summary>show</summary>
<p>

```bash
git add .
git commit -m "Your commit message"
```

</p>
</details>

## Manage pull requests and resolve conflicts

### How to open a pull request on GitHub?

<details><summary>show</summary>
<p>

1. Navigate to the repository on GitHub.
2. Click on the **Pull requests** tab.
3. Click **New pull request**.
4. Select the branches to compare and click **Create pull request**.

</p>
</details>

### How to resolve merge conflicts in Git?

<details><summary>show</summary>
<p>

1. Open the conflicting file in your editor.
2. Resolve the conflicts manually.
3. Stage the resolved file:

```bash
git add <file>
```

4. Commit the changes:

```bash
git commit
```

</p>
</details>

## Collaborate using issues and labels

### How to create an issue on GitHub?

<details><summary>show</summary>
<p>

1. Navigate to the repository on GitHub.
2. Click on the **Issues** tab.
3. Click **New issue**.
4. Fill in the title and description, then click **Submit new issue**.

</p>
</details>

### How to assign a label to an issue?

<details><summary>show</summary>
<p>

1. Open the issue on GitHub.
2. Click on the **Labels** dropdown.
3. Select the appropriate label.

</p>
</details>

## Use Git commands for version control

### How to clone a repository?

<details><summary>show</summary>
<p>

```bash
git clone <repository-url>
```

</p>
</details>

### How to push changes to a remote repository?

<details><summary>show</summary>
<p>

```bash
git push origin <branch-name>
```

</p>
</details>

### How to pull the latest changes from a remote repository?

<details><summary>show</summary>
<p>

```bash
git pull origin <branch-name>
```

</p>
</details>