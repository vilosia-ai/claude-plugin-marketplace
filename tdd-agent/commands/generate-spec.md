# generate spec

## Feature file: $ARGUMENTS

Generate a complete specification for general feature implementation with thorough research. Ensure context is passed to the AI agent to enable self-validation and iterative refinement. Read the feature file first to understand what needs to be created, how the examples provided help, and any other considerations. The AI agent only gets the context you are appending to the spec and training data.

## Research Process

1. **Codebase Analysis**
   - Search for similar features/patterns in the codebase
   - Identify files to reference in the specification
   - Note existing conventions to follow
   - Check test patterns for validation approach

2. **User Clarification** (if needed)
   - Specific patterns to mirror and where to find them?
   - Integration requirements and where to find them?

## SPEC Generation

Using .vilosia/templates/spec-template.md as template:

### Critical Context to Include and pass to the AI agent as part of the Specifiation
- **Documentation**: URLs with specific sections
- **Code Examples**: Real snippets from codebase
- **Patterns**: Existing approaches to follow

### Implementation Blueprint
- Start with pseudocode showing approach
- Reference real files for patterns
- Include error handling strategy
- list tasks to be completed to fullfill the specification in the order they should be completed

*** CRITICAL AFTER YOU ARE DONE EXPLORING THE CODEBASE BEFORE YOU START WRITING THE SPECIFICATION ***
*** ULTRATHINK ABOUT THE SPECIFICATION AND PLAN YOUR APPROACH THEN START WRITING THE SPECIFICATION ***

## Output
Save as: `.vilosia/features/{feature-name-spec}.md`

## Quality Checklist
- [ ] All necessary context included
- [ ] References existing patterns
- [ ] Clear implementation path
- [ ] Error handling documented

Remember: The goal is one-pass an iterative testdriven design implementation through comprehensive context.