# simple-LightMode
ES6 Module for easier implementation of changing the color scheme of the site. It simply just adds  classes to body element.

## How to use

In order to use this module , you simply need to import `import lightModeModule from 'lightMode'` and call `lightModeModule` function with parameters object.
Example
```
import lightModeModule from './modules/lightMode'
lightModeModule({
    buttonSelector:'#light-button',
    light:'white',
    dark:'black'
});
```
CSS
```
.white{
  --bg-color: white;
}
.black{
  --bg-color: black;
}
body{
  background-color : var(--bg-color);
}
```

## Parameters

- **buttonSelector** - selector for button to change the color scheme of the site
- **light** - class that is added to body for light theme (default : light)
- **dark** - class that is added to body for dark theme (default : dark)
- **startMode** - default theme (true - light , false - dark ) (default : true )
