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

Tab size is 2 Spaces and all functions are arrow function.
```javascript
const HomeScreen = () => {
  const [value, setValue] = useState(0);
}
```
