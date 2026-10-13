# CodeLens demo repository

This repository exists to show [CodeLens](https://github.com/RAIF-KARANI/codelens), a
code reviewer that reads a pull request together with the code around it (its callers,
callees and related functions) and cites that code as evidence for every finding. It
runs entirely on local models (`qwen3:8b` through Ollama, on a laptop GPU).

**The open pull requests are the demo.** Each one was reviewed by the CodeLens GitHub
App, which posted its review on the PR. Some carry bugs planted on purpose, taken from
CodeLens's evaluation set; one is a harmless change, to show it doesn't invent problems.
**None of them is meant to be merged.**

The same reviews, with the diff, every finding's evidence, the call graph around the
change and the retrieval trace, are on the public demo dashboard linked from the CodeLens
README.

## Where the code comes from

The code is [sqlite-utils](https://github.com/simonw/sqlite-utils) by Simon Willison, at
commit `9c66bafa52ae23d40499c74b0db3b635bcddb876`, unchanged on `main`. It is licensed
under the Apache License 2.0 (see `LICENSE`); its own README is kept as
`README.sqlite-utils.md`. Please use the original project, not this copy.
