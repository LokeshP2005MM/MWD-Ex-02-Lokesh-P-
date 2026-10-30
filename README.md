# Exp 02 - React Lab Exercise: Using Props
## NAME : Lokesh P
## REG NO: 2305001015
## Aim

To create a React application that demonstrates passing data from a parent component to a child component using props.

## Objectives

- To create a React project using Vite.
- To create a reusable Employee component.
- To pass employee details such as name, ID, department, and designation using props.
- To display multiple employees using the same component.
- To understand props destructuring and one-way data flow in React.

## Program

### Step 1: Create a React Project

```bash
npm create vite@latest props-demo -- --template react
cd props-demo
npm install
npm run dev
```

### Step 2: Create Employee.jsx

```jsx
function Employee({ name, id, department, designation }) {
  return (
    <div>
      <h2>Employee Details</h2>
      <p>Name: {name}</p>
      <p>ID: {id}</p>
      <p>Department: {department}</p>
      <p>Designation: {designation}</p>
      <hr />
    </div>
  );
}

export default Employee;
```

### Step 3: Write App.jsx

```jsx
import Employee from "./Employee";

function App() {
  return (
    <div>
      <h1>Employee Information</h1>

      <Employee
        Name="Lokesh P"
        ID="2305001015"
        Department="CSE"
        Designation="Full Stack Developer"
      />

      <Employee
        Name="abc123"
        ID="102"
        Department="IT"
        Designation="Web Developer"
      />

      <Employee
        Name="xyz456"
        ID="103"
        Department="AIDS"
        Designation="Data Analyst"
      />
    </div>
  );
}

export default App;
```

## Output

<img width="1407" height="767" alt="WhatsApp Image 2026-10-29 at 2 39 12 PM" src="https://github.com/user-attachments/assets/3568d11e-7752-40ea-a933-5735a69d4a71" />


## Result

Thus, a React application was successfully created and executed to demonstrate passing employee information from a parent component to a child component using props.
