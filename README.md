# RNNavigationDrawer
React native navigation drawer , where drawer menu is common in all screen

# Steps:

1.react-native init ProjectName
2.cd ProjectName
3. npm install --save react-navigation
4. npm install --save react-native-gesture-handler
5. react-native link

# Note: In android the drawer not working on swipe,add below code in your MainActivity.java
  ```      
  @Override
  protected ReactActivityDelegate createReactActivityDelegate() {
    return new ReactActivityDelegate(this, getMainComponentName()) {
     @Override
     protected ReactRootView createRootView() {
     return new RNGestureHandlerEnabledRootView(MainActivity.this);
      }
    };
  }
  ```
  6. npm i react-native-vector-icons - for menu drawer icon
  
  # Run To Run the React Native App
    1. cd ProjectName
    2. react-native run-android (for android) Or
    3. react-native run-ios (for ios)
