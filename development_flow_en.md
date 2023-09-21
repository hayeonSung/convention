## Development Flow

1. Branch
    - We prefer `<category>/<name>` branch.  
      e.g., `feat/merge-automation`, `fix/configs-bug`  
      (Refer to [the link](https://github.com/pvdlg/conventional-changelog-metahub#commit-types) for the category candidates)
2. Fix files
    - Try to follow the standard code format
3. Commit
    - Follow [the link](https://chris.beams.io/posts/git-commit/) for the good commit messages
4. Pull Request
    - Update the commit (via force push) until the CI pipelines succeed
6. Merge
    - use squash-merge for the merge reqeust
