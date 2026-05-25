1. How to run the project

To run this project locally:

Steps:
Download or clone the repository
Open the project folder
Open index.html directly in any modern browser (Chrome, Edge, Firefox)
OR (recommended for development):
Open the project in VS Code
Install Live Server extension
Right-click index.html
Click "Open with Live Server"

No installation, build step, or dependencies are required since this is a pure HTML/CSS/JavaScript project.

2. Stack & design choices
Why this stack?

I chose Vanilla HTML, CSS, and JavaScript because the goal of this task was to demonstrate core frontend fundamentals without relying on frameworks. This allowed me to focus on DOM manipulation, state handling, and UI updates manually.

Design decisions:

1. Simple list-based layout for habits

Each habit is rendered as a row in a vertical list.
I chose this over a grid because it keeps the UI readable even when the number of habits increases.
This design improves scanning speed and avoids clutter.

2. Toggle-based completion system

Each habit uses a simple toggle button instead of complex checkboxes or calendars.
This keeps interaction lightweight and reduces cognitive load for the user.

Where it applies:

Habit list section (main UI area)
Habit interaction controls (mark complete/reset logic)
3. Responsive & accessibility
Responsive behavior:
On 1440px desktop, the layout stays centered with enough spacing for readability.
On 360px mobile screens, elements stack vertically and buttons expand to full width for easier tapping.
Flexbox is used to ensure natural wrapping without breaking layout.
Accessibility considerations:
Buttons are clearly labeled (Add, Complete, Reset)
High contrast between text and background improves readability
Native HTML buttons are used for better keyboard accessibility
One accessibility limitation:

I did not fully implement ARIA roles or screen-reader-specific labels because the focus of this submission was core functionality and DOM handling. This would be a next-step improvement in a production version.

4. AI usage

I used AI (ChatGPT) in the following parts:

Helping structure the initial project layout (HTML/CSS/JS separation)
Debugging JavaScript logic for adding and toggling habits
Generating initial UI styling ideas for a clean minimal interface
Example of modification:

The AI initially suggested storing each habit as an object with multiple properties and rendering a complex component structure.
I simplified this by:

Using a basic array of strings / simple objects
Direct DOM manipulation instead of re-rendering full component trees

This was done to keep the project lightweight and easier to understand without frameworks.

5. Honest gap

One area that is not fully polished is data persistence and state management.

Current limitation:
Habits and progress reset when the page is refreshed
There is no localStorage or backend integration
How I would improve it:

If I had one more day, I would:

Add localStorage support to persist habits and completion state
Refactor state into a structured object (habit + status + timestamp)
Improve UI feedback when toggling completion (animations or visual transitions)
