# Spendwise Project

## Project Overview

Spendwise is a comprehensive financial management tool designed to help users track and manage their expenses, set financial goals, and receive predictive insights. This project leverages Java, Spring Boot, Maven, Hibernate, and React to deliver a full-stack application.

### Key Features
- User login and authentication
- Expense tracking dashboard
- AI-powered financial insights
- Integration with banking statements
- User account management

## Branching Workflow

This document outlines the branching strategy used for the Spendwise project to ensure a well-organized and manageable workflow.

### Branch Hierarchy

1. **Epic Branch**: This is the top-level branch for an Epic. All related stories and tasks will be branched off from here.
2. **Story Branch**: This is a branch for each story under the Epic. It is branched off from the Epic branch. All subtasks for this story will be branched off from the story branch.
3. **Subtask Branches**: These are branches for individual subtasks. They are branched off from the story branch. Once a subtask is complete, it is merged back into the story branch.

### Workflow Example

#### 1. Create Epic Branch

```git checkout -b epic/SPEN-3```

#### 2. Create Story Branch from Epic Branch

```git checkout -b story/SPEN-4-backend epic/SPEN-3```

#### 3. Create Subtask Branch from Story Branch

```git checkout -b subtask/SPEN-6-create-readme story/SPEN-4-backend```


## Working on the Subtask Branch

#### 1. Making changes with Commits

```git add .```

```git commit -m "SPEN-6: Create comprehensive README for backend" ```

#### 2. Push Subtask Branch to Remote:

```git push origin subtask/SPEN-6-create-readme```

#### 3. Create pull/merge Request

Create a pull/merge request to merge subtask/SPEN-6-create-readme into story/SPEN-4-backend

#### 4. Review and Merge Subtask PR:

```Once the PR/MR is reviewed and approved, merge it.```


#### Repeat for Other Subtasks

    Repeat steps 2 to 4 for additional subtask branches, merging each back into the story/SPEN-4-backend branch.


#### Final Merges

    Merge Story Branch into Epic Branch:
        After all subtasks for SPEN-4 are complete and merged into story/SPEN-4-backend, merge story/SPEN-4-backend into epic/SPEN-3.

#### Summary of Branches

    Epic Branch: epic/SPEN-3
    Story Branch: story/SPEN-4-backend
    Subtask Branches: subtask/SPEN-6-create-readme, subtask/SPEN-7-another-task, etc.

### Benefits

    Clear Structure: Hierarchical branching provides a clear structure.
    Isolated Changes: Changes are isolated in subtask branches, making it easier to manage and review.
    Incremental Integration: Subtasks are integrated into the story branch incrementally, reducing merge conflicts.
    Traceability: Easier to trace changes back to specific Jira issues.