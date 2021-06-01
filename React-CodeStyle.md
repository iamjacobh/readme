# React Coding Style Standard

## 1. Import

Use `'` for package name or component name. And put semicolon at the end of the line.
```javascript
import React, { useEffect, useState } from 'react';
```

Break a line between open source packages and user-defined component. And break a line when define a class/functional component.
```javascript
import React from 'react';
import { View } from 'react-native';
import { StackNavigator } from 'react-navigation';

import Styles from './styles';

const HomeScreen = () => {
}
```

## 2. Define Component

Tab size is 2 spaces and all functions are arrow function. Break a line between variables and function. And break a line between functions as well. 
```javascript
const HomeScreen = () => {
  const [value, setValue] = useState(0);
  const [name, setName] = useState("Jacob");

  useEffect(() => {
    setValue(1);
  }, []);

  changeName = (newName) => {
    setName(newName);
  }

  return ();
}
```

## 3. Virtual DOM

If a component doesn't have any props, write it in a line. Put a space before ending mark.
```javascript
  return (
    <View />
  );
```

If a component has only 1 props, write it in a line as well. Put a space before ending mark.
```javascript
  return (
    <View style={styles.container} />
  );
```

If a component has more than 2 props, write props in next lines.
```javascript
  return (
    <Button
      style={styles.button}
      color={'#007AFF'}
      title="Button"
      onPress={() => {}}
    />
  );
```

If consition statement is needed to put between tags, write as following.
```javascript
  return (
    <View>
      {
        condition == true ?
          <View />
          :
          <View />
      }
    </View>
  );
```