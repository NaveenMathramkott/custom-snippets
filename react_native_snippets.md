{
  // ==================== REACT NATIVE SCREENS ====================
  "React Native Screen with SafeArea": {
    "prefix": "rnscreen",
    "body": [
      "import React from 'react';",
      "import { View, Text, StyleSheet, SafeAreaView } from 'react-native';",
      "",
      "const ${1:ScreenName} = () => {",
      "  return (",
      "    <SafeAreaView style={styles.container}>",
      "      <View style={styles.content}>",
      "        <Text style={styles.title}>$0</Text>",
      "      </View>",
      "    </SafeAreaView>",
      "  );",
      "};",
      "",
      "const styles = StyleSheet.create({",
      "  container: {",
      "    flex: 1,",
      "    backgroundColor: '#fff',",
      "  },",
      "  content: {",
      "    flex: 1,",
      "    padding: 16,",
      "  },",
      "  title: {",
      "    fontSize: 24,",
      "    fontWeight: 'bold',",
      "  },",
      "});",
      "",
      "export default ${1:ScreenName};"
    ],
    "description": "React Native screen with SafeAreaView"
  },
  "React Native Screen with KeyboardAvoidingView": {
    "prefix": "rnkeyboard",
    "body": [
      "import React from 'react';",
      "import { View, StyleSheet, KeyboardAvoidingView, Platform } from 'react-native';",
      "",
      "const ${1:ScreenName} = () => {",
      "  return (",
      "    <KeyboardAvoidingView",
      "      style={styles.container}",
      "      behavior={Platform.OS === 'ios' ? 'padding' : 'height'}",
      "    >",
      "      $0",
      "    </KeyboardAvoidingView>",
      "  );",
      "};",
      "",
      "const styles = StyleSheet.create({",
      "  container: {",
      "    flex: 1,",
      "  },",
      "});",
      "",
      "export default ${1:ScreenName};"
    ],
    "description": "Screen with KeyboardAvoidingView"
  },

  // ==================== FLATLIST VARIATIONS ====================
  "FlatList with Empty State": {
    "prefix": "rnfle",
    "body": [
      "<FlatList",
      "  data={${1:data}}",
      "  keyExtractor={(item) => item.${2:id}.toString()}",
      "  renderItem={({ item, index }) => (",
      "    $0",
      "  )}",
      "  ListEmptyComponent={() => (",
      "    <View style={styles.emptyContainer}>",
      "      <Text>No items found</Text>",
      "    </View>",
      "  )}",
      "  contentContainerStyle={styles.listContainer}",
      "/>"
    ],
    "description": "FlatList with empty state"
  },
  "FlatList with Pull to Refresh": {
    "prefix": "rnflr",
    "body": [
      "const [refreshing, setRefreshing] = React.useState(false);",
      "",
      "const onRefresh = React.useCallback(() => {",
      "  setRefreshing(true);",
      "  // Fetch data",
      "  $0",
      "  setRefreshing(false);",
      "}, []);",
      "",
      "<FlatList",
      "  data={${1:data}}",
      "  keyExtractor={(item) => item.${2:id}.toString()}",
      "  renderItem={({ item }) => (",
      "    ${3:renderItem}",
      "  )}",
      "  refreshing={refreshing}",
      "  onRefresh={onRefresh}",
      "/>"
    ],
    "description": "FlatList with pull to refresh"
  },
  "FlatList with Load More": {
    "prefix": "rnfll",
    "body": [
      "const [loading, setLoading] = React.useState(false);",
      "",
      "const loadMore = () => {",
      "  if (!loading) {",
      "    setLoading(true);",
      "    // Load more data",
      "    $0",
      "    setLoading(false);",
      "  }",
      "};",
      "",
      "<FlatList",
      "  data={${1:data}}",
      "  keyExtractor={(item) => item.${2:id}.toString()}",
      "  renderItem={({ item }) => (",
      "    ${3:renderItem}",
      "  )}",
      "  onEndReached={loadMore}",
      "  onEndReachedThreshold={0.5}",
      "  ListFooterComponent={() => loading && <ActivityIndicator />}",
      "/>"
    ],
    "description": "FlatList with load more pagination"
  },
  "FlatList Horizontal": {
    "prefix": "rnflh",
    "body": [
      "<FlatList",
      "  data={${1:data}}",
      "  horizontal",
      "  showsHorizontalScrollIndicator={false}",
      "  keyExtractor={(item) => item.${2:id}.toString()}",
      "  renderItem={({ item }) => (",
      "    $0",
      "  )}",
      "  contentContainerStyle={styles.listContainer}",
      "/>"
    ],
    "description": "Horizontal FlatList"
  },

  // ==================== SCROLLVIEW ====================
  "ScrollView with RefreshControl": {
    "prefix": "rnsv",
    "body": [
      "const [refreshing, setRefreshing] = React.useState(false);",
      "",
      "const onRefresh = React.useCallback(() => {",
      "  setRefreshing(true);",
      "  $0",
      "  setRefreshing(false);",
      "}, []);",
      "",
      "<ScrollView",
      "  refreshControl={",
      "    <RefreshControl refreshing={refreshing} onRefresh={onRefresh} />",
      "  }",
      "  contentContainerStyle={styles.scrollContent}",
      ">",
      "  ${1:content}",
      "</ScrollView>"
    ],
    "description": "ScrollView with RefreshControl"
  },

  // ==================== TOUCHABLES ====================
  "TouchableOpacity with Feedback": {
    "prefix": "rnto",
    "body": [
      "<TouchableOpacity",
      "  onPress={${1:handlePress}}",
      "  activeOpacity={0.7}",
      "  style={styles.${2:button}}",
      ">",
      "  $0",
      "</TouchableOpacity>"
    ],
    "description": "TouchableOpacity with activeOpacity"
  },
  "Pressable Component": {
    "prefix": "rnpr",
    "body": [
      "<Pressable",
      "  onPress={${1:handlePress}}",
      "  style={({ pressed }) => [",
      "    styles.${2:button},",
      "    pressed && styles.${3:pressed}",
      "  ]}",
      ">",
      "  {({ pressed }) => (",
      "    $0",
      "  )}",
      "</Pressable>"
    ],
    "description": "Pressable with pressed state"
  },

  // ==================== TEXTINPUT VARIATIONS ====================
  "TextInput with Label": {
    "prefix": "rntil",
    "body": [
      "<View style={styles.inputContainer}>",
      "  <Text style={styles.label}>${1:Label}</Text>",
      "  <TextInput",
      "    value={${2:value}}",
      "    onChangeText={${3:setValue}}",
      "    placeholder=\"${4:Enter text}\"",
      "    style={styles.input}",
      "    placeholderTextColor=\"#999\"",
      "  />",
      "</View>",
      "$0"
    ],
    "description": "TextInput with label"
  },
  "TextInput Secure": {
    "prefix": "rntis",
    "body": [
      "const [showPassword, setShowPassword] = React.useState(false);",
      "",
      "<View style={styles.inputContainer}>",
      "  <TextInput",
      "    value={${1:password}}",
      "    onChangeText={${2:setPassword}}",
      "    placeholder=\"Password\"",
      "    secureTextEntry={!showPassword}",
      "    style={styles.input}",
      "  />",
      "  <TouchableOpacity onPress={() => setShowPassword(!showPassword)}>",
      "    <Text>{showPassword ? 'Hide' : 'Show'}</Text>",
      "  </TouchableOpacity>",
      "</View>",
      "$0"
    ],
    "description": "Secure TextInput with show/hide toggle"
  },
  "TextInput Multiline": {
    "prefix": "rntim",
    "body": [
      "<TextInput",
      "  value={${1:value}}",
      "  onChangeText={${2:setValue}}",
      "  placeholder=\"${3:Enter text}\"",
      "  multiline",
      "  numberOfLines={${4:4}}",
      "  textAlignVertical=\"top\"",
      "  style={styles.${5:textArea}}",
      "/>"
    ],
    "description": "Multiline TextInput"
  },

  // ==================== MODAL ====================
  "Modal Component": {
    "prefix": "rnmod",
    "body": [
      "const [modalVisible, setModalVisible] = React.useState(false);",
      "",
      "<Modal",
      "  visible={modalVisible}",
      "  animationType=\"${1:slide}\"",
      "  transparent={${2:true}}",
      "  onRequestClose={() => setModalVisible(false)}",
      ">",
      "  <View style={styles.modalContainer}>",
      "    <View style={styles.modalContent}>",
      "      $0",
      "      <TouchableOpacity onPress={() => setModalVisible(false)}>",
      "        <Text>Close</Text>",
      "      </TouchableOpacity>",
      "    </View>",
      "  </View>",
      "</Modal>"
    ],
    "description": "Modal component with state"
  },

  // ==================== IMAGE ====================
  "Image with URI": {
    "prefix": "rnimg",
    "body": [
      "<Image",
      "  source={{ uri: '${1:https://example.com/image.jpg}' }}",
      "  style={styles.${2:image}}",
      "  resizeMode=\"${3:cover}\"",
      "/>"
    ],
    "description": "Image with URI source"
  },
  "Image Local": {
    "prefix": "rnimgl",
    "body": [
      "<Image",
      "  source={require('${1:./assets/image.png}')}",
      "  style={styles.${2:image}}",
      "  resizeMode=\"${3:contain}\"",
      "/>"
    ],
    "description": "Image with local source"
  },
  "ImageBackground": {
    "prefix": "rnimgb",
    "body": [
      "<ImageBackground",
      "  source={{ uri: '${1:https://example.com/image.jpg}' }}",
      "  style={styles.${2:background}}",
      "  resizeMode=\"${3:cover}\"",
      ">",
      "  $0",
      "</ImageBackground>"
    ],
    "description": "ImageBackground component"
  },

  // ==================== ANIMATED ====================
  "Animated Value": {
    "prefix": "rnanim",
    "body": [
      "const ${1:fadeAnim} = React.useRef(new Animated.Value(${2:0})).current;",
      "",
      "React.useEffect(() => {",
      "  Animated.timing(${1:fadeAnim}, {",
      "    toValue: ${3:1},",
      "    duration: ${4:1000},",
      "    useNativeDriver: true,",
      "  }).start();",
      "}, []);",
      "",
      "<Animated.View style={{ opacity: ${1:fadeAnim} }}>",
      "  $0",
      "</Animated.View>"
    ],
    "description": "Animated value with timing"
  },
  "Animated Spring": {
    "prefix": "rnanims",
    "body": [
      "const ${1:springAnim} = React.useRef(new Animated.Value(${2:0})).current;",
      "",
      "const ${3:animate} = () => {",
      "  Animated.spring(${1:springAnim}, {",
      "    toValue: ${4:1},",
      "    friction: ${5:3},",
      "    tension: ${6:40},",
      "    useNativeDriver: true,",
      "  }).start();",
      "};",
      "$0"
    ],
    "description": "Animated spring animation"
  },

  // ==================== NAVIGATION ====================
  "Stack Navigator": {
    "prefix": "rnstack",
    "body": [
      "import { createNativeStackNavigator } from '@react-navigation/native-stack';",
      "",
      "const Stack = createNativeStackNavigator();",
      "",
      "const ${1:AppNavigator} = () => {",
      "  return (",
      "    <Stack.Navigator",
      "      initialRouteName=\"${2:Home}\"",
      "      screenOptions={{",
      "        headerStyle: { backgroundColor: '${3:#fff}' },",
      "        headerTintColor: '${4:#000}',",
      "      }}",
      "    >",
      "      <Stack.Screen name=\"${2:Home}\" component={${5:HomeScreen}} />",
      "      $0",
      "    </Stack.Navigator>",
      "  );",
      "};"
    ],
    "description": "Stack Navigator setup"
  },
  "Tab Navigator": {
    "prefix": "rntab",
    "body": [
      "import { createBottomTabNavigator } from '@react-navigation/bottom-tabs';",
      "",
      "const Tab = createBottomTabNavigator();",
      "",
      "const ${1:TabNavigator} = () => {",
      "  return (",
      "    <Tab.Navigator",
      "      screenOptions={{",
      "        tabBarActiveTintColor: '${2:#007AFF}',",
      "        tabBarInactiveTintColor: '${3:#8E8E93}',",
      "      }}",
      "    >",
      "      <Tab.Screen name=\"${4:Home}\" component={${5:HomeScreen}} />",
      "      $0",
      "    </Tab.Navigator>",
      "  );",
      "};"
    ],
    "description": "Tab Navigator setup"
  },
  "Navigation Options": {
    "prefix": "rnnavopt",
    "body": [
      "React.useLayoutEffect(() => {",
      "  navigation.setOptions({",
      "    title: '${1:Title}',",
      "    headerRight: () => (",
      "      <TouchableOpacity onPress={${2:handlePress}}>",
      "        <Text>${3:Action}</Text>",
      "      </TouchableOpacity>",
      "    ),",
      "  });",
      "}, [navigation]);",
      "$0"
    ],
    "description": "Set navigation options"
  },

  // ==================== DIMENSIONS & PLATFORM ====================
  "Get Dimensions": {
    "prefix": "rndim",
    "body": [
      "const { width, height } = Dimensions.get('${1:window}');",
      "$0"
    ],
    "description": "Get screen dimensions"
  },
  "Platform Specific Code": {
    "prefix": "rnplat",
    "body": [
      "Platform.select({",
      "  ios: ${1:iosValue},",
      "  android: ${2:androidValue},",
      "})"
    ],
    "description": "Platform specific values"
  },
  "Platform OS Check": {
    "prefix": "rnplatos",
    "body": [
      "Platform.OS === '${1:ios}' ? ${2:iosCode} : ${3:androidCode}"
    ],
    "description": "Platform OS check"
  },

  // ==================== STYLESHEET PATTERNS ====================
  "StyleSheet Create": {
    "prefix": "rnss",
    "body": [
      "const styles = StyleSheet.create({",
      "  container: {",
      "    flex: 1,",
      "    backgroundColor: '${1:#fff}',",
      "    padding: ${2:16},",
      "  },",
      "  $0",
      "});"
    ],
    "description": "Create StyleSheet"
  },
  "Flexbox Layout": {
    "prefix": "rnflex",
    "body": [
      "${1:container}: {",
      "  flex: ${2:1},",
      "  flexDirection: '${3:column}',",
      "  justifyContent: '${4:center}',",
      "  alignItems: '${5:center}',",
      "},"
    ],
    "description": "Flexbox layout style"
  },
  "Shadow Style": {
    "prefix": "rnshadow",
    "body": [
      "${1:shadow}: {",
      "  ...Platform.select({",
      "    ios: {",
      "      shadowColor: '${2:#000}',",
      "      shadowOffset: { width: 0, height: 2 },",
      "      shadowOpacity: ${3:0.25},",
      "      shadowRadius: ${4:3.84},",
      "    },",
      "    android: {",
      "      elevation: ${5:5},",
      "    },",
      "  }),",
      "},"
    ],
    "description": "Cross-platform shadow style"
  },

  // ==================== GESTURES ====================
  "PanResponder": {
    "prefix": "rnpan",
    "body": [
      "const panResponder = React.useRef(",
      "  PanResponder.create({",
      "    onStartShouldSetPanResponder: () => true,",
      "    onPanResponderMove: (evt, gestureState) => {",
      "      $0",
      "    },",
      "    onPanResponderRelease: (evt, gestureState) => {",
      "      ${1:// Handle release}",
      "    },",
      "  })",
      ").current;"
    ],
    "description": "PanResponder for gestures"
  },

  // ==================== ASYNC STORAGE ====================
  "AsyncStorage Set": {
    "prefix": "rnaset",
    "body": [
      "const ${1:storeData} = async (${2:key}, ${3:value}) => {",
      "  try {",
      "    await AsyncStorage.setItem(${2:key}, JSON.stringify(${3:value}));",
      "  } catch (error) {",
      "    console.error('Error storing data:', error);",
      "  }",
      "};",
      "$0"
    ],
    "description": "AsyncStorage set item"
  },
  "AsyncStorage Get": {
    "prefix": "rnaget",
    "body": [
      "const ${1:getData} = async (${2:key}) => {",
      "  try {",
      "    const value = await AsyncStorage.getItem(${2:key});",
      "    return value ? JSON.parse(value) : null;",
      "  } catch (error) {",
      "    console.error('Error retrieving data:', error);",
      "    return null;",
      "  }",
      "};",
      "$0"
    ],
    "description": "AsyncStorage get item"
  },
  "AsyncStorage Remove": {
    "prefix": "rnarem",
    "body": [
      "const ${1:removeData} = async (${2:key}) => {",
      "  try {",
      "    await AsyncStorage.removeItem(${2:key});",
      "  } catch (error) {",
      "    console.error('Error removing data:', error);",
      "  }",
      "};",
      "$0"
    ],
    "description": "AsyncStorage remove item"
  },

  // ==================== ALERTS ====================
  "Alert Simple": {
    "prefix": "rnalert",
    "body": [
      "Alert.alert(",
      "  '${1:Title}',",
      "  '${2:Message}',",
      "  [",
      "    { text: 'OK', onPress: () => ${3:console.log('OK Pressed')} }",
      "  ]",
      ");"
    ],
    "description": "Simple Alert"
  },
  "Alert with Buttons": {
    "prefix": "rnalertb",
    "body": [
      "Alert.alert(",
      "  '${1:Confirm Action}',",
      "  '${2:Are you sure?}',",
      "  [",
      "    {",
      "      text: 'Cancel',",
      "      onPress: () => console.log('Cancel Pressed'),",
      "      style: 'cancel',",
      "    },",
      "    {",
      "      text: 'OK',",
      "      onPress: () => ${3:handleConfirm()},",
      "    },",
      "  ]",
      ");"
    ],
    "description": "Alert with multiple buttons"
  },

  // ==================== LINKING ====================
  "Open URL": {
    "prefix": "rnlink",
    "body": [
      "const ${1:openURL} = async (${2:url}) => {",
      "  const supported = await Linking.canOpenURL(${2:url});",
      "  if (supported) {",
      "    await Linking.openURL(${2:url});",
      "  } else {",
      "    Alert.alert(`Don't know how to open this URL: ${${2:url}}`);",
      "  }",
      "};",
      "$0"
    ],
    "description": "Open URL with Linking"
  },

  // ==================== PERMISSIONS ====================
  "Request Permission": {
    "prefix": "rnperm",
    "body": [
      "const ${1:requestPermission} = async () => {",
      "  try {",
      "    const granted = await PermissionsAndroid.request(",
      "      PermissionsAndroid.PERMISSIONS.${2:CAMERA},",
      "      {",
      "        title: '${3:Permission Title}',",
      "        message: '${4:Permission Message}',",
      "        buttonPositive: 'OK',",
      "      }",
      "    );",
      "    if (granted === PermissionsAndroid.RESULTS.GRANTED) {",
      "      console.log('Permission granted');",
      "      $0",
      "    } else {",
      "      console.log('Permission denied');",
      "    }",
      "  } catch (error) {",
      "    console.error('Permission error:', error);",
      "  }",
      "};"
    ],
    "description": "Request Android permission"
  },

  // ==================== DEBUGGING ====================
  "React Native Log": {
    "prefix": "rnlog",
    "body": [
      "console.log('[${1:Component}] ${2:message}:', $2);"
    ],
    "description": "Labeled console log for RN"
  },
  "React Native Dev Log": {
    "prefix": "rnlogd",
    "body": [
      "if (__DEV__) {",
      "  console.log('${1:Debug}:', $0);",
      "}"
    ],
    "description": "Development-only console log"
  },
  "Performance Log": {
    "prefix": "rnperf",
    "body": [
      "const ${1:startTime} = Date.now();",
      "$0",
      "console.log('${2:Operation} took:', Date.now() - ${1:startTime}, 'ms');"
    ],
    "description": "Performance timing log"
  },

  // ==================== CUSTOM HOOKS ====================
  "useEffect for Mount Only": {
    "prefix": "rnuem",
    "body": [
      "React.useEffect(() => {",
      "  $0",
      "}, []);"
    ],
    "description": "useEffect mount only"
  },
  "useBackHandler": {
    "prefix": "rnback",
    "body": [
      "React.useEffect(() => {",
      "  const backHandler = BackHandler.addEventListener(",
      "    'hardwareBackPress',",
      "    () => {",
      "      $0",
      "      return true; // Return true to prevent default back behavior",
      "    }",
      "  );",
      "",
      "  return () => backHandler.remove();",
      "}, []);"
    ],
    "description": "Android back button handler"
  },
  "useFocusEffect": {
    "prefix": "rnfocus",
    "body": [
      "import { useFocusEffect } from '@react-navigation/native';",
      "",
      "useFocusEffect(",
      "  React.useCallback(() => {",
      "    $0",
      "    ",
      "    return () => {",
      "      // Cleanup",
      "    };",
      "  }, [])",
      ");"
    ],
    "description": "useFocusEffect for navigation"
  }
}
