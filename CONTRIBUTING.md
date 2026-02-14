# Contributing to PyVLX

Thank you for your interest in contributing to PyVLX!

## Pull Request Process

### For Contributors (Fork Owners)

When you create a pull request from your fork to the main repository, please ensure:

1. **Allow Maintainer Edits**: Enable the "Allow edits from maintainers" option when creating your pull request. This allows the repository maintainers to make minor adjustments if needed.

2. **Keep PRs Focused**: Each pull request should address a single issue or feature.

3. **Follow Code Style**: Ensure your code follows the existing code style in the repository.

4. **Test Your Changes**: Make sure your changes don't break existing functionality.

### For Maintainers

Pull requests from forks with "Allow edits from maintainers" enabled (shown as `maintainer_can_modify: true` in the GitHub API) can be:

- Merged directly by maintainers
- Modified by maintainers before merging
- Updated with additional commits by maintainers

## Current Open Pull Requests

The following pull requests from the MaGeHome fork are ready for review and can be merged directly by maintainers:

- **PR #539**: Update node_updater.py - Adds state tracking from FrameNodeStatePositionChangedNotification
- **PR #540**: Update nodes.py - Adds state attribute to Nodes class

Both PRs have:
- ✅ `maintainer_can_modify: true` enabled
- ✅ Mergeable state (no conflicts)
- ✅ Clean merge status

## How to Merge PRs from Forks

As a maintainer of the Julius2342/pyvlx repository, you can merge pull requests from forks in several ways:

### Option 1: Direct Merge via GitHub UI
1. Go to the pull request page
2. Review the changes
3. Click "Merge pull request" button
4. Choose merge type (merge commit, squash, or rebase)
5. Confirm the merge

### Option 2: Command Line Merge
```bash
# Fetch the PR branch
git fetch origin pull/539/head:pr-539
git fetch origin pull/540/head:pr-540

# Review and merge
git checkout master
git merge pr-539
git merge pr-540
git push origin master
```

### Option 3: Merge Both PRs Together
If the PRs are related and should be merged together:
```bash
# Create a new branch
git checkout master
git checkout -b merge-prs-539-540

# Fetch and merge both PRs
git fetch origin pull/539/head:pr-539
git fetch origin pull/540/head:pr-540
git merge pr-539
git merge pr-540

# Push and create a new PR or merge directly
git push origin merge-prs-539-540
```

## Questions?

If you have any questions about the contribution process or specific pull requests, please open an issue or comment on the relevant pull request.

---

**Note**: This document was created to clarify the merge process for pull requests from forks. The existing PRs #539 and #540 are properly configured and ready to be merged by the repository maintainer (Julius2342) at their discretion.
