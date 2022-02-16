# Demo

## Demo

### Demo

#### Demo

##### Demo

Demo

# The React Cheatsheet for 2022

Do you want to get up to speed with React as quickly as possible?

I’ve put together a super helpful cheatsheet to give you a complete overview of all of the React concepts you need to know in 2022.

Let’s get started!

## Table of Contents
.[React Elements](https://github.com/PAVAN-221/Demo/blob/main/README.md#react-elements)<br/>
.[React Element Attributes]()<br/>
.[React Element Styles]()<br/>
.[React Fragments]()<br/>
.[React Components]()<br/>
.[React Props]()<br/>
.[React Children Props]()<br/>
.[React Conditionals]()<br/>
.[React Lists]()<br/>
.[React Context]()<br/>
.[React Hooks]()<br/>
.[React useState Hook]()<br/>
.[React useEffect Hook]()<br/>
.[React useRef Hook]()<br/>
.[React useContext Hook]()<br/>
.[React useCallback Hook]()<br/>
.[React useMemo Hook]()<br/>

## React Elements
React elements are written just like regular HTML elements. You can write any valid HTML element in React.
```
<h1>My Header</h1>
<p>My paragraph>
<button>My button</button>
```
We write React elements using a feature called *JSX*

However, because JSX is really just JavaScript functions (and not HTML), the syntax is a bit different.

Unlike HTML, single-tag elements (like the img element), must be self-closing. They must end in a forward slash ```/```:

```
<img src="my-image.png" />
<br />
<hr />
```
## React Element Attributes
Additionally, JSX requires a different syntax for its attributes.

Since JSX is really JavaScript and JavaScript uses a camelcase naming convention (that is, “camelCase”), attributes are written differently than HTML.

The most common example is the ```class``` attribute, which we write as ```className```.

```<div className="container"></div>```

## React Element Styles
To apply inline styles, instead of using double quotes (“”), we use two sets of curly braces.

Inline styles are not written as plain strings, but as properties on objects:

```<h1 style={{ fontSize: 24, margin: '0 auto', textAlign: 'center' }}>My header</h1>```

## React Fragments
React also gives us an element called a *fragment*.

React requires that all returned elements be returned within a single “parent” component.

For example, we can’t return two sibling elements, like an h1 and a paragraph from a component:

```
// this syntax is invalid
function MyComponent() {
  return (
    <h1>My header</h1>
    </p>My paragraph</p>
  );
}
```
If we don’t want to wrap our elements in a container element like a div, we can use a fragment:
```
// valid syntax
function MyComponent() {
  return (
    <>
      <h1>My header</h1>
      </p>My paragraph</p>
    </>
  );
}
```
We can write fragments in a regular or shorthand syntax: <React.Fragment></React.Fragment> or <></>.
## React Components
We can organized groups of elements into React components.

A basic function component is written similarly to a regular JavaScript function with a couple of differences.

 1.Component names must start with a capital letter (that is, MyComponent, instead of myComponent)<br/>
 2.Components, unlike JavaScript functions, must return JSX.
 
Here is the basic syntax of a React function component:
```
function App() {
  return (
     <div>Hello world!</div>
  );
} 
```
