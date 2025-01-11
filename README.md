# Password Generator Application

This application is a simple password generator built with React. It allows users to generate random passwords based on selected criteria, such as including numbers and special characters. The generated password can be easily copied to the clipboard.

## Features
- **Password Length Selection**: Users can adjust the password length between 6 and 15 characters using a slider.
- **Include Numbers**: An option to include numbers in the generated password.
- **Include Special Characters**: An option to include special characters in the password.
- **Copy to Clipboard**: A button to copy the generated password to the clipboard.

## Components

### `App`
The main component that manages the state and renders the UI for the password generator.

#### State Variables:
- `lenght`: The length of the password (default is 8).
- `numberAllowed`: Boolean to indicate if numbers should be included.
- `charAllowed`: Boolean to indicate if special characters should be included.
- `password`: The generated password.

#### Refs:
- `passwordRef`: Reference to the input field containing the generated password.

#### Functions:
- `passwordGenerator`: Generates a random password based on the selected criteria.
- `copyPasswordToClibBoard`: Copies the generated password to the clipboard.

## UI Elements
- **Password Display**: An input field to display the generated password (read-only).
- **Copy Button**: A button to copy the password to the clipboard.
- **Length Slider**: A range input to select the length of the password.
- **Checkboxes**: Options to include numbers and special characters in the password.

## Usage
1. Clone the repository and navigate to the project directory.
2. Install dependencies using `npm install`.
3. Run the application using `npm start`.
4. Adjust the password length and toggle the options to include numbers and special characters.
5. Click the "copy" button to copy the generated password to the clipboard.

## Notes
- The application uses the `useState` hook to manage state and the `useEffect` hook to trigger the password generation whenever the relevant state changes.
- The `useCallback` hook is used to memoize the functions `passwordGenerator` and `copyPasswordToClibBoard` for better performance.
- The application includes CSS styles in `App.css` to style the components.

---

Place this file in the `README.md` file in your project's `readme` folder for use in VS Code.

