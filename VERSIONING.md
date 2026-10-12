# Versioning

`VERSION` is the source of truth, using MAJOR.MINOR.PATCH. Version 1.0.0 establishes the baseline for this previously unversioned repository.

- PATCH: documentation, styling, bug fixes, performance, and refactoring.
- MINOR: additive user-facing functionality.
- MAJOR: breaking changes, including incompatible saved-data formats.

Every repository-file change must bump `VERSION` and update the version in the README. Commit the version change together with the implementation. About descriptions are GitHub metadata and do not require a repository release.

Requested PATCH changes may be committed and pushed to `main` after verification. MINOR and MAJOR releases require explicit owner confirmation before commit and push. Never classify a feature or breaking change as PATCH to bypass confirmation.

For documentation changes, check accuracy against the implementation and run `git diff --check`. For application changes, also check inline JavaScript syntax and verify the affected flows in desktop and phone layouts, including local saving and JSON import/export when relevant. This app has no build step or automated test suite.
