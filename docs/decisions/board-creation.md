## Description
The `createJobSearchBoard()` function will validate the board name, create the board and initialise it with the default stages Saved, Applied and Closed.

## Input
### boardName
A text value containing the name of the new job-search board.
The board name must not be empty or contain only spaces.

## Output
If the board name is valid, the function returns or creates a new board containing:
 - The board name.
 - Saved as the first default stage.
 - Applied as the second default stage.
 - Closed as the third default stage.

## Error Cases
### Empty board name
If no board name is entered, the function must not create a board and should return a validation error.

### Whitespace-only board name
A value containing only spaces will be treated as invalid.

### Board creation failure
If the board cannot be created, the function should return an error.