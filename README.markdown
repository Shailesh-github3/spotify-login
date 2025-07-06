# Spotify Login Page

A simple, responsive login page mimicking Spotify's login interface, built with HTML, CSS, and minimal JavaScript for a password toggle feature.

## Screenshot
![Login Page](screenshots/login.png)

## Features
- **Responsive Design**: Centered login container (300px × 500px) with a dark theme.
- **Social Login Buttons**: Google and Apple buttons with centered text and left-aligned icons, redirecting to respective authentication pages.
- **Form Validation**: HTML5 `required` validation for username and password fields with custom CSS error messages (red border and text) when fields are empty and focused.
- **Password Toggle**: Show/hide password functionality using a Font Awesome eye icon (requires JavaScript).
- **Centered Spotify Logo**: Spotify logo displayed prominently at the top.
- **Clean Styling**: Uses Font Awesome icons, a dark background, and Spotify's green (`#1DB954`) for the submit button.

## Setup
1. **Clone or Download**:
   - Clone the repository or download the project files.
2. **Project Structure**:
   ```
   /project-folder
   ├── index.html
   ├── css/
   │   └── loginstyle.css
   ├── screenshots/
   │   └── login.png
   ├── README.md
   ```
3. **Dependencies**:
   - Include Font Awesome via CDN (already in `index.html`):
     ```html
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css">
     ```
   - No other external dependencies required.
4. **Local Server** (optional):
   - Serve using a local server (e.g., VS Code Live Server, `python -m http.server`) to test redirects and ensure proper rendering.
   - Alternatively, open `index.html` directly in a browser (redirects may not work).

## Usage
1. Open `index.html` in a browser.
2. Interact with the form:
   - Click Google or Apple buttons to redirect to their login pages.
   - Enter username and password. Empty fields show a red border and error message ("Username is required" or "Password is required") when focused.
   - Click the eye icon next to the password field to toggle visibility.
   - Submitting with empty fields triggers browser-native validation tooltips.
3. Customize as needed (e.g., add form submission logic or modify styles in `css/loginstyle.css`).

## Notes
- **Form Submission**: The form lacks an `action` attribute. Add a backend endpoint or JavaScript handler for submission.
- **JavaScript**: The password toggle requires JavaScript. Remove the toggle icon and script for a JavaScript-free version.
- **CSS**: Styles can be in `css/loginstyle.css` or inline in `index.html`. Current code assumes an external file.
- **Screenshot**: Capture the login page and save as `screenshots/login.png`. Update the path in this README if renamed.
- **Browser Compatibility**: Tested in modern browsers (Chrome, Firefox, Edge). HTML5 validation tooltips vary by browser.
- **Customization**:
  - Adjust error message styles in `.error-message` (e.g., color, font-size).
  - Modify colors (e.g., `#1DB954`) or sizes in `css/loginstyle.css`.

## License
Unlicensed, for educational purposes. Use and modify freely, but do not claim as official Spotify branding.