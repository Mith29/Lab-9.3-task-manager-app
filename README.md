                             Task Manager App


A simple Task Manager application built using React and TypeScript. This app demonstrates component-based architecture, state management, filtering, and strong typing. 

 # Features:

*Add and manage tasks

*Update task status (Pending, In Progress, Completed)

*Delete tasks

*Filter tasks by:

*Status

*Priority

*Strong TypeScript typing

*Clean component structure





# Set up:
1. Install dependencies:

    npm install

2. Run the development server:

    npm run dev





# Components:


* TaskList:

-Renders a list of tasks

-Receives tasks as props

-Passes handlers to TaskItem




* TaskItem:

Displays individual task details.

Allows:

-Status update

-Task deletion





* TaskFilter:

Filters tasks by:

-Status

-Priority

-Sends selected filters back to parent component





# State Management:

tasks → Stores all tasks

filters → Stores selected filter values

filteredTasks → Dynamically filters tasks based on selected filters





#  Reflection Questions:

1.How did you ensure unique keys for your list items?

I used a unique id for each task as the key when rendering the list. This helps React update items correctly and avoid rendering issues.


2.What considerations did you make when implementing the filtering functionality?

I made sure the filters worked independently and together without breaking the list. I also handled the case when no filter is selected so all tasks show.


3.How did you handle state updates for task status changes?

I updated the task list using state and created a new updated array instead of modifying the old one. This keeps React updates predictable.


4.What challenges did you face when implementing conditional rendering?

At first, managing multiple conditions was confusing, but I simplified it using clear boolean checks. That made the UI logic easier to understand and maintain.



