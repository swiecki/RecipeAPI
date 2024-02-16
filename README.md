# Take Home Assignment - L3 Front End Engineer, AI Solutions

This project is a web application for searching recipes by title, developed as part of the Take Home Assignment for the L3 Front End Engineer position at AI Solutions. The primary objective is to showcase creativity, decision-making skills, and the ability to discuss thought processes during debrief.

## Objective

Develop a web application for searching recipes by title.

## Requirements

### Functionality

- Enable users to search for recipes by entering their titles.
- Display a list of recipes that match the search criteria.
- Include as much detail about the recipe as appropriate.
- Each recipe should include a title, ingredients list, and cooking instructions.
- Allow users to view detailed information by clicking on a recipe title.

### Technology

- Utilize TypeScript and NextJS.
- Restrict total development time to 2-3 hours.

### Design

- Design a clean and user-friendly UI.
- Implement Shadcn/ui components for UI development.

### Data Fetching

- Bonus 1: Use TanStack query for efficient data fetching from a server or API.

### Integration

- Bonus 2: Integrate OpenAI API to provide additional features like ideas for recipe modifications or other suggestions.

### Testing

- Bonus 3: Include tests (unit, integration, and/or end-to-end) for main functionalities.

## Deliverables

- Source code hosted on a public repository (e.g., GitHub).

## Evaluation Criteria

- **Functionality:** Does the app fulfill the specified requirements?
- **Code Quality:** Organization, clarity, and cleanliness of the code.
- **Design:** User-friendliness and visual appeal of the UI.
- **Testing:** Adequate coverage of the main functionalities.
- **Bonus:** Implementation of bonus features.

## Note

- Recipe data can be hardcoded or sourced from an external API.

## Getting Started

If you've never started a Next.js project before, start [here](https://ui.shadcn.com/docs/installation/next).

## Contact

For any questions or clarifications regarding the assignment, feel free to contact Cassidy.

---

## Code Explanation

The provided code consists of a Next.js web application that allows users to search for recipes and view their details. Here's a breakdown of the key components:

### `Home` Component

- Implements the main functionality of the application, including searching for recipes and displaying them.
- Utilizes `QueryClient` from `@tanstack/react-query` for efficient data fetching.
- Handles user interactions such as searching for recipes and filtering by special diets.
- Renders recipe cards for each recipe retrieved from the API.

### `PageLayout` Component

- Defines the layout structure of the application, including the header, search bar, special diets section, and footer.
- Handles user interactions such as searching for recipes and clicking on the home icon.
- Provides a clean and user-friendly UI design using Shadcn/ui components.

### `RecipeCard` Component

- Represents a recipe card displayed in the application.
- Fetches and displays detailed information about a recipe when clicked.
- Utilizes the `fetchRecipeInformation` function to fetch recipe details from the API.

### `api` Module

- Contains functions for fetching recipe data from the Spoonacular API.
- Provides functions for fetching recipes by title, fetching recipe information by ID, and fetching recipes by special diets.

### Explanation of Code Sections

- **Fetching Data:** The application fetches recipe data from the Spoonacular API using asynchronous functions. It handles errors gracefully and displays appropriate error messages.
- **UI Components:** The application uses Shadcn/ui components for building a clean and user-friendly UI. Components such as cards, accordions, and search bars enhance the user experience.
- **State Management:** The application manages state using React's `useState` hook. It maintains state variables for recipes, error messages, and whether to show full recipe details.
- **Event Handling:** Event handlers are used to handle user interactions such as searching for recipes, clicking on special diet filters, and clicking on recipe cards to view details.
- **TanStack Query:** The application leverages TanStack's query functionality for efficient data fetching. It utilizes `QueryClient` from `@tanstack/react-query` to manage and cache API requests, ensuring optimal performance and data consistency.

 ---

Feel free to explore the code further and reach out if you have any questions or need further clarification.

