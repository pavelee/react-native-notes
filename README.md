# My notes about react-native

-   [Style sheet](#style-sheet)
-   [Layout system](#layout-system)

## Style sheet

-   To style elements we use StyleSheet from react-native
```
import { StyleSheet } from 'react-native'

const styles = StyleSheet.create({});
```

## Layout system

-   Layout system purpose is to take control of element's position
    -   make our app looks nice
-   We want to be able to recreate mockups from designer

### Three ways

![layout_system](https://raw.githubusercontent.com/pavelee/react-native-notes/main/assets/layout_system.png)

-   Box Object Model
    -   familiar for web developer
        -   padding, margin, border
        -   width, height of element
    -   using when you want to position single element by itself
-   Flex Box
    -   familiar for web developer
    -   how we layout some number of child element that are all in the same parent element
        -   layout multiple element with one common parent
-   Position
    -   position single element in a parent element
        -   override box object model and flex blox
        -   similar to position absolute from web development

