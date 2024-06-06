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

