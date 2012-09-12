# OmniFocus Keyboard Maestro Macro Functions

##  Retrieve Information From a Selected OmniFocus Task

- Get OmniFocus task name
- Get OmniFocus task note
- Get OmniFocus task creation date
- Get OmniFocus task due date
- Get OmniFocus task context
- Get OmniFocus Task URL

## Usage ##

Use Keyboard Maestro action: "Execute A Macro".  
  
Each function stores the returned value in a Keyboard Maestro variable.

- OFTaskName
- OFTaskNote
- OFTaskDate
- OFTaskDueDate
- OFTaskContext
- OFTaskURL

## Best Practice ##

At the end of the calling macro, use the Keyboard Maestro action "Set Variable to Text" and overwrite  the function variable with:

	%Delete%
