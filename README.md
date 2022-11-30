# React App From Scratch
###### These are the steps that I followed inorder to create a react app from scratch `with out using npx create-react-app`

### Step 1
  > npm init -y
  * This command will create a package.json file that contains the name and version of the application.
  
### Step 2
  > npm install react react-dom react-scripts 
  * This command will install ***3*** modules, ***react*** that is need to create the ui, ***react-dom*** that is a glue to react and browser dom 
  and ***react-scripts*** that is responsible for running the application. **NOTE** This will also create a node_module folder and will also add 
  dependencies section in package.json file.
  
 ### Step 3
  > Create a src folder and create App.js and index.js files in it. 
  * App.js file contains the following code.
  ```javascript
  import React from "react";
  export default function App() {
      return <>
          <div>
              <h1>React app from scratch. ╰(*°▽°*)╯</h1>
          </div>
      </>
  }
  ```
  * index.js contains the following code.
  ```javascript
    import React from "react";
    import ReactDOM from "react-dom";
    import App from "./App";
    ReactDOM.render(<App/>,document.querySelector("#root"));
  ```
 ### Step 4
 > Create a public folder and add index.html file
 * This html file must contain a div with id ***root***
 
 ### Step 5
> Add the following script attribute to the package.json
```json
"scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject"
  }
  ```
### Step 6
> npm start 
* This will start you react application, for the first time it might ask to add defaults to your package.json just press y.

###### React application is now built 🥳
