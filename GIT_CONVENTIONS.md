# Git Conventions for the ORAS Community

This guide is a specification for adding human and machine readable meaning to Pull Request and git commit messages in the ORAS community. It provides an easy set of rules for creating an explicit commit history that makes it easier to explore a more structured commit history and automatically generating CHANGELOGs for each new release. 

When contributing to the ORAS projects, please first discuss the change you wish to make via a GitHub issue, a GitHub discussion, or any other methods with the ORAS community maintainers before making a change.

> Note: Please follow the [Code of Conduct](https://github.com/cncf/foundation/blob/master/code-of-conduct.md) in all your interactions with the ORAS project, and follow the [reviewers guide](https://github.com/oras-project/community/blob/main/REVIEWING.md) when contributing to an ORAS project.

## Commit Message Guidelines

This guide provides very precise rules over how Pull Requests and git commit messages should be done.

### Commit Message Format
Each commit message consists of a **header**, a **body** and a **footer**.  The header has a special format that includes a **type**, a **scope** and a **subject**:

```
<type>[optional scope]: <subject>

[optional body]

[optional footer(s)]
```
The **header** is mandatory, and the **scope** of the header is optional. Commits MUST be prefixed with a type.

The first line of commit messages are recommended to be 52 characters or less. The maximum length of body lines should not exceed 72 characters. This allows the message to be easier to read on GitHub as well as in various git tools.

The footer should contain a [closing reference to an issue](https://help.github.com/articles/closing-issues-via-commit-messages/) if any.

Below is a complete example. For reference, you can find more [samples here](https://www.conventionalcommits.org/en/v1.0.0/#examples).

```
docs: correct spelling of CHANGELOG
```
```
fix: prevent racing of requests

Introduce a request id and a reference to latest request. Dismiss
incoming responses other than from latest request.

Reviewed-by: Z
Refs: #123
```

### Type
Must be one of the following:

* **build**: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
* **chore**: Changes that external user won't see (example: change to .gitignore file or .prettierrc file)
* **ci**: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)
* **deprecate**: Deprecates existing functionality, but does not remove it from the product
* **docs**: Documentation only changes
* **feat**: A new feature
* **fix**: A bug fix
* **perf**: A code change that improves performance
* **refactor**: A code change that neither fixes a bug nor adds a feature
* **remove**: Removes a feature from the product
* **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
* **test**: Adding missing tests or correcting existing tests

### Subject
The subject contains a succinct description of the change.

* use the imperative, present tense: "change" not "changed" nor "changes"
* don't capitalize the first letter
* no period (.) at the end

### Body
Just as in the **subject**, use the imperative, present tense: "change" not "changed" nor "changes." The body should include the motivation for the change and contrast this with previous behavior.

### Footer
The footer should contain any information about **Breaking Changes** and is also the place to reference GitHub issues that this commit **Closes**.

**Breaking Changes** should start with the word `BREAKING CHANGE:` with a space or two newlines. The rest of the commit message is then used for this.

### Revert
If you need to undo a commit, you might want to use [revert](https://www.theserverside.com/tutorial/How-to-git-revert-a-commit-A-simple-undo-changes-example). We ask for a specific format for these reverted commits too. When the commit reverts a previous commit, it should begin with `revert: ` followed by the header of the reverted commit. In the body it should say: `This reverts commit <hash>.`, where the hash is the SHA of the commit being reverted.

## References

- [Conventional Commits](https://www.conventionalcommits.org/)
- [the Angular convention](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines)
- [Conventional Commits: A Better Way](https://medium.com/neudesic-innovation/conventional-commits-a-better-way-78d6785c2e08)
