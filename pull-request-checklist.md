# Frontend Pull Request reviewer checklist

- It follows the MediaMonks [frontend coding standards](https://github.com/mediamonks/frontend-coding-standards) (proper naming for variables, functions, properties, booleans, etc.)
- Does the title follow the correct structure?
- Does the PR correctly solve the issue or implement the feature?
- Is there a clear description of what this PR adds/changes/fixes?
- Has a linked issue
- Pipeline doesn't fail
- Are the files in the right directory?
- Is there any commented code that should be removed?
- Are all comments resolved by either a check or a closing statement?
- If a util or global molecule or atom has been changed does it affect other areas?
- If there are additions to package.json dependencies, check if they are really necessary and how they affect the bundle size.
- Check for unintended code duplication (have utilities or components been added of which similar versions already exist in the codebase?)
- If the code in the PR is only part of a feature instead of a complete feature: is the part useful by itself?
- Are you using any? There are a couple of valid use cases, but in a lot of cases unknown is better.
- Would it break if data is unavailable?
- For abstractions: abstractions are often a trade-off between maintainability (DRY) and readability (DAMP). Is this abstraction worth the trade-off?
- Is code understandable enough when reviewed, or does it need some code comments to explain the intent or behaviour.
- Is code in the PR already present in a similar or relatable way somewhere else in the codebase, and can it be merged/copied/refactored?
- Can the code in the PR be written more generically to be more usable at a later time?
- Is code in the PR already available as an NPM module (already tested, well used, documented)?
- Are all TODO comments ticketed up, with a ticket link appended to the TODO comment?
- Does the feature need any documentation outside of the code/PR (e.g. confluence)?