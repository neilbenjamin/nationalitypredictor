# Nationality Predictor: Unit Testing with React Testing Library

This project is a Create React App (CRA) that features a simple nationality prediction application, which fetches data from an external API based on user input. This `README.md` specifically highlights the **unit testing** aspect of the application, demonstrating how to effectively test asynchronous operations and component interactions using **React Testing Library** and Jest.

## 🌟 Features

* **Nationality Prediction Functionality:** (As described in the main app) Takes a name as input and predicts the most likely nationality using an external API.
* **Comprehensive Unit Tests:** Includes a dedicated unit test suite for the `FetchComponent` to ensure its functionality and reliability.
* **Asynchronous Testing:** Demonstrates best practices for testing components that perform asynchronous operations (like API calls) using `async/await` and `waitFor` from React Testing Library.
* **Mocking API Calls:** Utilizes `jest.fn().mockResolvedValue` to create a mock `fetch` function, simulating API responses without making actual network requests during tests. This ensures tests are fast and reliable.
* **Simulating User Interaction:** Employs `fireEvent` to simulate user input (typing into a textbox) and clicks on buttons, allowing for realistic testing of component behavior.
* **DOM Assertions:** Uses `expect().toBeInTheDocument()` and other assertions to verify that the component renders the correct information after data is fetched and processed.

## 📸 Screenshot

Here's a preview of the Nationality Predictor application's interface (the application that this test suite is for):

![Screenshot of the Nationality Predictor App](Screenshot%202025-07-06%20at%2000.07.53.png)

## 📦 Dependencies

This project relies on the following key dependencies, as listed in `package.json`:

* `react`: The core React library for building user interfaces.
* `react-dom`: Provides DOM-specific methods that can be used at the top level of a web app.
* `react-scripts`: A set of scripts and configuration used by Create React App projects.
* `@testing-library/react`: Tools for testing React components.
* `@testing-library/jest-dom`: Custom Jest matchers for asserting on DOM nodes.
* `@testing-library/user-event`: Simulates user interactions by dispatching the events that a user would dispatch.
* `web-vitals`: For measuring web performance.

## 🚀 How to Run the Project and Tests

**For this project to work, you must have Node.js installed on your system.**

If you don't have Node.js installed, please visit the [official Node.js website](https://nodejs.org/) to download and install it. You can verify your installation by opening your terminal or command prompt and typing `node -v` and `npm -v`.

**Once Node.js is installed, follow these steps:**

1.  **Clone or Download the Project:**
    Obtain the project files and navigate to the project's root directory in your terminal. This directory should contain the `package.json` file.

2.  **Install Dependencies:**
    Install all the necessary project dependencies as listed in `package.json`.
    ```bash
    npm install
    ```
    (Alternatively, if you use Yarn: `yarn install`)

3.  **Run the Tests:**
    To execute the unit tests for the application, use the following command:
    ```bash
    npm test
    ```
    (Or `yarn test`)

    This command will launch the test runner in interactive watch mode, showing the results of your tests.

4.  **Start the Development Server (to see the app):**
    If you wish to see the application in action, you can start the development server:
    ```bash
    npm start
    ```
    (Or `yarn start`)

    This command will open the application in your default web browser, usually at `http://localhost:3000`.

## ⚙️ Available Scripts

In the project directory, you can run:

* **`npm start`**
    Runs the app in the development mode.\
    Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

    The page will reload if you make edits.\
    You will also see any lint errors in the console.

* **`npm test`**
    Launches the test runner in the interactive watch mode.\
    See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

* **`npm run build`**
    Builds the app for production to the `build` folder.\
    It correctly bundles React in production mode and optimizes the build for the best performance.

    The build is minified and the filenames include the hashes.\
    Your app is ready to be deployed!

    See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

* **`npm run eject`**
    **Note: this is a one-way operation. Once you `eject`, you can’t go back!**

    If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project. Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc.) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them.

    You don’t have to use `eject`. The curated feature set is suitable for small and medium deployments, and you shouldn’t feel obligated to use this feature.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://react.dev/).

### Testing Resources:

* [Jest Documentation: Asynchronous Testing](https://jestjs.io/docs/asynchronous#promises)
* [FreeCodeCamp: How to Write Unit Tests in React Redux](https://www.freecodecamp.org/news/how-to-write-unit-tests-in-react-redux/)
* [OpenAI](https://openai.com/) (Consulted for assistance)
* Hyperion Dev (Course Material)