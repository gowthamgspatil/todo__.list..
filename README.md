This program is a simple command-line-based **Todo List Manager**. 

### **Functions and Their Roles**
1. **`print_menu()`**:
   - Displays the main menu of the application with four options:
     1. View Tasks
     2. Add a Task
     3. Remove a Task
     4. Exit
   - Called whenever the menu needs to be displayed.

---

2. **`get_choice()`**:
   - Prompts the user to enter their choice from the menu.
   - Validates user input to ensure it is one of the allowed choices (`1`, `2`, `3`, or `4`).
   - Returns the valid choice.

---

3. **`display_tasks(tasks)`**:
   - Takes the current task list (`tasks`) as an argument.
   - Displays all tasks with their corresponding indices (starting from 1).
   - If the task list is empty, it prints **"No tasks in the list."**

---

4. **`add_task(tasks)`**:
   - Takes the current task list (`tasks`) as an argument.
   - Prompts the user to input a new task.
   - Ensures the task is not empty (by checking if the input is not blank).
   - Adds the valid task to the `tasks` list.

---

5. **`remove_task(tasks)`**:
   - Takes the current task list (`tasks`) as an argument.
   - Displays the tasks so the user can see which one to remove.
   - Prompts the user to enter the task number to be removed.
   - Validates the input:
     - Ensures the number corresponds to a valid task in the list.
   - Removes the selected task from the list.

---

### **The Main Program (`main`)**
1. **Initialization**:
   - Creates an empty list `tasks` to store the tasks.

2. **Menu Loop**:
   - Displays the menu using `print_menu()`.
   - Gets the user's choice using `get_choice()`.

3. **Perform Actions Based on User Choice**:
   - **Choice 1**: Calls `display_tasks(tasks)` to display the current tasks.
   - **Choice 2**: Calls `add_task(tasks)` to add a new task to the list.
   - **Choice 3**: Calls `remove_task(tasks)` to remove a task by its number.
   - **Choice 4**: Exits the program.

4. **Exit**:
   - If the user selects "4", the program breaks out of the loop and terminates.

