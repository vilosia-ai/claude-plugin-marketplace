---
description:Executes the given spec file.
---
# Execute SPECIFICATION

## SPEC File: $ARGUMENTS

## Execution Process

1. **Load Specification**
   - Read the Specification file
   - Understand all context and requirements
   - Follow all instructions in the Specification
   - Ensure you have all needed context to implement the Specification fully
   - Do more web searches and codebase exploration as needed

2. **ULTRATHINK**
   - Think hard before you execute the plan. Create a comprehensive plan addressing all requirements.
   - Break down complex tasks into smaller, manageable steps using your todos tools.
   - Use the TodoWrite tool to create and track your implementation plan.
   - Identify implementation patterns from existing code to follow.

3. **Execute the plan**
   - Execute the Specification
   - Follow the test driven design approach: red, green, refactor
   - Find and implement all tests you can find here: Save as: `.vilosia/features/{feature-name-tests}.md`
   - Implement the test first, run the test, see it fail, implement the according code to fullfill the test, refactor, test again

4. **Validate**
   - Fix any failures
   - Re-run until all pass
   - CRITICAL: You need to run go tests via script eg. [script -qec "go test -v ./internal/api/pullrequests" /dev/null] otherwise the output is ommited and you don't get an exit code.

5. **Complete**
   - Ensure all checklist items done
   - Run final validation suite
   - Report completion status
   - Read the Specification again to ensure you have implemented everything

6. **Reference the Specification**
   - You can always reference the Specification again if needed