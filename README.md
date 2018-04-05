# Scaled-Image-React-Native
## How To Use

 1. Import ScaledImage to your code
`import ScaledImage from 'ScaledImage';`
2. To using you can following this example
```
import React, { Component } from 'react';
import {
  AppRegistry,
  Dimensions,
  StyleSheet,
  Text,
  View
} from 'react-native';
import ScaledImage from 'ScaledImage';

const width = Dimensions.get('window').width;

export default class SomeApps extends Component {
  render() {
    return (
      <View>
        <ScaledImage uri={source('img/image.png')} width={width} />
      </View>
      <View style={styles.container}>
        <Text style={styles.welcome}>
          Welcome to React Native!
        </Text>
        <Text style={styles.instructions}>
          To get started, edit index.ios.js
        </Text>
        <Text style={styles.instructions}>
          Press Cmd+R to reload,{'\n'}
          Cmd+D or shake for dev menu
        </Text>
      </View>
    );
  }
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    justifyContent: 'center',
    alignItems: 'center',
    backgroundColor: '#F5FCFF',
  },
  welcome: {
    fontSize: 20,
    textAlign: 'center',
    margin: 10,
  },
  instructions: {
    textAlign: 'center',
    color: '#333333',
    marginBottom: 5,
  },
});

AppRegistry.registerComponent('SomeApps', () => SomeApps);
```

3. Refence
