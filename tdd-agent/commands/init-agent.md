---
description:Initializes the vilosia agent plugin.
---

# Create file and directory structure
Create the following directory and file structure.

.vilosia
├── features
├── stories
├── templates
    ├── spec-template.md


File Contents
[spec-template.md]

Name: "Spec Template v. 1.0"

## Purpose
Template optimized for AI agents to implement features with sufficient context and self-validation capabilities to achieve working code through iterative refinement with the test driven design approach.

## Core Principles
1. **Context is IMPORTANT**: Include ALL necessary documentation, examples and test cases
2. **Validation Loops**: Provide executable tests the AI can run and fix
3. **Information Dense**: Use keywords and patterns from the codebase
4. **Progressive Success**: Start simple, validate, then enhance
5. **Global rules**: Be sure to follow all rules in CLAUDE.md

---

## Overview
Goal: What needs to be built - be specific about how a successfull Implememtation looks like from a user perspective

### Success Criteria
- [ ] [Specific measurable outcomes]

## All Needed Context

### Documentation & References (list all context needed to implement the feature)
```yaml
# MUST READ - Include these in your context window
- url: [Official API docs URL]
  why: [Specific sections/methods you'll need]
  
- file: [path/to/example.go]
  why: [Pattern to follow, gotchas to avoid]

```

### Current Codebase tree (run `tree` in the root of the project) to get an overview of the codebase

### Desired Codebase tree with files to be added and responsibility of file

## Implementation Blueprint

### Data models and structure

Create the core data models, we ensure type safety and consistency.
```golang
Examples: 
 - orm models
 - DTOs

```

### list of tasks to be completed to fullfill the Spec in the order they should be completed

```yaml
Task 1:
MODIFY internal/api/existing_file.go:
  - FIND pattern: "func OldImplementation"
  - PRESERVE existing method signatures

CREATE internal/api/existing_file.go:
  - MIRROR pattern from: internal/api/similar_feature.go
  - MODIFY function name and core logic
  - KEEP error handling pattern identical

...(...)

Task N:
...

```

### Integration Points
```yaml
DATABASE:
  - migration: "Add column 'feature_enabled' to users table"
  - index: "CREATE INDEX idx_feature_lookup ON users(feature_id)"
  
CONFIG:
  - add to: Makefile
  - pattern: "LOG_GRAYLOG_ENABLED="false" \"
```

### Tests
- create Unit test for the controller and the service

## Validation Loop
run the tests
```

## Final validation Checklist
- [ ] Error cases handled gracefully
- [ ] Logs are informative but not verbose
---

## Anti-Patterns to Avoid
- ❌ Don't create new patterns when existing ones work
- ❌ Don't ignore failing tests - fix them
- ❌ Don't hardcode values that should be config