## Status
Accepted

## Context
ApplyFlow needs a structure for organising job applications in a way that reflects how applicants track their progress. The approach is to organise applications visually using Boards containing Stages, with individual job applications represented as Cards.

## Decision
ApplyFlow will use a Board → Stage → Card model where a board represents a job-search campaign or category, a stage represents a step in the application workflow. The initial default stages are Saved, Applied and Closed and a card represents an individual job application.

Applications will be able to move between stages as their status changes.

## Consequences
### Positive
- The model gives users a visual representation of their application pipeline.
- Moving a Card between Stages naturally represents application progress.
- The structure supports filtering and board management functionality.

### Negative
- The implementation will need to maintain relationships between Boards, Stages and Cards.

## Result
Future ApplyFlow implementation should preserve this model unless a later ADR records and explains a decision to replace it.