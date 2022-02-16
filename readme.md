
# React Native Scroll Up

React native scroll up container is a react native component with scroll up animation, you will see an example below.

![Default](https://media.giphy.com/media/3SsAp23SFICXT3vSJP/giphy.gif)

![With Children](https://media.giphy.com/media/etEWUFiDDMPV1eqA1s/giphy.gif)


## Installation

Before you install this package, this package requires react-native-gesture-handler and react-native-reanimated packages.

```bash
  npm i react-native-gesture-handler react-native-reanimated
```
After that you can install this package.

```bash
  npm i react-native-scroll-up-container
```
## Usage/Examples

```javascript
import React from 'react'
import { View } from 'react-native'
import SwipeContainer from 'react-native-scroll-up-container'

function App() {
  return <SwipeContainer 
    useLine
    containerStyle={{
      flex:1
    }}
    translateY={300}
    overValue={50}
    topComponent={
      <View style={{
        flex:1,
        backgroundColor:'blue'
      }}>
      </View>
    }
    limitTopValue={50}
    limitBottomValue={250}
  >
    <View style={{
      height:800,
      width:'100%',
      backgroundColor:'red
    }}>
    </View>
  </SwipeContainer>
}
```


## Props

| Prop | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `useLine` | `Boolean` | **Optional, Default: True**. Use default line for bottom component  |
| `containerStyle` | `Object` | **Optional**. For customize container style  |
| `translateY` | `Number` | **Optional, Default: 300**. Position translateY of bottom component  |
| `overValue` | `Number` | **Optional, Default: 50**. Over height value for top component  |
| `limitTopValue` | `Number` | **Optional, Default: 50**. Limit top value for animate spring |
| `limitBottomValue` | `Number` | **Optional,  Default: 250**. Limit bottom value for animate spring |
| `topComponent` | `Component` | For customize top component of container  |
| `children` | `Component` | For customize children of container  |

## Contributing
- Fork it ( https://github.com/jfalih/react-native-scroll-up-container/fork )
- Create your feature branch (`git checkout -b my-new-feature`)
- Commit your changes (`git commit -am 'Add some feature'`)
- Push to the branch (`git push origin my-new-feature`)
- Create a new Pull Request


## License

[MIT](https://choosealicense.com/licenses/mit/)


## Authors

- [@jfalih](https://www.github.com/jfalih)

