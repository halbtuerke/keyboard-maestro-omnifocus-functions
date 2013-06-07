# OmniFocus Keyboard Maestro Macro Functions

## Update ##

As of 2013-06-07, the Keyboard Maestro macros have been removed from this repo. I am no longer a OmniFocus user. It would be irresponsible and careless of me to provide macros that I have no intention to support.

If you are interested in maintaining the Keyboard Maestro macros for future use, feel free to contact me.

----

Useful for exporting an OmniFocus tasks to another bucket (nvALT, MindMap) in a format that works best for you.



##  Retrieve Information From a Selected OmniFocus Task

- Get OmniFocus task name
- Get OmniFocus task note
- Get OmniFocus task creation date
- Get OmniFocus task due date
- Get OmniFocus task start date
- Get OmniFocus task context
- Get OmniFocus task URI
- Get OmniFocus task project name
- Get OmniFocus task parent name (Action Group)
- Get URL(s) From OmniFocus task note
- Get OmniFocus task flag status
- Convert OmniFocus task creation date format
- Convert OmniFocus task due date format
- Convert OmniFocus task start date format



## Usage ##

Use Keyboard Maestro action: "Execute A Macro".

Each function stores the returned value in a Keyboard Maestro variable.

- OFTaskName - Name of the selected task
- OFTaskNote - Note of the selected task
- OFTaskDate - Creation Date of the selected task
- OFTaskDueDate - Due date of the selected task
- OFTaskContext - Context of the selected task
- OFTaskURL - The URI of the selected task
- OFTaskNoteURL - The URL(s) in the note of the selected task
- OFTaskFlag - Flag status of the selected Task
- OFTaskParentName - The name of the selected task's parents (Action Group)
- OFTaskProj - The Name of the Project associated with the Selected Task
- OFConvertedDate - Contains the time stamp conversions for creation date, due date and start date


## Best Practice ##

At the end of the calling macro, use the Keyboard Maestro action "Set Variable to Text" and overwrite  the function variable with:

	%Delete%
