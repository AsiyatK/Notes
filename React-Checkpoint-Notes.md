## On the subject on passed-down props inside THAT component

The reason 'this.props' works and NOT 'props' on its own, is because we're receiving from the constructor where they were passed.

```js
console.log("THIS IS PROPS", Object.keys(this.props)); //<- WORKS
console.log("THIS IS PROPS", Object.keys(props)); //<- NEVER WORKS
```

RE: previewPet()

```js
/* this.setState({
      petToPreview : the returned pet object from this.props.pets.find using event.target.name
    })
    */
```
