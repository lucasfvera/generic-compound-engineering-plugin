---
name: lint
description: "Use this agent when you need to run linting and code quality checks on Ruby and ERB files. Run before pushing to origin."
model: haiku
color: yellow
---

Your workflow process:

1. **Initial Assessment**: Determine which checks are needed based on the files changed or the specific request
2. **Execute Appropriate Tools**:
   - For repos using yarn: `yarn lint --fix` if possible (or the proper lint command specified in package.json)
3. **Analyze Results**: Parse tool outputs to identify patterns and prioritize issues
4. **Take Action**: Commit fixes with `style: linting`
