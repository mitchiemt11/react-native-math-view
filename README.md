# react-native-math-view

| Launch Test | Example App |
| --- | --- |
| ![Launch](./docs/launchAndroid.gif) | ![Example App](./docs/exampleAndroid.gif) |


## WIP V3

A react native view used to easily display and handle math.

## Installation

`npm install --save react-native-math-view`

**OR**

`yarn add react-native-math-view`


## Getting Started

```

### Rendering `MathView`
```js
import MathView, { MathProvider } from 'react-native-math-view';

render() {
  return (
    ...
    	<MathView
		resizeMode='stretch'
		math='x=\\frac{-b\\pm\\sqrt{b^2-4ac}}{2a}'
	/> 
	<MathView
		scaleToFit
		math='\\cos\\left(x\\right)=\\frac{b}{c}'
	/> 
    ...
  );
}


```


## Running example app
from the project's directory run:
```
cd MathExample
yarn --production=false
npx react-native run-android
```

## Implementation:
  - [ ] [iOS native MathView](https://github.com/kostub/iosMath) - linked native! Need to create RN component

  - [x] Android MathView - **native since V2**, based on [Android SVGImageView](https://bigbadaboom.github.io/androidsvg). Need to implement `editable` state.

### FollowUp

[KaTeX](https://github.com/Khan/KaTeX) - Math keypad that works with `<WebView>`. See [this](https://github.com/ShaMan123/math-input)

[React with LaTeX](https://github.com/Pomax/BezierInfo-2) - using server side rendering to speed things up.

[Writing math dynamically](https://github.com/nicolewhite/algebra.js)

