# jest-tutorial
for learning jest configuration

How to overcome this error

 import {
    ^^^^^^

    SyntaxError: Cannot use import statement outside a module

Fix: 
https://stackoverflow.com/questions/66959585/how-to-configure-jest-to-transform-modules-containing-invalid-syntax

Add to jest config the following:
```

 "transform": {
      "^.+\\.ts?$": "ts-jest",
      "^.+\\.tsx?$": "ts-jest",
      "^.+\\.js$": "<rootDir>/node_modules/react-native/jest/preprocessor.js"
    }
```

    
   
