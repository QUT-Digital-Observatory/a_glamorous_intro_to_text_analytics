# Contributing to the workshop materials

Find a problem? Is there confusing wording that needs clarifying, or a bug in the code? [Submit an issue on GitHub](https://github.com/QUT-Digital-Observatory/a_glamorous_intro_to_text_analytics/issues)!

Thank you for letting us know about the problems you've found 😊

## Development 

### Local setup

Follow the same local setup instructions as in the [readme](readme.md). The following instructions use the shell, and also assume some familiarity with git.

Install additional development requirements with:

```shell
pip install -r python_requirements_dev.txt
pre-commit install
```

### Pre-commit

The recommended development setup uses [pre-commit](https://pre-commit.com/) and [nbstripout](https://github.com/kynan/nbstripout) to automatically clean up Jupyter notebooks before committing them to git.

This means that the current environment and cell outputs in your notebooks will be deleted whenever you run `git commit` - which you need to be aware of so that you don't lose current working, but has the enormous benefit of ensuring no sensitive data is ever committed to git within your notebook cell outputs.

Notebook files which are not added to the current commit will be unaltered.

If when you run `git commit` the output says that nbstripout failed, it means that nbstripout cleaned up at least one notebook file.

Example output:

```shell
❯ git commit -m "Set up files for data collection section"
nbstripout...............................................................Failed
- hook id: nbstripout
- files were modified by this hook
```

Note the final line stating that files were modified. Your git commit failed, but the files you added are all still in the staging area - run `git status` to see the list of which files are still staged and which were modified by nbstripout. Use `git add ...` to add each modified notebook file back in to the staging area, and then once `git status` shows that all your changes are staged again, you can re-run the commit and it should succeed (as long as you have not run any notebook cells since the first commit attempt).

**Notebook cleaning tip**: You can also [use nbstripout on its own as a command line tool](https://github.com/kynan/nbstripout?tab=readme-ov-file#usage) to clean up a notebook file separately from a git commit.

