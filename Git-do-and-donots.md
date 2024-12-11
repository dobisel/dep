- Do not add any automatic generated file (ignore them by using `.gitignore`). 
- Do not force push unless you know what you do.
- Do not add binary files into the git.
- Do not add large files into the git (reset the commit if you did it).
- Do use git sub-modules to make it DRY.
- All commit messages should start with `Fix: ... `, `Feature: ...`,
  `Purge: ...`, `Refactor: ...`, `Enhancement: ...`, `Lint[: ...]`.
- Open source projects must have a proper license file to save the 
  contributors rights.
- All commits to The Master branch must always be squashed.
- Before sending any pull requests, do `make lint` and `make cover` to ensure
  100% code coverage and coding-style.
- After merging any pull request, the source branch must be deleted.
