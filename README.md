# toDoAPP
Let’s break down your code and analyze each function:

handler(event):
This function handles input changes from the user.
It extracts the name and value from the event target.
If the name is 'taskname', it updates the taskname property.
If the name is 'taskdate', it updates the taskdate property.
addtaskhandler():
This function adds a task to the incompletetask array.
If taskdate is not set, it defaults to the current date.
It validates the task using the validateTask() function.
If the task is valid, it adds the task to incompletetask, resets the input fields, sorts the array, and updates incompletetask.
validateTask():
Validates whether the task is valid (non-empty and not a duplicate).
Checks if the task name and date combination already exists in incompletetask.
Sets custom validity and reports validity for the input element.
sortTask(inputarr):
Sorts the input array of tasks based on their taskdate.
Uses Date objects to compare dates.
resethandler():
Resets the taskname and taskdate properties.
removeHandler(event):
Removes a task from incompletetask based on the index from the event target.
Sorts the array after removal.
completeHandler(event):
Moves a task from incompletetask to completetask based on the index from the event target.
Sorts the array after removal.
Overall, your code manages tasks, validates input, and maintains separate arrays for incomplete and completed tasks.
