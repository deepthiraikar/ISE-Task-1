# ISE-Task-1
## Branching and Merging Strategy for Myntra SDLC Report

## Branching Strategy

We follow the **Git Feature Branch Workflow** to maintain code quality, collaboration efficiency, and version control.

### Main Branches:
1. main: The stable branch containing the final version of the report. Only tested and approved changes are merged here.
2. develop: The integration branch where new features and updates are merged before finalizing them into `main`.

### Supporting Branches:
1. feature/<feature-name>: Created for developing new sections, enhancements, or modifications. Once completed, it is merged into `develop`.
2. bugfix/<bug-description>: Used for fixing errors or inconsistencies. Merged into `develop` after review.
3. hotfix/<hotfix-name>: Reserved for urgent fixes in `main` and merged into both `main` and `develop`.
4. release/<version-number>: A temporary branch created when preparing a final version for release. After completion, it is merged into `main` and `develop`.

## Merging Strategy

### Feature Integration:
- Developers work on feature branches and submit pull requests to `develop`.
- After peer review and approval, changes are merged into `develop`.

### Bug Fixing:
- Identified issues are addressed in **bugfix branches** and merged into `develop` after testing.
- If critical, a hotfix branch is created from `main`, fixed, tested, and merged back into both `main` and `develop`.

### Release Process:
1. A release branch is created from `develop` when the report is ready for finalization.
2. Any final changes are made and tested in the release branch.
3. Once stable, it is merged into `main` and tagged with a version number.
4. The release branch is then merged into `develop` to ensure all updates are reflected.

## Best Practices:
- Use descriptive branch names for clarity.
- Keep feature branches short-lived to avoid conflicts.
- Conduct code reviews and testing before merging.
- Maintain a clean commit history for better traceability.

This branching strategy ensures an organized and efficient workflow while maintaining code quality and project stability.

