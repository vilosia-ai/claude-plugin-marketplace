# User Story breakdown

## User Story file: $ARGUMENTS
Analyse the given user story to break it down into smaller features that can be implemented and deployed in isolation.

## Analyse Process

1. **High Level Breakdown**
   - create one feature file for all Database related tasks, if needed
   - CRITICAL: if there are multiple new endpoints in an API separate them into separate feature files, one per endpoint

2. **Feature Definition**
   - For each feature of the user story create one file in location `.vilosia/features/{feature-name-}.md`
   - link to the original user story file: $ARGUMENTS
   - summary of what the feature does, make sure to include information about the domain the feature is being implemented in
   - database schema (if needed)
     - CRITICAL: When creating Database schemas: use m:n mapping tables only when necessary, try to find schemas that implement 1:n relationships with a simple foreign key to the other table
   - endpoint definition (CRITICAL only include the 4 items, only include if needed)
     - HTTP Method 
     - Route
     - Path Parameters (if needed)
     - Request Parameters (if needed)

*** ULTRATHINK ABOUT THE Feature Definition and if the features together fulfill the user story wish before creating the feature files. If there is not enough information provided by the userstory, ask the user for clarification***

## Quality Checklist
- [ ] All features are created
- [ ] Every featurefile includes a summary, database / DTO structure, description of new endpoints if necessary