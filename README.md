https://github.com/the-road-to-learn-react/the-road-to-learn-react/tree/master/manuscript


# reactjs
ReactJS Tutorial

React is a Library, not a Framework.

A library in programming can be explained as a collection of codes. We use a library to 
write code in a much simpler way or to import a feature from it into our project. 
JQuery is a library for example.


What is the benefit of Virtual DOM?
Each time you make a change in the code, DOM will be completely updated and rewritten. 
This is an expensive operation and consumes lots of time. In this point, React provides a solution: The Virtual DOM.

So when something changes:
React first creates an exact copy of the DOM
Then React figures out which part is new and only updates that specific part in the Virtual DOM
Finally, React copies only the new parts of the Virtual DOM to the actual DOM, rather than completely rewriting it.
This approach makes a webpage much faster than a standard webpage. 
That’s also one of the reasons why React is so popular.


In classic Frontend programming, we have separated HTML, CSS and JS file structures. 
React is a bit different. We don’t have separated HTML files in React.

JSX (JavaScript XML) is a syntax extension to JavaScript used by React. 
JSX is basically used to write HTML tags inside JavaScript.

In JSX syntax, we write HTML tags inside JavaScript.

e.g: const element = <h1>Hello!</h1>;

React doesn’t have HTML files, HTML tags are rendered directly inside JavaScript. T
his approach makes React faster.

To start a project:

npx create-react-app hello-world-app
cd hello-world-app
Finally, type npm start


It is absolutely possible to run a React app without a production node server. That being said, developers may need to use a node dev server locally via npm start, as well as 
using node to perform production builds via npm run build. But one can take the build output from npm run build and serve it from any static server and have a working react application.

 // JavaScript ES5 function
function getGreeting() {
  return 'Welcome to JavaScript';
}
 
// JavaScript ES6 arrow function with body
const getGreeting = () => {
  return 'Welcome to JavaScript';
}


// JavaScript ES6 arrow function without body and implicit return
const getGreeting = () => 'Welcome to JavaScript';

Tutorial for javascript to get ready for React and ES6 ->  https://www.robinwieruch.de/javascript-fundamentals-react-requirements



Template literals are another JavaScript language specific feature that came with JavaScript ES6. 
It is worth to mention it shortly, because when people new to JavaScript and React see them, they can be confusing as well. 
When learning JavaScript, it's the following syntax that you grow up with for concatenating a string:

function getGreeting(what) {
  return 'Welcome to ' + what;
}
 
const greeting = getGreeting('JavaScript');
console.log(greeting);
// Welcome to JavaScript

Template literals can be used for the same which is called string interpolation:

function getGreeting(what) {
  return `Welcome to ${what}`;
}

You only have to use backticks and the ${} notation for inserting JavaScript primitives. 
However, string literals are not only used for string interpolation, but also for multiline strings in JavaScript:

function getGreeting(what) {
  return `
    Welcome
    to
    ${what}
  `;
}
Basically that's how larger text blocks can be formatted on multiple lines.

Template Literals are a new ES2015 / ES6 feature that allows you to work with strings in a novel way compared to ES5 and below.

The syntax at a first glance is very simple, just use backticks instead of single or double quotes:

const a_string = `something`

advantages:
-they offer a great syntax to define multiline strings
-they provide an easy way to interpolate variables and expressions in strings
-they allow you to create DSLs with template tags (DSL means domain specific language, and it’s for example used in React by Styled Components, to define CSS for a component)

https://flaviocopes.com/javascript-template-literals/

Template literals provide an easy way to interpolate variables and expressions into strings.

You do so by using the ${...} syntax:

const myVariable = 'test'
const string = `something ${myVariable}` //something test
inside the ${} you can add anything, even expressions:

const string = `something ${1 + 2 + 3}`
const string2 = `something ${doSomething() ? 'x' : 'y'}`


https://www.robinwieruch.de/npm-crash-course
Set up a throw away npm project using the terminal:
	Create a new folder with mkdir <folder_name>
	Navigate into the folder with cd <folder_name>
	Execute npm init -y or npm init
	Install a local package like React with npm install react
	Check the package.json file and the node_modules/ folder
	Attempt to uninstall and reinstall the react node package




JSX — Allows us to write HTML like syntax which gets
transformed to lightweightJavaScript objects.

Virtual DOM — A JavaScript representation of the actual
DOM.

React.Component — The way in which you create a new component.

render (method) — Describes what the UI will look like for
the particular component.

ReactDOM.render — Renders a React component to a DOM node.

state — The internal data store (object) of a component.

constructor (this.state) - The way in which you establish
the initial state of a component.

setState — A helper method used for updating the state of a
component and re-rendering the UI

props — The data which is passed to the child component
from the parent component.

propTypes — Allows you to control the presence, or types of
certain props passed to the child component.

defaultProps — Allows you to set default props for your component.

Component LifeCycle
  - componentDidMount — Fired after the component mounted
  - componentWillUnmount — Fired before the component will unmount
  - getDerivedStateFromProps - Fired when the component mounts and
whenever the props change. Used to update the state of a
component when its props change

Events
  - onClick
  - onSubmit
  - onChange
