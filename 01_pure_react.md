## Pure React

```
<!-- Html -->
<div id="root">not rendered</div>
<script src="https://unpkg.com/react@17.0.1/umd/react.development.js"></script>
<script src="https://unpkg.com/react-dom@17.0.1/umd/react-dom.development.js"></script>
```

```
<script>
const App =()=>{
    return React.createElement(
        'div',
        {},
        React.createElement('h1',{},'Adopt me!')
    )
}

ReactDOM.render(React.createElement(App),document.getElementById('root))
</script>
```

---

- React components 概念
- Components 分类
  - class 定义
  - function 定义

## Components

> React's dev warnings are trying to help your code run faster

```
const Pet = (props) => {
  return React.createElement("div", {}, [
    React.createElement("h1", {}, props.name),
    React.createElement("h2", {}, props.animal),
    React.createElement("h2", {}, props.breed),
  ]);
};

const App = () => {
  return React.createElement("div", {}, [
    React.createElement("h1", {}, "Adopt Me!"),
    React.createElement(Pet, {
      name: "Luna",
      animal: "Dog",
      breed: "Havanese",
    }),
    React.createElement(Pet, {
      name: "Pepper",
      animal: "Bird",
      breed: "Cockatiel",
    }),
    React.createElement(Pet, { name: "Doink", animal: "Cat", breed: "Mix" }),
  ]);
};

ReactDOM.render(React.createElement(App), document.getElementById("root"));
```
