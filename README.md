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
