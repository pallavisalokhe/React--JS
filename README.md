# React--JS
## Introduction of react JSX
- JSX elements are treated as JavaScript expressions. They can go anywhere that JavaScript expressions can go.SX element can be saved in a variable, passed to a function, stored in an object or array…you name it.
- JSX elements can have attributes, just like HTML elements can.A single JSX element can have many attributes.(id,src,alt,width,height)are some attribute
- Neasted JSX means You can add JSX elements inside of other JSX elements, just like in HTML.Nested JSX expressions can be saved as variables, passed to functions
- To render a JSX expression means to make it appear onscreen.
- We can also Passing a Variable to ReactDOM.render()
- ReactDOM.render() is only updates DOM elements that have changed.That means if you render the exact same thing twice in a row, the second render will do nothing. It only updating the necessary DOM elements is a large part of what makes React so successful.this is called Virtual DOM.
- Class Vs ClassName:In HTML we use class attribute and in JSX we use className attribute because JSX gets translated into JavaScript, and class is a reserved word in JavaScript.
- In a self-closing tag forword slash / is compulsary.<img>,<br> are self closing tags
- JavaScript, written inside of a JSX expression, written inside of a JavaScript file.and when we add curly bracket {} we get output.
- Variables in JSX means that you can access variables while inside of a JSX expression, even if those variables were declared on the outside.
- The ternary operator works the same way in React as it does in regular JavaScript. 
- && works in conditionals that will sometimes do an action, but other times do nothing action
- If to create a list of JSX elements, then .map() is used
- A key is a JSX attribute.The attribute’s value should be something unique, similar to an id attribute.
- By using React.creatElement() we can write react code without using JSX.
## React components
-  React component is a small, reusable chunk of code that is responsible for one job, which often involves rendering HTML.
-  you have to import the React library, and save it in a variable named React
-  the DOM is used in React applications, but it isn’t part of React.Methods imported from 'react' are only for pure React purposes, such as creating components or writing JSX elements.
-  React.Component is a JavaScript class. To create your own component class, you must subclass React.Component. You can do this by using the syntax class YourComponentNameGoesHere extends React.Component {}.
-  Subclassing React.Component is the way to declare a new component class.
-  A render method must contain a return statement.
-  we can also use variable attributes in components
-  by putting logic in render before the return statement
-  the if statement is located inside of the render function, but before the return statement.
- Render functions often contain event listeners. 
## Components Interacting
- A React application can contain many of components.Each component might be small and relatively unremarkable on its own. When combined this get complex ecosystems of information.React special is the ways in which components interact.
- render methods return <div></div>s, <p></p>s, and <h1></h1> Render methods can also return component class <omg/>
- When you use React.js, every JavaScript file in your application is invisible to every other JavaScript file by default. ProfilePage.js and NavBar.js can’t see each other.
- If you use an import statement, and the string at the end begins with either a dot or a slash, then import will treat that string as a filepath. import will follow that filepath, and import the file that it finds.If your filepath doesn’t have a file extension, then “.js” is assumed.Ex.,import { NavBar } from './NavBar';
- When you import a variable from a file that is not the current file, then an import statement isn’t quite enough. You also need an export statement, written in the other file, exporting the variable that you hope to grab.export and import are meant to be used together, and you rarely see one without the other.
