# Projekti4

## Branch Protection Rules

The `main` branch is protected to ensure code quality and stability.

- Direct commits to `main` are not allowed.
- All changes must be introduced via a Pull Request from another branch.
- Each Pull Request requires at least one review before it can be merged.
- Pull Requests must be merged by someone other than the author.

## Working with Branches & Pull Requests

### If you accidentally commit to `main`
Undo the last commit while keeping your changes staged:

~~~bash
git reset --soft HEAD~1
~~~

Create a new branch:

~~~bash
git checkout -b task-name
~~~

Commit your changes:

~~~bash
git add .
git commit -m "Your commit message"
~~~

Push the branch:

~~~bash
git push -u origin branch-name
~~~
