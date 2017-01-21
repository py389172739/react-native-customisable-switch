# react-native-customisable-switch
A React Native module that allows you to customize switch (style, form and animation), availble for android and IOS.

### Content
- [Installation](#installation)
- [Examples](#usage-example)
- [Properties](#properties)
- [Questions](#questions)

### Installation
```bash
npm install react-native-customisable-switch

### Examples
<p align="center">
    <img src ="./examples.gif" />
</p>
```javascript
import React, { Component } from 'react';
import {
  Text,
  View,
} from 'react-native';
import Switch from 'react-native-customisable-switch';

export default class Test extends Component {
  constructor(props) {
    super(props);
  }

  render() {
    return(
      <View style={styles.container}>
        <View style={styles.container}>
          <Switch />
        </View>
        <View style={styles.container}>
          <Switch
            defaultValue={true}
            activeText={''}
            inactiveText={''}
            fontSize={16}
            activeTextColor={'rgba(255, 255, 255, 1)'}
            inactiveTextColor={'rgba(255, 255, 255, 1)'}
            activeBackgroundColor={'rgba(50, 163, 50, 1)'}
            inactiveBackgroundColor={'rgba(137, 137, 137, 1)'}
            activeButtonBackgroundColor={'rgba(255, 255, 255, 1)'}
            inactiveButtonBackgroundColor={'rgba(255, 255, 255, 1)'}
            switchWidth={70}
            switchHeight={30}
            switchBorderRadius={0}
            switchBorderColor={'rgba(0, 0, 0, 1)'}
            switchBorderWidth={0}
            buttonWidth={25}
            buttonHeight={25}
            buttonBorderRadius={0}
            buttonBorderColor={'rgba(0, 0, 0, 1)'}
            buttonBorderWidth={0}
            animationTime={150}
            padding={true}
            onChangeValue={(value) => {
              console.log(value);
            }}
          />
        </View>  
        <View style={styles.container}>
          <Switch 
            defaultValue={false}
            activeText={'On'}
            inactiveText={'Off'}
            fontSize={16}
            switchWidth={70}
            switchHeight={25}
            switchBorderRadius={12}
            switchBorderWidth={0}
            buttonWidth={25}
            buttonHeight={40}
            buttonBorderRadius={20}
            buttonBorderColor={'rgba(0, 0, 0, 1)'}
            buttonBorderWidth={0}
            animationTime={150}
            padding={true}
            onChangeValue={(value) => {
              console.log(value);
            }}
          />
        </View>
      </View>
    )
  }
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#464857',
    justifyContent: 'center',
    alignItems: 'center',
  },
)};
```
### Properties
**defaultValue** (Boolean): false //Default switch value
**onChangeValue** (Function): () => null //Sends the current value of switch
**activeText** (String): "On" //Text when switch is activated
**inactiveText** (String): "Off" //Text when switch is inactivated
**fontSize** (Number): 16 //Size of text
**activeTextColor** (String): "rgba(255, 255, 255, 1)" //Color of activated switch text
**inactiveTextColor** (String): "rgba(255, 255, 255, 1)" //Color of inactivated switch text
**activeBackgroundColor** (String): "rgba(50, 163, 50, 1)" //Background color of activated switch
**inactiveBackgroundColor** (String): "rgba(137, 137, 137, 1)" //Background color of inactivated switch
**activeButtonBackgroundColor** (String): "rgba(255, 255, 255, 1)"  //Color of activated switch button
**inactiveButtonBackgroundColor** (String): "rgba(255, 255, 255, 1)"  //Color of inactivated switch button
**switchWidth** (Number): 70 // Switch width
**switchHeight** (Number): 30 // Switch height
**switchBorderRadius** (Number): 15 // Switch border radius 
**switchBorderColor** (String): 'rgba(0, 0, 0, 1)' // Switch border color 
**switchBorderWidth** (Number): 0 //Switch border width 
**buttonWidth** (Number): 25 //Switch button width
**buttonHeight** (Number): 25 //Switch button height
**buttonBorderRadius** (Number): 15 // Switch button border radius
**buttonBorderColor** (String): 'rgba(0, 0, 0, 1)' // Switch button border color
**buttonBorderWidth** (Number): 0 //Switch button border width
**animationTime** (Number): 150 // Animation duration
**padding** (Boolean): true // Switch horizontal padding

### Questions
Create an issue (https://github.com/baderahmed/react-native-customisable-switch/issues)