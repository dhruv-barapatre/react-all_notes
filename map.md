# 🚀 React Learning Roadmap (2025 Edition)

## 🔰 Phase 1: React Fundamentals (Beginner Level)
📌 **Goal:** Understand the basics of React and JSX

* **Topic:** **Learn JSX**
    * Syntax, expressions (`{}`), attributes, embedding JavaScript logic.
    * Understanding JSX as syntactic sugar for `React.createElement`.
    * JSX Fragments (`<> </>`) for grouping elements.
* **Topic:** **Functional Components**
    * Component creation as JavaScript functions.
    * Props: Passing data down the component tree (read-only).
    * Component composition: Rendering components within other components.
    * Returning JSX from components.
* **Topic:** **`useState`**
    * State management within functional components.
    * Declaring and updating state variables using the `useState` hook.
    * Understanding state immutability and the setter function.
    * Reading state values.
* **Topic:** **Event Handling**
    * Inline event handlers.
    * Creating separate event handler functions.
    * Accessing the event object.
    * Synthetic events in React.
    * `onClick`, `onChange`, `onSubmit`, `onKeyDown`, etc.
    * Preventing default browser behavior (`event.preventDefault()`).
    * Stopping event propagation (`event.stopPropagation()`).
* **Topic:** **Conditional Rendering**
    * `if/else` statements within JavaScript blocks.
    * Ternary operator (`condition ? true : false`).
    * Logical AND operator (`&&`) for short-circuit evaluation.
    * Logical OR operator (`||`).
* **Topic:** **Lists & Keys**
    * Rendering dynamic lists using `.map()`.
    * The importance of the `key` prop for efficient updates.
    * Choosing appropriate key values (unique and stable).
    * Best practices for rendering collections.

📘 **Mini Project:** Counter App, Todo App (with local state, adding, deleting, marking as complete)

## ⚙️ Phase 2: React Essentials (Intermediate Level)
📌 **Goal:** Build small apps with routing, effects, and form handling

* **Topic:** **`useEffect`**
    * Side effects in functional components (data fetching, subscriptions, timers, manual DOM manipulations).
    * The dependency array: controlling when effects run.
    * Cleanup functions: preventing memory leaks.
    * Understanding the different dependency array scenarios (`[]`, no array, `[dependencies]`).
* **Topic:** **`useRef`**
    * Accessing DOM elements directly.
    * Persisting values across renders (without causing re-renders).
    * Managing focus, controlling media elements, triggering animations.
* **Topic:** **Forms**
    * **Controlled Components:** Managing form state with React state. Handling `onChange` to update state on input changes. Binding state to input `value` prop.
    * **Uncontrolled Components:** Relying on DOM refs to get form values. When to use them.
    * Handling form submissions (`onSubmit`).
    * Input validation (client-side).
    * Handling different input types (`<input>`, `<textarea>`, `<select>`, checkboxes, radio buttons).
    * Managing multiple form fields.
* **Topic:** **Routing**
    * **React Router DOM:** Installation and setup.
    * `<BrowserRouter>`: Creating a router instance.
    * `<Routes>` and `<Route>`: Defining application routes and their corresponding components.
    * `<Link>` and `<NavLink>`: Navigating between routes.
    * `useParams()`: Accessing route parameters.
    * `useNavigate()`: Programmatic navigation.
    * Nested routes and layout components.
* **Topic:** **Lifting State Up**
    * Sharing state between sibling components by moving it to their common ancestor.
    * Passing down setter functions as props.
    * Understanding the flow of data in React.
* **Topic:** **Context API**
    * Avoiding prop drilling for deeply nested components.
    * `createContext()`: Creating a context object.
    * `<Provider>`: Making context values available to consuming components.
    * `useContext()`: Accessing context values in functional components.
    * When to use Context API vs. more advanced state management.

📘 **Mini Project:** Blog Viewer (with multiple pages for articles, dynamic routing for article details, using `useEffect` to fetch mock data, simple form for comments using controlled components)

## 🧠 Phase 3: Advanced React Concepts
📌 **Goal:** Master hooks, optimizations, and reusable logic

* **Topic:** **Custom Hooks**
    * Creating reusable logic by extracting stateful logic into custom functions.
    * Naming conventions for custom hooks (`use...`).
    * Sharing state and behavior across multiple components.
* **Topic:** **`useMemo` & `useCallback`**
    * **`useMemo`:** Memoizing expensive calculations to avoid re-computation on every render.
    * **`useCallback`:** Memoizing callback functions to prevent unnecessary re-renders of child components that receive them as props.
    * Understanding dependency arrays for memoization.
* **Topic:** **`React.memo`**
    * Memoizing functional components to prevent re-renders if props haven't changed (shallow comparison).
    * When to use `React.memo` for performance optimization.
* **Topic:** **Higher-Order Components (HOC) & Render Props**
    * (For legacy understanding and working with older libraries).
    * **HOC:** Wrapping components to share functionality.
    * **Render Props:** Passing a function as a prop to share rendering logic.
    * Understanding their purpose and how they compare to custom hooks.
* **Topic:** **Error Boundaries**
    * Gracefully handling JavaScript errors in component trees.
    * `componentDidCatch` lifecycle method (for class components).
    * Static `getDerivedStateFromError` lifecycle method (for class components).
    * Creating error boundary components to wrap potentially failing parts of the UI.

📘 **Project:** Weather App (fetching data from a weather API, using custom hooks for data fetching and location handling, optimizing rendering with `useMemo` and `useCallback`) or Expense Tracker (managing transactions, using custom hooks for filtering and sorting, optimizing list rendering).

## 📦 Phase 4: Real-World React
📌 **Goal:** Work with APIs, authentication, state management, and deployment

* **Topic:** **State Management**
    * **Redux Toolkit:** Setting up a Redux store, defining slices (reducers and actions), dispatching actions, selecting state. Asynchronous actions with Thunks.
    * **Zustand:** Simpler state management with stores, selectors, and actions.
    * Understanding the trade-offs between different state management solutions.
* **Topic:** **Async Redux**
    * **Redux Thunk:** Writing action creators that return functions to handle asynchronous operations (API calls).
    * **RTK Query:** Data fetching and caching utility built into Redux Toolkit. Defining API endpoints, handling loading and error states automatically.
* **Topic:** **API Integration**
    * Working with RESTful APIs.
    * Using `fetch` API or libraries like Axios for making HTTP requests.
    * Handling different HTTP methods (GET, POST, PUT, DELETE).
    * Working with request and response data (JSON).
    * Handling loading states and error states during API calls.
* **Topic:** **Authentication**
    * Implementing JWT (JSON Web Tokens) based authentication.
    * Handling user login and signup.
    * Storing and managing authentication tokens (local storage, cookies - considerations for each).
    * Implementing private routes: protecting certain parts of the application for authenticated users.
    * Role-based access control (basic implementation).
* **Topic:** **Protected Routes**
    * Creating components that conditionally render based on user authentication status.
    * Using React Router features to implement route protection.
* **Topic:** **Middleware-like logic in React Router**
    * Implementing custom route protection logic.
* **Topic:** **React Query**
    * Declarative data fetching, caching, synchronization, and updating.
    * Queries, mutations, invalidation.
    * Handling background updates and stale data.
    * Pagination and infinite scrolling.

📘 **Project:** Full Auth App (user registration, login, protected dashboard with user-specific data fetched from an API) or a basic e-commerce store front (displaying products fetched from an API, simple cart functionality, user authentication for checkout).

## 🧪 Phase 5: Professional Development (Expert Level)
📌 **Goal:** Make production-grade apps and get job-ready

* **Topic:** **Testing**
    * **Unit Testing:** Testing individual components and functions in isolation using Jest and React Testing Library. Writing effective test cases. Mocking dependencies (components, modules, APIs). Testing component behavior and rendering.
    * **Integration Testing:** Testing how different components interact with each other. Testing user flows.
    * **End-to-End (E2E) Testing:** Testing the entire application from the user's perspective using tools like Cypress or Selenium.
    * **Mocking APIs:** Setting up mock API responses for testing purposes.
* **Topic:** **TypeScript with React**
    * Adding static typing to React applications.
    * Defining prop types using interfaces and types.
    * Typing `useState` and `useEffect` hooks.
    * Typing Redux actions, reducers, and state.
    * Benefits of using TypeScript for larger projects.
* **Topic:** **Next.js (Optional SSR/SSG)**
    * Understanding Server-Side Rendering (SSR) and Static Site Generation (SSG).
    * File-based routing in Next.js.
    * Fetching data in Next.js (`getServerSideProps`, `getStaticProps`, `getStaticPaths`, client-side fetching).
    * API routes in Next.js.
    * Deployment of Next.js applications.
* **Topic:** **Deployment**
    * Deploying React applications to platforms like Vercel, Netlify, Firebase Hosting, AWS Amplify, GitHub Pages.
    * Understanding build processes and environment variables.
* **Topic:** **CI/CD Basics**
    * Introduction to Continuous Integration and Continuous Deployment.
    * Setting up basic CI/CD pipelines using GitHub Actions or Netlify integrations for automated building and deployment.
* **Topic:** **Code Splitting**
    * Improving application performance by splitting the code into smaller chunks.
    * Lazy loading components with `React.lazy` and `Suspense`.
    * Route-based code splitting.

📘 **Capstone Project:** A more complex e-commerce store with user authentication, product listings, cart management, checkout process (potentially with a mock backend), and unit/integration tests. Or an Admin Dashboard with user management, data visualization (using a charting library), and protected routes.

## ✅ Bonus: Supporting Skills
* **Git & GitHub:** Version control, branching, merging, pull requests, collaboration.
* **ES6+ JavaScript:** Destructuring, spread/rest operators, arrow functions, promises, async/await, array methods (`map`, `filter`, `reduce`), object literals, classes, modules.
* **DevTools:** Browser developer tools (React DevTools extension, Network tab, Console, Elements).
* **Design Systems:** Understanding and using UI libraries like Tailwind CSS (utility-first), Material UI, Chakra UI, Ant Design.
