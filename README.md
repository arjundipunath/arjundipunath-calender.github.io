-----

## 📅 Simple Web Calendar

This is a basic, single-view web application designed to display the current date and time information (day, date, month, and year). It is built using fundamental web technologies and serves as a great starter project for learning client-side date manipulation with JavaScript.

### ✨ Features

  * **Real-Time Display:** Shows the current date, day, month, and year from the user's system clock.
  * **Date Formatting:** Pre-pends a zero to the date if it is a single digit (e.g., "05").
  * **Modern Design:** Features a two-panel design with a distinct color contrast, utilizing the **Poppins** font family for a clean look.
  * **Responsive Structure:** Uses Flexbox to align and center the calendar component on the page.

-----

### 🛠️ Technology Stack

| Technology | Purpose |
| :--- | :--- |
| **HTML5** | Defines the calendar structure with separate containers for the date/day (`.left`) and month/year (`.right`). |
| **CSS3** | Styles the layout, applies the dark background, sets the contrasting color scheme for the calendar panels, and manages font styles (Poppins). |
| **Vanilla JavaScript** | Handles date retrieval using `new Date()` and dynamically updates the HTML elements (`#date`, `#day`, `#month`, `#year`) upon loading. |

-----

### 🚀 Getting Started

To run this calendar application locally, you only need a web browser.

#### Prerequisites

  * A modern web browser (Chrome, Firefox, Edge, Safari, etc.)

#### Installation and Execution

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/arjundipunath/calender.git # Assuming the repo name is 'calender'
    ```
2.  **Navigate to the Project Directory:**
    ```bash
    cd calender
    ```
3.  **Open the File:**
    Double-click the **`index.html`** file, or right-click it and select "Open with" your preferred web browser.

The current date and time information will immediately load on the screen.

-----

### 💻 Code Logic Highlights (JavaScript)

The core logic for displaying the time resides in a simple script block within `index.html`:

1.  **Date Retrieval:**

    ```javascript
    const today = new Date();
    ```

    This line creates a `Date` object containing the current date and time.

2.  **Data Arrays:**
    `weekDays` and `allMonths` arrays are defined to map the numeric values returned by `today.getDay()` and `today.getMonth()` to their corresponding string names.

3.  **DOM Updates:**

    ```javascript
    date.innerHTML = (today.getDate()<10?"0":"")+today.getDate();
    day.innerHTML = weekDays[today.getDay()];
    // ... and so on for month and year
    ```

    The script accesses the elements by ID and populates them with the current data. The ternary operator `(today.getDate()<10?"0":"")` handles the leading zero requirement for the date.

-----

### ✍️ Author

  * **Arjun Dipunath**

-----
