# Interactive Card Grid Page

## Description
This project is a single-page HTML application that displays a responsive grid of informational cards. It features client-side search/filtering and pagination capabilities, allowing users to easily browse and find relevant content cards. The styling is handled using Tailwind CSS loaded via CDN.

## Features
1. Responsive Card Grid: Displays cards in a grid that adapts to different screen sizes (from 1 column on small screens up to 5 on extra-large screens).
1. Clickable Cards: Each card acts as a link, opening the associated URL in a new browser tab.
1. Client-Side Search: An input field allows users to filter cards in real-time based on title, description, author, or skill tag.
1. Pagination: Automatically divides the cards into pages if the total number exceeds the configured limit (ITEMS_PER_PAGE). Navigation buttons allow users to move between pages.
1. Dynamic Rendering: Cards and pagination controls are rendered dynamically using JavaScript based on the current data set (all data or filtered data) and the current page.
1. Tailwind CSS Styling: Utilizes the Tailwind CSS utility-first framework for styling, loaded via CDN.

## How to Use
1. Save the code from the card_grid_page artifact as an HTML file (e.g., index.html).
2. Open the index.html file directly in any modern web browser.

No build steps or server setup are required as it's a self-contained HTML file with embedded CSS (via Tailwind CDN) and JavaScript.

## Dependencies
- Tailwind CSS: Loaded via CDN (https://cdn.tailwindcss.com). An internet connection is required for the styles to apply correctly.

## Data Structure
The card data is currently hardcoded within the <script> tag in the HTML file as a JavaScript array of objects. Each card object follows this structure:

|Field| Description|
|----|----|
|id           | Unique identifier (currently unused but good practice)|
|title        | Main title of the card|
|publishedDate| Date string (e.g., "March 1, 2025")|
|description  | Descriptive text content|
|linkUrl      | URL the card links to|
|author       | Name of the author/creator|
|skill        | Skill category/tag (e.g., "Python", "CSS")|


```json
{
  "id": "Number",
  "title": "String",
  "publishedDate": "String",
  "description": "String",
  "linkUrl": "String",
  "author": "String",
  "skill": "String"
}
```

## Future Enhancements
1. Fetch Data from API: Load card data dynamically from an external API instead of hardcoding it.
1. Advanced Filtering/Sorting: Add options to sort cards (e.g., by date, title) or filter by specific skills/authors using dropdowns or checkboxes.
1. Line Clamp Plugin: Officially include the @tailwindcss/line-clamp plugin (requires a build step or alternative CDN) for more robust description truncation.
1. State Management: For more complex versions, consider a simple state management approach.
1. Accessibility Improvements: Further review and enhance accessibility features (e.g., more descriptive aria-labels, keyboard navigation testing).
1. Loading State: Add a visual indicator while data might be loading (more relevant if fetching from an API).
1. Error Handling: Implement more robust error handling, especially if fetching data externally.