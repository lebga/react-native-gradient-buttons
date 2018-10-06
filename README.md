# React Native Gradient Buttons

A lightweight, customizable and haptic Gradient Button library for React Native.

<img src="./Examples.png" alt="Examples" width="250">

## Requirements
Requires React, React Native, and Expo.

## Installation

```
yarn add react-native-gradient-buttons
# or
npm install --save react-native-gradient-buttons
```

## Usage

```
# ES6 import
import GradientButton from 'react-native-gradient-buttons';
```

## Props
  - `text`: `String`
    - No default
    - options: any string
  - `gradientBegin`: `String` 
    - default: `'#00d2ff'`
    - options: Any hex, rgb, or color    
  - `gradientEnd`: `String`
    - default: `'#3a47d5'`
    - options: Any hex, rgb, or color
  - `gradientDirection`: `String`
    - default: `'horizontal'`
    - options: `'horizontal'`, `'vertical'`, `'diagonal'`
  - `height`: `Number` or `String` (for %)
    - default: `75`
    - options: any number
  - `width`: `Number` or `String` (for %)
    - No default
    - options: any number
  - `radius`: `Number`
    - default: `50`
    - options: any number
  - `impact`: `Boolean`
    - default: `false`
    - options: `true` or `false`
  - `impactStyle`: `String`
    - default: `'Heavy'`
    - options: `'Heavy'`, `'Medium'`, `'Light'`
  - `onPressAction`: `Function`
    - No default
    - options: any function you want to pass to the Gradient Button

  **Design+Code Specifc Gradient Props**
  - purpleViolet
  - violetPink
  - pinkDarkGreen
  - blueViolet
  - blueMarine
  - deepBlue

## Examples

```
  <View style={{flex: 1, justifyContent: 'space-evenly', alignItems: 'center', marginVertical: 24}}>
    <GradientButton
      text="Gradient Button"
      gradientBegin="#874f00"
      gradientEnd="#f5ba57"
      gradientDirection="diagonal"
      height={60}
      width={300}
      radius={15}
      impact
      impactStyle='Light'
      onPressAction={() => alert('You pressed me!')}
    />

    <GradientButton text="Purple Violet" width='90%' purpleViolet impact />
    <GradientButton text="Violet Pink" width='90%' violetPink impact />
    <GradientButton text="Pink Dark Green" width='90%' pinkDarkGreen impact />
    <GradientButton text="Blue Violet" width='90%' blueViolet impact />
    <GradientButton text="Blue Marine" width='90%' blueMarine impact />
    <GradientButton text="Deep Blue" width='90%' deepBlue impact />
  </View>
```