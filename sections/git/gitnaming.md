## Git
Use [Git Flow](/gitflow.md) as a reliable version control model

**Git branch naming convention:**

`<type>/<name>`

**_\<type\>_**

Allowed `<type>` values:
- `feat`:     (new feature for the user, not a new feature for build script)
- `fix`:      (bug fix for the user, not a fix to a build script)
- `docs`:     (changes to the documentation)
- `style`:    (formatting, missing semi colons, etc; no production code change)
- `refactor`: (refactoring production code, eg. renaming a variable)
- `test`:     (adding missing tests, refactoring tests; no production code change)
- `chore`:    (updating grunt tasks etc; no production code change)

**_\<name\>_**

Always use dashes to seperate words, and keep it short.

#### Examples:
```
feat/renderer-cookies
hotfix/dockerfile-base-image
bug/login-ie
```

*The commit message should be structured as follows:*

```
<type>[optional scope]: <description>

[optional body]

[optional footer]
```
Allowed `<type>` values:
- `feat`:     (new feature for the user, not a new feature for build script)
- `fix`:      (bug fix for the user, not a fix to a build script)
- `docs`:     (changes to the documentation)
- `style`:    (formatting, missing semi colons, etc; no production code change)
- `refactor`: (refactoring production code, eg. renaming a variable)
- `test`:     (adding missing tests, refactoring tests; no production code change)
- `chore`:    (updating grunt tasks etc; no production code change)

#### Examples:
```
docs: correct spelling of CHANGELOG
```
```
feat(lang): added polish language
```
```
fix: minor typos in code

see the issue for details on the typos fixed

fixes issue #12
```
[See more about commit messages](https://www.conventionalcommits.org/en/)
