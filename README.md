# Mast5020-Final-POE
Changelog

v1.0.0

Project Initialization: Set up a new Expo project using TypeScript.
File Organization: Structured the project with distinct folders for components, utilities, types, and navigation.
Home Screen: Implemented a screen to display menu items, with functionality to calculate the average price by course.
Menu Management Screen: Added a screen for adding and removing menu items.
Filter Screen: Created a screen for filtering menu items by course type.
Utility Functions: Developed calculateAverage.ts to handle average price calculations.
Type Definitions: Added type safety by defining MenuItem and Averages types in index.ts.
v1.1.0

UI/UX Enhancements: Improved layout for a more user-friendly experience, including button labels and clearer 
navigation.
Data Validation: Added checks to ensure fields are properly filled and input formats are correct.
Code Refactoring: Streamlined repeated code into reusable functions and reorganized files by feature for better readability and performance.


After reviewing the feedback from my lecture, I made several key changes to enhance the app’s code structure, maintainability, and overall user experience. First, I addressed the issue with the duplicate export default App line by consolidating it into a single, clean component definition, which eliminates any ambiguity and potential errors. I also streamlined the font-loading process by removing the redundant return statement after AppLoading, which simplifies the code and ensures a smoother, faster execution during startup.

Since the MenuForm component was initially undefined, I created it as a controlled input form that gathers essential fields like dishName, course, description, and price. These inputs are then passed to the addMenuItem function on submission, making the app more modular and keeping the main App component focused on handling high-level functionality. To ensure code maintainability, I refactored the logic by moving reusable form elements and handlers into custom hooks, which reduces code duplication and makes each component's purpose clearer.

Given the navigation setup, I separated the menu display and form functionalities into distinct screens, placing them within the Navigator structure. This setup not only enhances the app's organization but also improves its user flow, making it intuitive to switch between viewing and adding menu items. I configured homeStack to include the new screens and added transition animations for smoother navigation. Additionally, I implemented a “Back to Home” button and customized the header titles, improving navigation clarity for users.

In terms of styling, I refined the visual presentation by making the menuItem background more distinct and adding padding and margin adjustments to enhance the spacing between items. The app now uses custom fonts for headers, menu items, and details, achieving a cohesive, polished look. I also introduced color themes to match the app’s brand, applied consistent styling for buttons, and added hover and active states to give users visual feedback during interactions.

Finally, I focused on user experience by implementing real-time validation for the MenuForm input fields, guiding users as they fill in the form. For example, fields such as price now check for valid numeric input, and required fields provide feedback if left empty. I also added an error summary that displays a user-friendly message when inputs are invalid, enhancing the app's professionalism and usability. These updates collectively make the app more responsive, visually appealing, and user-friendly.

