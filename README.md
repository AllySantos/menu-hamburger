# Menu Hamburger
A clean, simple and easy to use library

# Installation
#### Via packages
```
yarn add menu-hamburger 
```
or
```
npm i menu-hamburguer
```
#### Via CDN
```
<script type="text/javascript" src="https://unpkg.com/menu-hamburger@2.0.0/lib/menu-hamburger.min.js"></script>
```
# Usage

### HTML
``` html 
<!DOCTYPE html>
<html>
<head>
  <title>A Simple Menu Hamburger</title>
  <script src="https://unpkg.com/menu-hamburger@2.0.0/lib/menu-hamburger.min.js"></script>
</head>
<body>
  <div id="menu-wrapper"></div>
  <script type="text/javascript">
  	//Js code here
  </script>
</body>
</html>
``` 
### JavaScript - CDN
``` javascript
const rootElement = document.getElementById("menu-wrapper");
const menu = MenuHamburger.initialize({
  rootElement,
  size: 50,
  backgroundColor: "#f2f2f2",
});
```
### JavaScript - Package
``` javascript
import MenuHamburger from "menu-hamburger";

const rootElement = document.getElementById("menu-wrapper");
const menu = MenuHamburger.initialize({
  rootElement,
  size: 50,
  backgroundColor: "#f1f1f1",
});
```
# Config
Configure Menu Hamburger by passing an options object as the argument of the initialize method. Default values are:
``` javascript
const menu = MenuHamburger.initialize({
  rootElement: null,
  size: 30,
  lineWidth: 3,
  menuClassName: null,
  menuIconClassName: null,
  transition: 'all .2s ease-in-out',
  backgroundColor: 'white',
  borderRadius: '8px',
  iconColor: '#444',
});
```
#### `rootElement`
> Receives the HTML container element from the menu

required: `true`  
type: `HTMLNode`  
Allowed values: `any HTML Node`  
Default value: `null`

#### `size`
> Receives the Menu Hamburger width and height

required: `false`  
type: `number`  
Allowed values: `any number`  
Default value: `30`

#### `lineWidth`
> Receives the Menu line width

required: `false`  
type: `number`  
Allowed values: `any number`  
Default value: `3`

#### `menuClassName`
> Receives the class to apply on the Menu Node

required: `false`  
type: `string`  
Allowed values: `any valid HTML class string`  
Default value: null

#### `menuIconClassName`
> Receives the class to apply on the Menu Node Icon

required: `false`  
type: `string`  
Allowed values: `any valid HTML class string`  
Default value: null

#### `transition`
> Receives the custom Css transition

required: `false`  
type: `string`  
Allowed values: `any valid value to Css property transition`  
Default value: "all .2s ease-in-out"

#### `backgroundColor`
> Receive the Background Color of Menu

required: `false`  
type: `string`  
Allowed values: `any Css color`  
Default value: "white"

#### `borderRadius`
> Receive the Menu border radius

required: `false`  
type: `string`  
Allowed values: `any Css size`  
Default value: "8px"

#### `iconColor`
> Receive the Menu Icon color

required: `false`  
type: `string`  
Allowed values: `any Css color`  
Default value: "#444"
