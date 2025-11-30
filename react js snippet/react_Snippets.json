{
  // ==================== REACT COMPONENTS ====================
  "React Functional Component": {
    "prefix": "rfc",
    "body": [
      "import React from 'react';",
      "",
      "const ${1:ComponentName} = () => {",
      "  return (",
      "    <div>",
      "      $0",
      "    </div>",
      "  );",
      "};",
      "",
      "export default ${1:ComponentName};"
    ],
    "description": "Create a React functional component"
  },
  "React Functional Component with Props": {
    "prefix": "rfcp",
    "body": [
      "import React from 'react';",
      "",
      "interface ${1:ComponentName}Props {",
      "  $2",
      "}",
      "",
      "const ${1:ComponentName}: React.FC<${1:ComponentName}Props> = ({ $3 }) => {",
      "  return (",
      "    <div>",
      "      $0",
      "    </div>",
      "  );",
      "};",
      "",
      "export default ${1:ComponentName};"
    ],
    "description": "React functional component with TypeScript props"
  },
  "React Native Functional Component": {
    "prefix": "rnfc",
    "body": [
      "import React from 'react';",
      "import { View, Text, StyleSheet } from 'react-native';",
      "",
      "const ${1:ComponentName} = () => {",
      "  return (",
      "    <View style={styles.container}>",
      "      <Text>$0</Text>",
      "    </View>",
      "  );",
      "};",
      "",
      "const styles = StyleSheet.create({",
      "  container: {",
      "    flex: 1,",
      "  },",
      "});",
      "",
      "export default ${1:ComponentName};"
    ],
    "description": "React Native functional component with styles"
  },

  // ==================== HOOKS ====================
  "useState Hook": {
    "prefix": "ush",
    "body": [
      "const [${1:state}, set${1/(.*)/${1:/capitalize}/}] = useState${2:<${3:type}>}(${4:initialValue});"
    ],
    "description": "React useState hook"
  },
  "useEffect Hook": {
    "prefix": "ueh",
    "body": [
      "useEffect(() => {",
      "  $0",
      "}, [${1:dependencies}]);"
    ],
    "description": "React useEffect hook"
  },
  "useEffect with Cleanup": {
    "prefix": "uehc",
    "body": [
      "useEffect(() => {",
      "  $0",
      "  ",
      "  return () => {",
      "    // Cleanup",
      "    $1",
      "  };",
      "}, [${2:dependencies}]);"
    ],
    "description": "useEffect with cleanup function"
  },
  "useRef Hook": {
    "prefix": "urh",
    "body": [
      "const ${1:ref} = useRef${2:<${3:type}>}(${4:null});"
    ],
    "description": "React useRef hook"
  },
  "useMemo Hook": {
    "prefix": "umh",
    "body": [
      "const ${1:memoizedValue} = useMemo(() => {",
      "  return $0;",
      "}, [${2:dependencies}]);"
    ],
    "description": "React useMemo hook"
  },
  "useCallback Hook": {
    "prefix": "uch",
    "body": [
      "const ${1:memoizedCallback} = useCallback(",
      "  (${2:params}) => {",
      "    $0",
      "  },",
      "  [${3:dependencies}]",
      ");"
    ],
    "description": "React useCallback hook"
  },
  "useContext Hook": {
    "prefix": "uctx",
    "body": [
      "const ${1:value} = useContext(${2:Context});"
    ],
    "description": "React useContext hook"
  },
  "useReducer Hook": {
    "prefix": "urdh",
    "body": [
      "const [${1:state}, ${2:dispatch}] = useReducer(${3:reducer}, ${4:initialState});"
    ],
    "description": "React useReducer hook"
  },

  // ==================== CUSTOM HOOKS ====================
  "Custom Hook Template": {
    "prefix": "usehook",
    "body": [
      "import { useState, useEffect } from 'react';",
      "",
      "const use${1:HookName} = (${2:params}) => {",
      "  const [${3:state}, set${3/(.*)/${1:/capitalize}/}] = useState(${4:initialValue});",
      "",
      "  useEffect(() => {",
      "    $0",
      "  }, [${5:dependencies}]);",
      "",
      "  return ${3:state};",
      "};",
      "",
      "export default use${1:HookName};"
    ],
    "description": "Custom React hook template"
  },

  // ==================== CONSOLE LOGS ====================
  "Console Log": {
    "prefix": "clg",
    "body": [
      "console.log('$1', $1);"
    ],
    "description": "Console log with label"
  },
  "Console Log Object": {
    "prefix": "clo",
    "body": [
      "console.log('$1:', JSON.stringify($1, null, 2));"
    ],
    "description": "Console log object with JSON.stringify"
  },
  "Console Error": {
    "prefix": "cer",
    "body": [
      "console.error('$1', $1);"
    ],
    "description": "Console error"
  },
  "Console Warn": {
    "prefix": "cwr",
    "body": [
      "console.warn('$1', $1);"
    ],
    "description": "Console warning"
  },
  "Console Table": {
    "prefix": "ctb",
    "body": [
      "console.table($1);"
    ],
    "description": "Console table for arrays/objects"
  },
  "Console Group": {
    "prefix": "cgr",
    "body": [
      "console.group('$1');",
      "$0",
      "console.groupEnd();"
    ],
    "description": "Console group for organized logs"
  },
  "Console Time": {
    "prefix": "ctm",
    "body": [
      "console.time('${1:label}');",
      "$0",
      "console.timeEnd('${1:label}');"
    ],
    "description": "Console time for performance tracking"
  },

  // ==================== ASYNC/AWAIT ====================
  "Async Function": {
    "prefix": "asf",
    "body": [
      "const ${1:functionName} = async (${2:params}) => {",
      "  try {",
      "    $0",
      "  } catch (error) {",
      "    console.error('Error in ${1:functionName}:', error);",
      "  }",
      "};"
    ],
    "description": "Async arrow function with try-catch"
  },
  "Fetch API": {
    "prefix": "fet",
    "body": [
      "const ${1:fetchData} = async () => {",
      "  try {",
      "    const response = await fetch('${2:url}');",
      "    const data = await response.json();",
      "    $0",
      "  } catch (error) {",
      "    console.error('Fetch error:', error);",
      "  }",
      "};"
    ],
    "description": "Fetch API with async/await"
  },
  "Axios GET": {
    "prefix": "axg",
    "body": [
      "const ${1:fetchData} = async () => {",
      "  try {",
      "    const { data } = await axios.get('${2:url}');",
      "    $0",
      "  } catch (error) {",
      "    console.error('Axios error:', error);",
      "  }",
      "};"
    ],
    "description": "Axios GET request"
  },
  "Axios POST": {
    "prefix": "axp",
    "body": [
      "const ${1:postData} = async () => {",
      "  try {",
      "    const { data } = await axios.post('${2:url}', {",
      "      $3",
      "    });",
      "    $0",
      "  } catch (error) {",
      "    console.error('Axios error:', error);",
      "  }",
      "};"
    ],
    "description": "Axios POST request"
  },

  // ==================== EVENT HANDLERS ====================
  "onClick Handler": {
    "prefix": "onc",
    "body": [
      "const handle${1:Click} = (${2:e}) => {",
      "  $0",
      "};"
    ],
    "description": "onClick event handler"
  },
  "onChange Handler": {
    "prefix": "onch",
    "body": [
      "const handle${1:Change} = (${2:e}) => {",
      "  const { value } = ${2:e}.target;",
      "  $0",
      "};"
    ],
    "description": "onChange event handler"
  },
  "onSubmit Handler": {
    "prefix": "ons",
    "body": [
      "const handle${1:Submit} = (${2:e}) => {",
      "  ${2:e}.preventDefault();",
      "  $0",
      "};"
    ],
    "description": "onSubmit event handler with preventDefault"
  },

  // ==================== REACT NATIVE SPECIFIC ====================
  "React Native StyleSheet": {
    "prefix": "rnss",
    "body": [
      "const styles = StyleSheet.create({",
      "  ${1:container}: {",
      "    $0",
      "  },",
      "});"
    ],
    "description": "React Native StyleSheet"
  },
  "React Native FlatList": {
    "prefix": "rnfl",
    "body": [
      "<FlatList",
      "  data={${1:data}}",
      "  keyExtractor={(item) => item.${2:id}}",
      "  renderItem={({ item }) => (",
      "    $0",
      "  )}",
      "/>"
    ],
    "description": "React Native FlatList component"
  },
  "React Native TouchableOpacity": {
    "prefix": "rnto",
    "body": [
      "<TouchableOpacity onPress={${1:handlePress}}>",
      "  $0",
      "</TouchableOpacity>"
    ],
    "description": "React Native TouchableOpacity"
  },
  "React Native TextInput": {
    "prefix": "rnti",
    "body": [
      "<TextInput",
      "  value={${1:value}}",
      "  onChangeText={${2:setValue}}",
      "  placeholder=\"${3:Enter text}\"",
      "  style={styles.${4:input}}",
      "/>"
    ],
    "description": "React Native TextInput"
  },

  // ==================== TYPESCRIPT ====================
  "TypeScript Interface": {
    "prefix": "tsi",
    "body": [
      "interface ${1:InterfaceName} {",
      "  ${2:property}: ${3:type};",
      "  $0",
      "}"
    ],
    "description": "TypeScript interface"
  },
  "TypeScript Type": {
    "prefix": "tst",
    "body": [
      "type ${1:TypeName} = {",
      "  ${2:property}: ${3:type};",
      "  $0",
      "};"
    ],
    "description": "TypeScript type"
  },
  "TypeScript Enum": {
    "prefix": "tse",
    "body": [
      "enum ${1:EnumName} {",
      "  ${2:VALUE} = '${3:value}',",
      "  $0",
      "}"
    ],
    "description": "TypeScript enum"
  },

  // ==================== IMPORTS ====================
  "Import React": {
    "prefix": "imr",
    "body": [
      "import React from 'react';"
    ],
    "description": "Import React"
  },
  "Import React with Hooks": {
    "prefix": "imrh",
    "body": [
      "import React, { ${1:useState, useEffect} } from 'react';"
    ],
    "description": "Import React with hooks"
  },
  "Import React Native": {
    "prefix": "imrn",
    "body": [
      "import { ${1:View, Text, StyleSheet} } from 'react-native';"
    ],
    "description": "Import React Native components"
  },
  "Import Styled Components": {
    "prefix": "imsc",
    "body": [
      "import styled from 'styled-components${1:/native}';"
    ],
    "description": "Import styled-components"
  },

  // ==================== NAVIGATION (React Native) ====================
  "React Navigation useNavigation": {
    "prefix": "rnun",
    "body": [
      "const navigation = useNavigation();"
    ],
    "description": "React Navigation useNavigation hook"
  },
  "React Navigation Navigate": {
    "prefix": "rnnav",
    "body": [
      "navigation.navigate('${1:ScreenName}', { ${2:params} });"
    ],
    "description": "Navigate to screen"
  },

  // ==================== UTILITIES ====================
  "Try Catch Block": {
    "prefix": "tryc",
    "body": [
      "try {",
      "  $0",
      "} catch (error) {",
      "  console.error('Error:', error);",
      "}"
    ],
    "description": "Try-catch block"
  },
  "Arrow Function": {
    "prefix": "af",
    "body": [
      "const ${1:functionName} = (${2:params}) => {",
      "  $0",
      "};"
    ],
    "description": "Arrow function"
  },
  "Destructure Props": {
    "prefix": "dpr",
    "body": [
      "const { ${1:props} } = ${2:object};"
    ],
    "description": "Destructure object"
  },
  "Ternary Operator": {
    "prefix": "ter",
    "body": [
      "${1:condition} ? ${2:true} : ${3:false}"
    ],
    "description": "Ternary operator"
  },
  "Promise": {
    "prefix": "prom",
    "body": [
      "new Promise((resolve, reject) => {",
      "  $0",
      "})"
    ],
    "description": "Promise constructor"
  },
  "setTimeout": {
    "prefix": "sto",
    "body": [
      "setTimeout(() => {",
      "  $0",
      "}, ${1:1000});"
    ],
    "description": "setTimeout"
  },
  "setInterval": {
    "prefix": "sin",
    "body": [
      "const ${1:intervalId} = setInterval(() => {",
      "  $0",
      "}, ${2:1000});"
    ],
    "description": "setInterval"
  }
}
