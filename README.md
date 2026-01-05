# React Props Practice

This project demonstrates how to use **props** in React to pass data from parent components to child components.

## What I Learned

### 1. What are Props?
- Props (short for "properties") are read-only inputs passed from parent to child components
- They allow components to be dynamic and reusable with different data
- Props are accessed using `props.propertyName` in the child component

### 2. Passing Different Data Types
In this project, I passed various data types as props:
- **Strings**: `name="Spongebob"` (with quotes)
- **Numbers**: `age={42}` (with curly braces)
- **Booleans**: `isStudent={true}` (with curly braces)

### 3. Using Props in Components
The `Student` component receives props and displays them:
```javascript
<p>Name: {props.name}</p>
<p>Age: {props.age}</p>
<p>Student: {props.isStudent ? "Yes" : "No"}</p>
```

### 4. Conditional Rendering with Props
- Used the ternary operator to display "Yes" or "No" based on the boolean `isStudent` prop
- Syntax: `{condition ? valueIfTrue : valueIfFalse}`

### 5. Default Props (Attempted)
- Tried using `defaultProps` to provide fallback values when props aren't passed
- Note: This approach doesn't work in newer React versions (needs alternative solutions)

## Project Structure

- `App.jsx`: Parent component that renders multiple `Student` components with different props
- `Student.jsx`: Reusable child component that displays student information

## Key Concepts

- **Props are read-only**: Child components cannot modify props received from parents
- **Component Reusability**: Same component (`Student`) used multiple times with different data
- **Unidirectional Data Flow**: Data flows from parent to child, not the other way around
- **Dynamic Content**: Props make components flexible and dynamic
