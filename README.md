# Firebase Counter Project

This project is a simple web-based counter that integrates with Firebase Realtime Database. It consists of two main HTML files:

1. **index.html**: A basic counter that allows users to increment and decrement a value stored in Firebase.
2. **widget_sabah.html**: A widget that visualizes the counter value and includes a dynamic dark theme toggle based on Firebase settings.

## Features
- **Firebase Integration**: Uses Firebase Realtime Database to store and retrieve counter values.
- **Increment & Decrement**: Users can update the counter in real-time.
- **Dark Theme Support**: `widget_sabah.html` dynamically switches between light and dark themes based on a Firebase-stored value.

## Technologies Used
- HTML, CSS, JavaScript
- Firebase Realtime Database
- Firebase JavaScript SDK

## Setup & Installation

1. Clone this repository:
   ```sh
   git clone https://github.com/SERENGOKYILDIZ/Firebase-Counter.git
   cd Firebase-Counter
   ```

2. Replace Firebase configuration in both `index.html` and `widget_sabah.html`:
   ```js
   const firebaseConfig = {
       apiKey: "YOUR_API_KEY",
       authDomain: "YOUR_AUTH_DOMAIN",
       projectId: "YOUR_PROJECT_ID",
       storageBucket: "YOUR_STORAGE_BUCKET",
       messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
       appId: "YOUR_APP_ID",
       measurementId: "YOUR_MEASUREMENT_ID"
   };
   ```

3. Start a local server (optional for testing):
   ```sh
   python -m http.server 8000  # Python 3 built-in server
   ```
   Then open `http://localhost:8000/index.html` in your browser.

## File Structure
```
Firebase-Counter/
│-- index.html           # Main counter page
│-- widget_sabah.html    # Counter with dark theme support
│-- README.md            # Project documentation
```

## Usage
- Open `index.html` to view the basic counter.
- Open `widget_sabah.html` to see the counter with theme-switching.
- Click the **+** or **-** buttons to modify the value in Firebase.

## Notes
- Make sure your Firebase Realtime Database rules allow read and write access.
- The theme in `widget_sabah.html` is controlled by a `DarkTheme` key in Firebase.

## License
This project is licensed under the MIT License.

---
**Author:** SERENGOKYILDIZ
