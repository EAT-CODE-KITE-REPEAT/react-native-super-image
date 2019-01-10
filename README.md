# reac-native-super-image
React Native Super Image: Image component with optional additional cool stuff

* animation loading
* downloading and caching image in the background
* showing default background color before loading
* option to resize to 100% height or width, keeping image ratio

## Install
`yarn add react-native-super-image`

```js
import RNSuperImage from "react-native-super-image";
import expo from "expo";
const SuperImage = props => RNSuperImage({ ...props, expo });
```

Props:

* expo (required): The expo class
* animated (optional): boolean. if set to true, the image fades in for 100ms once it's loaded
* source (required): see [react native image](https://facebook.github.io/react-native/docs/image)
* style (optional): see [react native image](https://facebook.github.io/react-native/docs/image)
* width (optional): number or "auto". overwrites style-width. If set to auto, it calculates the width based on height and image ratio
* heigh (optional)t: number or "auto". overwrites style-height. If set to auto, it calculates the height based on width and image ratio
