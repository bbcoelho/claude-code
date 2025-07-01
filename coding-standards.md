## Code Quality Requirements

**CRITICAL**: Before completing any code changes, you MUST verify the code compiles without syntax errors by running `npx tsc`. Never mark a task as completed without testing for compilation errors first.

**REFACTORING PRINCIPLE**: As always as possible, refactor the code using the best refactoring practices to reuse code instead of rewriting code. Extract common logic into reusable methods to avoid duplication.

**COMMIT GROUPING**: Always analyze file changes and group them logically for commits:
- **Related changes together**: Files that depend on each other or implement the same feature should be committed together
- **Unrelated changes separately**: Independent changes (documentation, different features, configuration) should be in separate commits
- **Examples of related changes**: Class + its caller, interface + implementation, new constant + code using it
- **Examples of unrelated changes**: Documentation updates, different features, configuration changes
- Do not include attribution to Claude in the commit message or co-author attribution
- **Important**: Do NOT push to remote repository.

**METHOD PLACEMENT**: When creating new methods, always write them below where they are called, never above. This maintains a logical top-down code flow.