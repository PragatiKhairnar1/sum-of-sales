# Sales Summary Dashboard

This is a simple, single-page web application designed to fetch sales data from a `data.csv` file, calculate the total sales, and display it prominently.

## Features

*   **Data Fetching**: Automatically loads `data.csv` from the same directory.
*   **Sales Calculation**: Parses the CSV and sums values from the 'sales' column.
*   **Dynamic Title**: Updates the page title with the calculated total sales.
*   **Responsive Design**: Built with Tailwind CSS for a clean, mobile-first experience.

## How to Use

1.  Ensure `index.html` and `data.csv` are in the same directory.
2.  Open `index.html` in any modern web browser.
3.  The application will automatically fetch and process `data.csv`, displaying the total sales.

## Data Format

The `data.csv` file is expected to be a comma-separated values file with a header row. It **must** contain a column named `sales` (case-insensitive for the header match). For example:

```csv
id,product,sales,region
1,Laptop,1200,North
2,Mouse,50,North
3,Keyboard,75,South
4,Monitor,300,West
5,Webcam,40,East
```

## Technologies Used

*   **HTML5**: Structure of the web page.
*   **Tailwind CSS**: For responsive and modern styling.
*   **JavaScript (ES6+)**: For data fetching, parsing, and DOM manipulation.

## Error Handling

The application includes basic error handling for scenarios such as:

*   `data.csv` not found or network errors.
*   Empty or malformed CSV file.
*   Missing 'sales' column.
*   Non-numeric values in the 'sales' column.

In case of an error, an appropriate message will be displayed on the page.