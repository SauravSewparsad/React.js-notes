# React.js-notes

# Introduction and onboarding

software development roadmap
- The Software Development Program equips candidates with the skills to develop full-stack web development business needs, enabling them to create apps, websites, databases, and desktop solutions.
- The program has been structured into 3 sections, each with specific courses. This course: React.js forms part of Front-End Web Development.
- Successful candidates are not only job ready, but can also gain a PCAP Certified Associate in Python Programming / Oracle Certified Professional Developer Certificate or a suitable alternative vendor qualification such as National Certificate: Information Technology Systems Development NQF Level 5

Course focus
- Welcome to the React.js course. This course introduces you to Software Development, what is expected of you, and how you will keep track of your progress.
- React is the library for web and native user interfaces. You will be able to build user interfaces out of individual pieces called components written in JavaScript.
- To help you navigate this fast-changing environment, this course is designed with that in mind. We're going to start with the easy stuff and gradually build up to more complex concepts
------------------------------------------------------

# Introduction to React.js

module focus
- This course covers React basics, focusing on reusable components for UI development.
- React.js is a standout among various JavaScript libraries.
-  It covers setting up Chrome tools, creating components, working with React Hooks, and using the Create React App for testing.
-  The goal is to confidently build browser-based projects.

Introduction to react
- React, a Facebook-founded JavaScript library, was open-sourced in 2013.
- It has evolved into React Native, enabling the creation of native mobile apps.
- React Docs provide regular updates and updates.
- React's popularity stems from its user-friendly interface and efficient component architecture, attracting major players like Twitter, Netflix, and Microsoft for its ability to streamline product development.
------------------------------------------------------------------
# React elements

Putting react in a project
-  React uses JavaScript to create elements, like a div with ID "root", and requires a script tag with type "text/javascript" and "ReactDOM.render" for two arguments.
-  First, "React.createElement" creates the element we want. For instance, replicate the h1 with React: "h1," null (no additional properties), and "getting started with React."
-  The second argument specifies where to place the element - here, "document.getElementById('root')." This says, "Render this element and put it inside the 'root' div." Save, refresh, and voila! We have  successfully created our first React element.

 Creating react elements
 - We're using ReactDOM.render to insert the createElement call from line 19 into the 'root' element, viewing it as a tiny UI component that can be rendered as needed.
 - To create a variable, cut and paste the entire section, add 'heading', and test the 'Getting Started with React' text with exclamation marks. This approach generates a React element using its dedicated variable.
 - To create a variable, cut and paste the entire section, add 'heading', and test the 'Getting Started with React' text with exclamation marks. This approach generates a React element using its dedicated variable.

Refactoring elements using JSX
- To turn your heading to a bulleted list we will turn it into an ul using React.createElement, and to add list items, we just need to tweak the third argument.
- Think of it as the instructions for what we are creating. For instance, we can throw in style: color, blue to give it a cool shade. Now, let's dive into the child elements. We start with a list item, null, and Monday. Simple. Adding more days is a breeze - Monday, Tuesday, Wednesday, and we are rolling.
- The UI uses JSX, a JavaScript superhero helper, to create emoji lists. However, React doesn't work with JSX tags.

Incorporating babel
- JSX, a tag-based syntax, is not browser-friendly.
- To make your code more user-friendly, use babeljs.io as a compiler tool.
- To optimize your JavaScript code, use a CDN link like unpkg.com/babel-standalone@6/babel.min.js and adjust the 'text/javascript' to 'text/babel' to fix syntax errors. Babel is essential for new JavaScript features.

JSX Syntax
- JSX is a powerful tool for incorporating dynamic content into your apps. It allows you to reference variables with variable names, like "robot" for a robot, "cowboy" for a cowboy, and "moon" for a friendly moon.
- These values are displayed in list items using curly braces.
- JSX expressions with curly braces can be incorporated with functions like "toUpperCase()" or "name.length".
--------------------------------------------

# React Components

React components
- Build react components
     + The text explains the process of creating elements and crafting a component, a small user interface piece in an application, which is a JavaScript function that executes JSX.
     +
       ![Screenshot 2024-04-17 091708](https://github.com/SauravSewparsad/React.js-notes/assets/101722970/1229221b-7001-4402-ad67-18e2eda8ae07)
     + Just like before, we render it, and boom! "We serve the most delicious food around" proudly takes its place on our page. Now, here is a little trick. You might be tempted to slam the Header and Main together side by side. Hold your horses! React insists on a single component, so toss them into a div. Voila! Problem solved.
     +
        ![Screenshot 2024-04-17 092115](https://github.com/SauravSewparsad/React.js-notes/assets/101722970/accaca29-0138-48f7-bf12-a4436a2bb4fa)


Introducing Component Properties
- The text outlines the use of components to display live data in a restaurant.
- The plan involves adding props to the header function, which is then refreshed and filled with the user's name.
- The values are then retrieved from the props object, such as "Cindy's Kitchen", to create a more personalized experience.
- This approach allows users to see their own name instead of Eve's.
- The main component can showcase delicious food by using a {props.adjective} attribute and a period for style.
- A new property for the footer component allows for a copyright year from props. Using curly braces and a function like {new Date().getFullYear()} can increase dynamism and add a number for properties.

Working with Lists
- We've used JSX expressions to send data to components, handling simple strings like "Cindy" and "amazing" and date functions and booleans. Now, we're considering more complex data types.
- To showcase the menu in the main component, map over it using dishes.map and return a list item for each dish.
- The dishes variable can be accessed through props, but a console warning is needed for each child in a list.

Applying keys to list items
- Two JavaScript approaches were discussed: adding an index for each item in the array, which could cause rendering issues, and creating an array with unique IDs for each dish, ensuring data stability and maintaining key synchronization during dynamic value iteration.

Image display with React.js
- We will use the first one, just right-clicking and copying the image address.
- Now, jump into your component, maybe the main one. Slap an image tag in there, and toss in the source with the URL we snagged.
- Hit refresh and boom, the picture is in the house.
- Do not forget the alt attribute – that is a caption for screen readers. We have used  "A server presenting two plates at a fancy restaurant." 
- Feeling fancy? Save that image to your computer, maybe call it "restaurant." Open your files, drag them into the start folder, and update your source to something like "./restaurant.jpg" for local swagger.
- Two ways to do the same thing: URL or local file. Take your pick!

React Fragments
- There is a div for root, then another, and finally, we reach the actual components on the page. Instead of a div, consider using a React Fragment.
- Add React.Fragment to create a neat div root for header, section, and footer components, requiring specific React versions.
- Shorter syntax requires specific versions.
------------------------------------------------------------

# React States

Building a Project with Create React App
- We have been using an index.html file to host our React components and test them locally in the browser. It has worked well, but now we will look at a project using a tool called Create React App. It is like a shortcut to set up a React project with things like Babel and file bundling.
- To create a React app, navigate to the correct terminal folder, check Node.js installation, run 'node -v' and 'npm -v', and install React and other essentials.
- Move to the project folder, start it with 'npm start', and open localhost:3000 in a browser.

Navigating a Create React App Project
- So, our project is generated in the start folder of the React app. In the package JSON, you will find all the dependencies, with the key ones being React (for creating components), React DOM (for adding them to the page), and React Scripts (for bundling).
- The testing libraries are in the dependencies section, with index.js being the main JavaScript file for rendering the app on the DOM, using document.getElementByID.
- Run the React app using 'NPM start' on localhost:3000, allowing instant changes, real-time CSS imports, and automatic class name application, enhancing the experience over traditional HTML development.

Destructuring Arrays and Objects
- Destructuring is a crucial JavaScript concept that allows dynamic retrieval of properties from the props object in the app.js file, enhancing clarity and allowing direct property extraction by their keys.
- Array destructuring assigns variable names based on their positions in the array, allowing us to console log specific values like "Tokyo" or "Tahoe City." Understanding both is crucial for upcoming lessons.

The useState Hook
- The useState function is a crucial method for managing state variables in React applications.
- It imports the state variable from React, discards destructured arrays, and updates the initial state with an undefined value.
- The initial state of an application can be set using a value passed to useState, such as 'happy'.
- This creates a value called 'emotion' and an updating function called'setEmotion'.
- This method allows dynamic state management throughout the application, regardless of the initial value passed.

Working with useEffect
-  there is this handy tool called useEffect, which is like a secret weapon in the library. It is a bit tricky but super useful.
-  First off, import useEffect from React, toss it into your app component, and instead of plugging in an array, throw in a function.
-  For instance, let's log the current emotion. Now, this is a side effect — it does not wait for a render, just does its thing alongside it.

The Dependency Array
- UseEffect and useState calls manage variables, including secondary variable "emotion" with initial state "tired".
- UseEffect handles emotions, including dependency arrays for tracking changes. Include state variables for useEffect to trigger on changes, ensuring proper tracking.

Using the useReducer
- The next step is to simplify state management by creating a checkbox that works with useState.
- This will be done by creating a variable called "checked" and its partner "setChecked," both of which will be set to false, simplifying state management.
- The "checked" variable is responsible for the checkbox state, so manipulating it can shake things up.
- OnChange will serenade setChecked, returning its alter ego. The label will echo this change, initially false. Toggle checked to toggle the state.
- The text suggests outsourcing state updates to a separate function, like useReducer, instead of juggling it inside onChange.
- This allows for a consistent state update and initial state, ensuring that the output remains cool and avoids bugs by avoiding extra onChange code.
--------------------------------------------------------------

# React Forms

Working with Uncontrolled Components
- In a React project, handling form inputs is crucial.
- The useRef hook allows access to individual elements like text and color inputs, allowing us to retrieve their values using current.
- This allows us to create an uncontrolled component without triggering re-render.

Creating Controlled Form Elements
- Forms can be managed using state, transitioning from uncontrolled to controlled components.
- By removing useRef, setting up state variables, and using onChange events, forms become controlled components, directly interacting with input values.

Building a Custom Hook
- React hooks enable the creation of custom hooks for various functionalities, simplifying form structures and enabling user input management.
- Hooks are like tools in a toolbox, ready for efficient and clean code across projects.

Choosing a Form Library
- Formik and React Hook Form are excellent form libraries for comprehensive management and advanced TypeScript support, respectively.
- Usehooks.com offers resources for creating various hooks, streamlining form-related tasks and allowing users to choose tools best suited to their project needs.
