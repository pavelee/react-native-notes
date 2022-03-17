# My notes about react-native

-   [Style sheet](#style-sheet)
-   [Layout system](#layout-system)

## Style sheet

-   To style elements we use StyleSheet from react-native
-   Just import StyleSheet and define your styles
```
import { StyleSheet } from 'react-native'

const styles = StyleSheet.create({
    myclass: {
        borderWidth: 1,
        borderColor: 'red'
    }
});
```
-   Use your style with components
```
<View style={styles.myclass}></View>
```

## Layout system

-   Layout system purpose is to take control of element's position
    -   make our app looks nice
-   We want to be able to recreate mockups from designer

### Three ways

![layout_system](https://raw.githubusercontent.com/pavelee/react-native-notes/main/assets/layout_system.png)

### Box Object Model
-   ![layout_system](https://raw.githubusercontent.com/pavelee/react-native-notes/main/assets/box_object_model.png)
-   box system familiar to web development
-   padding, margin, border
    -   margin
        -   margin - all sides
        -   marginVertical - margin top and bottom
        -   marginHorizontal - margin left and right
        -   marginTop
        -   marginBottom
        -   marginLeft
        -   marginRight
    -   padding
        -   padding - all sides
        -   paddingVertical - padding top and bottom
        -   paddingHorizontal - padding left and right
        -   paddingTop
        -   paddingBottom
        -   paddingLeft
        -   paddingRight
    -   border
        -   borderWidth - all sides
        -   borderTopWidth
        -   borderBottomWidth
        -   borderLeftWidth
        -   borderRightWidth
-   width, height of element
-   using when you want to position single element by itself
### Flex Box
-   familiar to flex system from web development
-   how we layout some number of child element that are all in the same parent element
    -   layout multiple element with one common parent
-   options
    -   alignitems
        -   ![layout_system](https://raw.githubusercontent.com/pavelee/react-native-notes/main/assets/flex_box_alignitems.png)
        -   stretch (default)
            -   use maximum space to stretch child elements
            -   default behaviour for flex box parent
        -   flex-start
            -   put child elements on the begining of parent element and use minimum space possible
        -   center
            -   put child elements on the center of parent element and use minimum space
        -   flex-end
            -   put child elements on the end of parent element and use minimum space
### Position
-   position single element in a parent element
    -   override box object model and flex blox
    -   similar to position absolute from web development

