name: mannual tests
on:
  workflow_dispatch:

jobs:
  latest:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/setup-python@main
        with:
          check-latest: true
      # Warning: The `python-version` input is not set.  The version of Python currently in `PATH` will be used.
      - run: python --version
