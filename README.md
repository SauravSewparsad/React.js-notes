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

