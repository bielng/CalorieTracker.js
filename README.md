# Calorie Tracker

A simple yet powerful **Calorie Tracker** application built with JavaScript to help users track their daily calorie consumption and manage their diet effectively.

## Features

- **Add Meals**: Log meals with their respective calorie counts.
- **View Total Calories**: Automatically calculates the total calories consumed for the day.
- **Delete Entries**: Remove meals from the tracker as needed.
- **Responsive Design**: Fully functional on both desktop and mobile devices.

## Technologies Used

- **HTML5**: Markup for the structure of the application.
- **CSS3**: Styling to create a user-friendly and visually appealing interface.
- **JavaScript (ES6)**: Core logic for managing meals and calories.

## Getting Started

Follow these steps to run the application locally:

### Prerequisites

- A modern web browser (e.g., Google Chrome, Mozilla Firefox).
- Basic knowledge of JavaScript and web development.

### Installation

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/bielng/calorie-tracker.git
   ```
2. Navigate to the project directory:
   ```bash
   cd calorie-tracker
   ```
3. Open the `index.html` file in your browser to view the application.

## Usage

1. Enter the name of a meal and its calorie count.
2. Click the **Add Meal** button to log the meal.
3. View your daily calorie total at the top of the app.
4. To delete a meal, click the delete button next to the respective entry.

## Code Structure

- **`index.html`**: The main HTML file containing the application's structure.
- **`style.css`**: Contains the styling for the application.
- **`app.js`**: The main JavaScript file handling functionality like adding meals, calculating totals, and removing entries.

## Troubleshooting

### Common Error:

- **`Uncaught TypeError: Cannot read properties of null (reading 'calories')`**:
  - Ensure that all entries added to the tracker include a valid `calories` property.
  - Sanitize the input to prevent invalid or `null` values.

### Solution:

- Filter entries before performing calculations:
  ```javascript
  const validEntries = this.entries.filter(
    (entry) => entry && entry.calories !== undefined
  );
  ```

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch for your feature:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- Special thanks to all open-source contributors whose tools and libraries helped make this project possible.
