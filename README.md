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
- When you use React.js, every JavaScript file in your application is invisible to every other JavaScript file by default. ProfilePage.js and NavBar.js can’t see each other.
- If you use an import statement, and the string at the end begins with either a dot or a slash, then import will treat that string as a filepath. import will follow that filepath, and import the file that it finds.If your filepath doesn’t have a file extension, then “.js” is assumed.Ex.,import { NavBar } from './NavBar';
- When you import a variable from a file that is not the current file, then an import statement isn’t quite enough. You also need an export statement, written in the other file, exporting the variable that you hope to grab.export and import are meant to be used together, and you rarely see one without the other.
- **this.props**:
-  a component can pass information to another component.Information that gets passed from one component to another is known as “props.”A component’s props is an object. It holds information about that component.
- to pass `Props` that is information to a component, you need a name for the information that you want to pass.
- By using this.Props.information name it helps to print value which is passed through the information name in render statement
- If <App /> is going to pass a prop to <Greeting />, then it follows that <App /> is going to render <Greeting />.this is called to pass Props components to components
- you attach any event handler to a JSX element: you give that JSX element a special attribute. The attribute’s name should be something like onClick or onHover. The attribute’s value should be the event handler that you want to attach.
-  If you are listening for a “keyPress” event, then you name your event handler handleKeyPress:
-  this.props.children will return everything in between a component’s opening and closing JSX tags.
-  If nobody passes any text to Button, then Button‘s display will be blank.then we can used default Props and give text to the button
-  **This.state**
-  React components will often need dynamic information in order to render.Dynamic Information is information that can changed There are two ways for a component to get dynamic information: props and state. Besides props and state, every value used in a component should always stay exactly the same.
-  A component changes its state by calling the function this.setState().
## Component Lifecycle Methods
- constructor() is the first method called during the mounting phase. 
- render() is called later during the mounting phase, to render the component for the first time, and during the updating phase, to re-render the component.
- Mounting, when the component is being initialized and put into the DOM for the first time. We saw that the constructor, render(), and componentDidMount() are called during this phase.
- Updating, when the component updates as a result of changed state or changed props.render() and componentDidUpdate() are called during this phase.
- Unmounting, when the component is being removed from the DOM. componentWillUnmount() was called here, which was a good time to clean things up.
## Hooks
- **Functional components**
-  function components can do everything that class components can do.
-  written as a stateless functional component:
syntax:export const MyComponentClass = () => {
  return <h1></h1>;
}
- function components can receive information that is props.syntax:export function NewFriend (props) {
		return ()}
