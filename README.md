# GitHub Merge Rules

## Branches
1. **Master**: Serves as the production branch.
2. **Dev**: Serves as the active development branch.
3. **Feature/Bugfix Branches**:
   - All features and bugfixes must be developed in separate branches.
   - Direct commits to `dev` are prohibited. Changes must come via pull requests.

## Merging
4. **To Master**:
   - Direct merges are prohibited.
   - Merging is only allowed through pull requests from `dev` or `hotfix` branches.
5. **To Dev**:
   - Direct commits are prohibited.
   - Changes must be merged via pull requests from feature/bugfix branches.

## Production Versions
6. Every merge into `master` generates a new production version.

## Tagging and Releases
7. A new tag and release is generated from `master` every Wednesday.

## Repository Requirements
8. Each repository must include:
   - An `info.json` file carrying version details, which must be merged into the main executable.
   - A changelog documenting all versions.
