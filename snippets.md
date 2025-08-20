`{
 // Place your snippets for typescriptreact here. Each snippet is defined under a snippet name and has a prefix, body and 
 // description. The prefix is what is used to trigger the snippet and the body will be expanded and inserted. Possible variables are:
 // $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders. Placeholders with the 
 // same ids are connected.
 // Example:
 "Custom Console log print...": {
  "prefix": "cc",
  "body": [
   "console.log('$1-->',$1);",
  ],
  "description": "Console log"
 },
 "Custom Console Log Object...": {
  "prefix": "cj",
  "body": [
   "console.log('$1:', JSON.stringify($1, null, 2));"
  ],
  "description": "Console log object with formatting"
 },
 "Custom useEffect Basic...": {
  "prefix": "useEff",
  "body": [
   "useEffect(() => {",
   "  $1",
   "}, []);"
  ],
  "description": "Basic useEffect with empty dependencies"
 },
 "Custom useEffect with Dependencies...": {
  "prefix": "useEff2",
  "body": [
   "useEffect(() => {",
   "  $1",
   "}, [$2]);"
  ],
  "description": "useEffect with dependencies array"
 },
 "Custom useEffect with Cleanup...": {
  "prefix": "useEff3",
  "body": [
   "useEffect(() => {",
   "  $1",
   "  ",
   "  return () => {",
   "    $2",
   "  };",
   "}, [$3]);"
  ],
  "description": "useEffect with cleanup function"
 },
 "Custom useState...": {
  "prefix": "usestate",
  "body": [
   "const [$1, set${1/(.*)/${1:/capitalize}/}] = useState($2);"
  ],
  "description": "React useState hook"
 },
 "Custom Arrow Function...": {
  "prefix": "fnc",
  "body": [
   "const ${1:functionName} = ($2) => {",
   "  $3",
   "};"
  ],
  "description": "Arrow function"
 },
 "Custom Async Function...": {
  "prefix": "fncAsync",
  "body": [
   "const ${1:functionName} = async () => {",
   "  try {",
   "    $2",
   "  } catch (error) {",
   "    console.error('Error in $1:', error);",
   "  }",
   "};"
  ],
  "description": "Async function with error handling"
 },
 "Custom Try Catch...": {
  "prefix": "try",
  "body": [
   "try {",
   "  $1",
   "} catch (error) {",
   "  console.error('Error:', error);",
   "}"
  ],
  "description": "Try catch block"
 }
}`
