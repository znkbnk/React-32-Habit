Step 1: Get Current Date, show Date in toast message.

- Locate the HabitList.js, find the handleCheckClick
function and create a JavaScript Date object to
capture the current date and time.
- Update the toast.success function call within the
handleCheckClick function to include the
currentDate in the toast message.

Step 2: Add checked date to the Habit.

- In HabitList.js include a property to store the
check-in dates. You can add a checkedDates property
to each habit, which will be an array.
- In the handleCheckClick function, after you add
the current date and time to the checkedDates array
of the habit, ensure you save the updated habit data.
- After updating the habit with the check-in date,
save the updated habits array to local storage.

Step 3: Show the dates and times in CompletedHabits.js.

- In the CompletedHabits component, iterate over
the habits that you want to display.
- For each habit in the CompletedHabits component,
iterate over the checkedDates array, if it exists.
- Display the date and time of each check-in within
the component. You can format the date and time
 using the toLocaleString() method.

Step 4: Save and load habits and unfinished habits.

- Use the useState hook to initialize unfinishedHabits
state variable.
- Use the useEffect hook to load data from localStorage
when the component is mounted: Load the habits data
from localStorage. Load the unfinishedHabits data
from localStorage.
- Update handleEditChange, handleEditSave, and
handleCompleteClick functions to update the habits
state and save the updated habits back to localStorage.
- Create a function (e.g., saveCompletedHabitsToStorage)
to save completed habits to localStorage. Call this
function when a habit is completed or achieves its goal.


