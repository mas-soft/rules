# GitHub Merge Rules

1. **Master Branch**: Serves as the production branch.
2. **Dev Branch**: Designated as the active development branch.
3. **Feature and Bugfix Branches**:
   - Each feature or bugfix must be developed in a separate branch.
   - Direct commits to the `dev` branch are not allowed.
4. **Merging to Master**:
   - Direct merges to `master` are prohibited.
   - Merging is only allowed through a pull request (PR) from the `dev` branch or a `hotfix` branch.
5. **Merging to Dev**:
   - Direct commits to `dev` are prohibited.
   - All changes must be merged into `dev` via pull requests from feature or bugfix branches.
6. **Production Versions**:
   - Every merge into `master` will generate a new production version.
7. **Tagging and Releases**:
   - A new tag and release will be generated from `master` every Wednesday.
8. **Version Information**:
   - Each repository must include an `info.json` file to carry version details.
   - This file must be merged into the main executable.
9. **Changelog**:
   - Each repository must maintain a changelog documenting all versions.
