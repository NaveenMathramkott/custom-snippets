{
  // ==================== FUNCTIONS ====================
  "Arrow Function": {
    "prefix": "af",
    "body": [
      "const ${1:functionName} = (${2:params}) => {",
      "  $0",
      "};"
    ],
    "description": "Arrow function"
  },
  "Arrow Function Implicit Return": {
    "prefix": "afi",
    "body": [
      "const ${1:functionName} = (${2:params}) => $0;"
    ],
    "description": "Arrow function with implicit return"
  },
  "Async Arrow Function": {
    "prefix": "aaf",
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
  "Named Function": {
    "prefix": "fn",
    "body": [
      "function ${1:functionName}(${2:params}) {",
      "  $0",
      "}"
    ],
    "description": "Named function"
  },
  "Async Function": {
    "prefix": "afn",
    "body": [
      "async function ${1:functionName}(${2:params}) {",
      "  try {",
      "    $0",
      "  } catch (error) {",
      "    console.error('Error:', error);",
      "  }",
      "}"
    ],
    "description": "Async function with try-catch"
  },
  "IIFE": {
    "prefix": "iife",
    "body": [
      "(function() {",
      "  $0",
      "})();"
    ],
    "description": "Immediately Invoked Function Expression"
  },
  "Async IIFE": {
    "prefix": "aiife",
    "body": [
      "(async () => {",
      "  try {",
      "    $0",
      "  } catch (error) {",
      "    console.error('Error:', error);",
      "  }",
      "})();"
    ],
    "description": "Async IIFE"
  },

  // ==================== ARRAY METHODS ====================
  "forEach": {
    "prefix": "fe",
    "body": [
      "${1:array}.forEach((${2:item}) => {",
      "  $0",
      "});"
    ],
    "description": "forEach loop"
  },
  "map": {
    "prefix": "map",
    "body": [
      "const ${1:result} = ${2:array}.map((${3:item}) => {",
      "  return $0;",
      "});"
    ],
    "description": "Array map"
  },
  "filter": {
    "prefix": "filter",
    "body": [
      "const ${1:filtered} = ${2:array}.filter((${3:item}) => {",
      "  return $0;",
      "});"
    ],
    "description": "Array filter"
  },
  "reduce": {
    "prefix": "reduce",
    "body": [
      "const ${1:result} = ${2:array}.reduce((${3:acc}, ${4:item}) => {",
      "  $0",
      "  return ${3:acc};",
      "}, ${5:initialValue});"
    ],
    "description": "Array reduce"
  },
  "find": {
    "prefix": "find",
    "body": [
      "const ${1:found} = ${2:array}.find((${3:item}) => ${3:item}.${4:property} === ${5:value});"
    ],
    "description": "Array find"
  },
  "findIndex": {
    "prefix": "findi",
    "body": [
      "const ${1:index} = ${2:array}.findIndex((${3:item}) => ${3:item}.${4:property} === ${5:value});"
    ],
    "description": "Array findIndex"
  },
  "some": {
    "prefix": "some",
    "body": [
      "const ${1:hasMatch} = ${2:array}.some((${3:item}) => ${3:item}.${4:property} === ${5:value});"
    ],
    "description": "Array some"
  },
  "every": {
    "prefix": "every",
    "body": [
      "const ${1:allMatch} = ${2:array}.every((${3:item}) => ${3:item}.${4:property} === ${5:value});"
    ],
    "description": "Array every"
  },
  "sort": {
    "prefix": "sort",
    "body": [
      "${1:array}.sort((a, b) => ${2:a.property - b.property});"
    ],
    "description": "Array sort"
  },

  // ==================== OBJECT METHODS ====================
  "Object.keys": {
    "prefix": "ok",
    "body": [
      "Object.keys(${1:object}).forEach((${2:key}) => {",
      "  $0",
      "});"
    ],
    "description": "Object.keys with forEach"
  },
  "Object.values": {
    "prefix": "ov",
    "body": [
      "Object.values(${1:object}).forEach((${2:value}) => {",
      "  $0",
      "});"
    ],
    "description": "Object.values with forEach"
  },
  "Object.entries": {
    "prefix": "oe",
    "body": [
      "Object.entries(${1:object}).forEach(([${2:key}, ${3:value}]) => {",
      "  $0",
      "});"
    ],
    "description": "Object.entries with forEach"
  },
  "Object.assign": {
    "prefix": "oas",
    "body": [
      "const ${1:newObj} = Object.assign({}, ${2:obj1}, ${3:obj2});"
    ],
    "description": "Object.assign"
  },
  "Object Destructuring": {
    "prefix": "dob",
    "body": [
      "const { ${1:property} } = ${2:object};"
    ],
    "description": "Object destructuring"
  },
  "Array Destructuring": {
    "prefix": "dar",
    "body": [
      "const [${1:first}, ${2:second}] = ${3:array};"
    ],
    "description": "Array destructuring"
  },

  // ==================== PROMISES & ASYNC ====================
  "Promise": {
    "prefix": "prom",
    "body": [
      "new Promise((resolve, reject) => {",
      "  $0",
      "});"
    ],
    "description": "Promise constructor"
  },
  "Promise.then": {
    "prefix": "pthen",
    "body": [
      "${1:promise}",
      "  .then((${2:result}) => {",
      "    $0",
      "  })",
      "  .catch((${3:error}) => {",
      "    console.error('Error:', ${3:error});",
      "  });"
    ],
    "description": "Promise.then with catch"
  },
  "Promise.all": {
    "prefix": "pall",
    "body": [
      "Promise.all([${1:promises}])",
      "  .then((${2:results}) => {",
      "    $0",
      "  })",
      "  .catch((${3:error}) => {",
      "    console.error('Error:', ${3:error});",
      "  });"
    ],
    "description": "Promise.all"
  },
  "Promise.race": {
    "prefix": "prace",
    "body": [
      "Promise.race([${1:promises}])",
      "  .then((${2:result}) => {",
      "    $0",
      "  })",
      "  .catch((${3:error}) => {",
      "    console.error('Error:', ${3:error});",
      "  });"
    ],
    "description": "Promise.race"
  },
  "Promise.allSettled": {
    "prefix": "psettled",
    "body": [
      "Promise.allSettled([${1:promises}])",
      "  .then((${2:results}) => {",
      "    $0",
      "  });"
    ],
    "description": "Promise.allSettled"
  },
  "Async Await": {
    "prefix": "awa",
    "body": [
      "try {",
      "  const ${1:result} = await ${2:asyncFunction}();",
      "  $0",
      "} catch (error) {",
      "  console.error('Error:', error);",
      "}"
    ],
    "description": "Async await with try-catch"
  },

  // ==================== FETCH & AXIOS ====================
  "Fetch GET": {
    "prefix": "fetg",
    "body": [
      "fetch('${1:url}')",
      "  .then(response => response.json())",
      "  .then(data => {",
      "    $0",
      "  })",
      "  .catch(error => {",
      "    console.error('Fetch error:', error);",
      "  });"
    ],
    "description": "Fetch GET request"
  },
  "Fetch POST": {
    "prefix": "fetp",
    "body": [
      "fetch('${1:url}', {",
      "  method: 'POST',",
      "  headers: {",
      "    'Content-Type': 'application/json',",
      "  },",
      "  body: JSON.stringify({",
      "    $2",
      "  }),",
      "})",
      "  .then(response => response.json())",
      "  .then(data => {",
      "    $0",
      "  })",
      "  .catch(error => {",
      "    console.error('Fetch error:', error);",
      "  });"
    ],
    "description": "Fetch POST request"
  },
  "Async Fetch": {
    "prefix": "afet",
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
    "description": "Async fetch function"
  },
  "Axios GET": {
    "prefix": "axg",
    "body": [
      "axios.get('${1:url}')",
      "  .then(response => {",
      "    const { data } = response;",
      "    $0",
      "  })",
      "  .catch(error => {",
      "    console.error('Axios error:', error);",
      "  });"
    ],
    "description": "Axios GET request"
  },
  "Axios POST": {
    "prefix": "axp",
    "body": [
      "axios.post('${1:url}', {",
      "  $2",
      "})",
      "  .then(response => {",
      "    const { data } = response;",
      "    $0",
      "  })",
      "  .catch(error => {",
      "    console.error('Axios error:', error);",
      "  });"
    ],
    "description": "Axios POST request"
  },

  // ==================== DOM MANIPULATION ====================
  "querySelector": {
    "prefix": "qs",
    "body": [
      "const ${1:element} = document.querySelector('${2:selector}');"
    ],
    "description": "querySelector"
  },
  "querySelectorAll": {
    "prefix": "qsa",
    "body": [
      "const ${1:elements} = document.querySelectorAll('${2:selector}');"
    ],
    "description": "querySelectorAll"
  },
  "getElementById": {
    "prefix": "gid",
    "body": [
      "const ${1:element} = document.getElementById('${2:id}');"
    ],
    "description": "getElementById"
  },
  "addEventListener": {
    "prefix": "ael",
    "body": [
      "${1:element}.addEventListener('${2:event}', (${3:e}) => {",
      "  $0",
      "});"
    ],
    "description": "addEventListener"
  },
  "removeEventListener": {
    "prefix": "rel",
    "body": [
      "${1:element}.removeEventListener('${2:event}', ${3:handler});"
    ],
    "description": "removeEventListener"
  },
  "createElement": {
    "prefix": "ce",
    "body": [
      "const ${1:element} = document.createElement('${2:div}');"
    ],
    "description": "createElement"
  },
  "classList.add": {
    "prefix": "cla",
    "body": [
      "${1:element}.classList.add('${2:className}');"
    ],
    "description": "classList.add"
  },
  "classList.remove": {
    "prefix": "clr",
    "body": [
      "${1:element}.classList.remove('${2:className}');"
    ],
    "description": "classList.remove"
  },
  "classList.toggle": {
    "prefix": "clt",
    "body": [
      "${1:element}.classList.toggle('${2:className}');"
    ],
    "description": "classList.toggle"
  },

  // ==================== TIMING FUNCTIONS ====================
  "setTimeout": {
    "prefix": "st",
    "body": [
      "setTimeout(() => {",
      "  $0",
      "}, ${1:1000});"
    ],
    "description": "setTimeout"
  },
  "setInterval": {
    "prefix": "si",
    "body": [
      "const ${1:intervalId} = setInterval(() => {",
      "  $0",
      "}, ${2:1000});"
    ],
    "description": "setInterval"
  },
  "clearTimeout": {
    "prefix": "ct",
    "body": [
      "clearTimeout(${1:timeoutId});"
    ],
    "description": "clearTimeout"
  },
  "clearInterval": {
    "prefix": "ci",
    "body": [
      "clearInterval(${1:intervalId});"
    ],
    "description": "clearInterval"
  },
  "requestAnimationFrame": {
    "prefix": "raf",
    "body": [
      "const ${1:animate} = () => {",
      "  $0",
      "  requestAnimationFrame(${1:animate});",
      "};",
      "${1:animate}();"
    ],
    "description": "requestAnimationFrame"
  },

  // ==================== CONSOLE METHODS ====================
  "Console Log": {
    "prefix": "cl",
    "body": [
      "console.log($0);"
    ],
    "description": "Console log"
  },
  "Console Log with Label": {
    "prefix": "cll",
    "body": [
      "console.log('${1:label}:', $1);"
    ],
    "description": "Console log with label"
  },
  "Console Error": {
    "prefix": "ce",
    "body": [
      "console.error('${1:error}:', $1);"
    ],
    "description": "Console error"
  },
  "Console Warn": {
    "prefix": "cw",
    "body": [
      "console.warn('${1:warning}:', $1);"
    ],
    "description": "Console warning"
  },
  "Console Table": {
    "prefix": "ct",
    "body": [
      "console.table($1);"
    ],
    "description": "Console table"
  },
  "Console Group": {
    "prefix": "cg",
    "body": [
      "console.group('${1:label}');",
      "$0",
      "console.groupEnd();"
    ],
    "description": "Console group"
  },
  "Console Time": {
    "prefix": "ctime",
    "body": [
      "console.time('${1:label}');",
      "$0",
      "console.timeEnd('${1:label}');"
    ],
    "description": "Console time"
  },
  "Console Dir": {
    "prefix": "cd",
    "body": [
      "console.dir($1);"
    ],
    "description": "Console dir"
  },
  "Console Trace": {
    "prefix": "ctr",
    "body": [
      "console.trace('${1:label}');"
    ],
    "description": "Console trace"
  },

  // ==================== CONTROL FLOW ====================
  "If Statement": {
    "prefix": "if",
    "body": [
      "if (${1:condition}) {",
      "  $0",
      "}"
    ],
    "description": "If statement"
  },
  "If Else": {
    "prefix": "ife",
    "body": [
      "if (${1:condition}) {",
      "  $0",
      "} else {",
      "  ",
      "}"
    ],
    "description": "If else statement"
  },
  "If Else If": {
    "prefix": "ifei",
    "body": [
      "if (${1:condition}) {",
      "  $0",
      "} else if (${2:condition}) {",
      "  ",
      "} else {",
      "  ",
      "}"
    ],
    "description": "If else if statement"
  },
  "Ternary Operator": {
    "prefix": "ter",
    "body": [
      "${1:condition} ? ${2:true} : ${3:false}"
    ],
    "description": "Ternary operator"
  },
  "Switch Statement": {
    "prefix": "sw",
    "body": [
      "switch (${1:expression}) {",
      "  case ${2:value}:",
      "    $0",
      "    break;",
      "  default:",
      "    break;",
      "}"
    ],
    "description": "Switch statement"
  },
  "For Loop": {
    "prefix": "for",
    "body": [
      "for (let ${1:i} = 0; ${1:i} < ${2:array}.length; ${1:i}++) {",
      "  $0",
      "}"
    ],
    "description": "For loop"
  },
  "For Of": {
    "prefix": "forof",
    "body": [
      "for (const ${1:item} of ${2:array}) {",
      "  $0",
      "}"
    ],
    "description": "For of loop"
  },
  "For In": {
    "prefix": "forin",
    "body": [
      "for (const ${1:key} in ${2:object}) {",
      "  if (${2:object}.hasOwnProperty(${1:key})) {",
      "    $0",
      "  }",
      "}"
    ],
    "description": "For in loop"
  },
  "While Loop": {
    "prefix": "while",
    "body": [
      "while (${1:condition}) {",
      "  $0",
      "}"
    ],
    "description": "While loop"
  },
  "Do While": {
    "prefix": "dowhile",
    "body": [
      "do {",
      "  $0",
      "} while (${1:condition});"
    ],
    "description": "Do while loop"
  },

  // ==================== ERROR HANDLING ====================
  "Try Catch": {
    "prefix": "tc",
    "body": [
      "try {",
      "  $0",
      "} catch (error) {",
      "  console.error('Error:', error);",
      "}"
    ],
    "description": "Try catch block"
  },
  "Try Catch Finally": {
    "prefix": "tcf",
    "body": [
      "try {",
      "  $0",
      "} catch (error) {",
      "  console.error('Error:', error);",
      "} finally {",
      "  ",
      "}"
    ],
    "description": "Try catch finally block"
  },
  "Throw Error": {
    "prefix": "te",
    "body": [
      "throw new Error('${1:error message}');"
    ],
    "description": "Throw error"
  },

  // ==================== CLASS ====================
  "Class": {
    "prefix": "cls",
    "body": [
      "class ${1:ClassName} {",
      "  constructor(${2:params}) {",
      "    $0",
      "  }",
      "}"
    ],
    "description": "Class definition"
  },
  "Class with Methods": {
    "prefix": "clsm",
    "body": [
      "class ${1:ClassName} {",
      "  constructor(${2:params}) {",
      "    this.${3:property} = ${2:params};",
      "  }",
      "",
      "  ${4:methodName}() {",
      "    $0",
      "  }",
      "}"
    ],
    "description": "Class with methods"
  },
  "Class Extension": {
    "prefix": "clse",
    "body": [
      "class ${1:ClassName} extends ${2:BaseClass} {",
      "  constructor(${3:params}) {",
      "    super(${3:params});",
      "    $0",
      "  }",
      "}"
    ],
    "description": "Class extension"
  },

  // ==================== STRING METHODS ====================
  "Template Literal": {
    "prefix": "tl",
    "body": [
      "`${${1:expression}}`"
    ],
    "description": "Template literal"
  },
  "String Split": {
    "prefix": "spl",
    "body": [
      "${1:string}.split('${2:separator}');"
    ],
    "description": "String split"
  },
  "String Join": {
    "prefix": "join",
    "body": [
      "${1:array}.join('${2:separator}');"
    ],
    "description": "Array join"
  },
  "String Includes": {
    "prefix": "sinc",
    "body": [
      "${1:string}.includes('${2:searchString}')"
    ],
    "description": "String includes"
  },
  "String Replace": {
    "prefix": "srep",
    "body": [
      "${1:string}.replace('${2:search}', '${3:replace}')"
    ],
    "description": "String replace"
  },
  "String Trim": {
    "prefix": "strim",
    "body": [
      "${1:string}.trim()"
    ],
    "description": "String trim"
  },

  // ==================== JSON ====================
  "JSON Parse": {
    "prefix": "jsp",
    "body": [
      "const ${1:data} = JSON.parse(${2:jsonString});"
    ],
    "description": "JSON parse"
  },
  "JSON Stringify": {
    "prefix": "jss",
    "body": [
      "const ${1:jsonString} = JSON.stringify(${2:data}, null, 2);"
    ],
    "description": "JSON stringify"
  },
  "JSON Try Parse": {
    "prefix": "jstp",
    "body": [
      "let ${1:data};",
      "try {",
      "  ${1:data} = JSON.parse(${2:jsonString});",
      "} catch (error) {",
      "  console.error('JSON parse error:', error);",
      "  ${1:data} = null;",
      "}"
    ],
    "description": "JSON parse with try-catch"
  },

  // ==================== LOCAL STORAGE ====================
  "LocalStorage Set": {
    "prefix": "lss",
    "body": [
      "localStorage.setItem('${1:key}', JSON.stringify(${2:value}));"
    ],
    "description": "LocalStorage set item"
  },
  "LocalStorage Get": {
    "prefix": "lsg",
    "body": [
      "const ${1:data} = JSON.parse(localStorage.getItem('${2:key}'));"
    ],
    "description": "LocalStorage get item"
  },
  "LocalStorage Remove": {
    "prefix": "lsr",
    "body": [
      "localStorage.removeItem('${1:key}');"
    ],
    "description": "LocalStorage remove item"
  },
  "LocalStorage Clear": {
    "prefix": "lsc",
    "body": [
      "localStorage.clear();"
    ],
    "description": "LocalStorage clear"
  },

  // ==================== UTILITIES ====================
  "Import": {
    "prefix": "imp",
    "body": [
      "import ${1:module} from '${2:path}';"
    ],
    "description": "Import statement"
  },
  "Import Destructured": {
    "prefix": "impd",
    "body": [
      "import { ${1:modules} } from '${2:path}';"
    ],
    "description": "Import destructured"
  },
  "Export Default": {
    "prefix": "expd",
    "body": [
      "export default ${1:name};"
    ],
    "description": "Export default"
  },
  "Export Named": {
    "prefix": "expn",
    "body": [
      "export { ${1:name} };"
    ],
    "description": "Export named"
  },
  "Export Const": {
    "prefix": "expc",
    "body": [
      "export const ${1:name} = ${2:value};"
    ],
    "description": "Export const"
  },
  "Typeof Check": {
    "prefix": "tof",
    "body": [
      "typeof ${1:variable} === '${2:type}'"
    ],
    "description": "Typeof check"
  },
  "Instance Of": {
    "prefix": "iof",
    "body": [
      "${1:object} instanceof ${2:Class}"
    ],
    "description": "Instance of check"
  },
  "Spread Operator": {
    "prefix": "spr",
    "body": [
      "...${1:array}"
    ],
    "description": "Spread operator"
  },
  "Rest Parameters": {
    "prefix": "rest",
    "body": [
      "...${1:args}"
    ],
    "description": "Rest parameters"
  },
  "Default Parameters": {
    "prefix": "defp",
    "body": [
      "function ${1:name}(${2:param} = ${3:defaultValue}) {",
      "  $0",
      "}"
    ],
    "description": "Function with default parameters"
  },
  "Optional Chaining": {
    "prefix": "oc",
    "body": [
      "${1:object}?.${2:property}"
    ],
    "description": "Optional chaining"
  },
  "Nullish Coalescing": {
    "prefix": "nc",
    "body": [
      "${1:value} ?? ${2:defaultValue}"
    ],
    "description": "Nullish coalescing operator"
  },
  "Debounce Function": {
    "prefix": "debounce",
    "body": [
      "const ${1:debounce} = (func, delay) => {",
      "  let timeoutId;",
      "  return (...args) => {",
      "    clearTimeout(timeoutId);",
      "    timeoutId = setTimeout(() => func(...args), delay);",
      "  };",
      "};"
    ],
    "description": "Debounce function"
  },
  "Throttle Function": {
    "prefix": "throttle",
    "body": [
      "const ${1:throttle} = (func, limit) => {",
      "  let inThrottle;",
      "  return (...args) => {",
      "    if (!inThrottle) {",
      "      func(...args);",
      "      inThrottle = true;",
      "      setTimeout(() => inThrottle = false, limit);",
      "    }",
      "  };",
      "};"
    ],
    "description": "Throttle function"
  },
  "Deep Clone": {
    "prefix": "clone",
    "body": [
      "const ${1:cloned} = JSON.parse(JSON.stringify(${2:object}));"
    ],
    "description": "Deep clone object"
  },
  "UUID Generator": {
    "prefix": "uuid",
    "body": [
      "const ${1:uuid} = crypto.randomUUID();"
    ],
    "description": "Generate UUID"
  },
  "Random Number": {
    "prefix": "rand",
    "body": [
      "Math.floor(Math.random() * ${1:max}) + ${2:min}"
    ],
    "description": "Random number generator"
  }
}
