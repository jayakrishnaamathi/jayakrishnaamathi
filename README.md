import React from 'react';
import { StyleSheet, Text, View, Button, Alert } from 'react-native';

const App = () => {
  const showAlert = () => {
    Alert.alert('Alert', 'Button was pressed!');
  };

  return (
    <View style={styles.wrapper}>
      <Text style={styles.title}>Hello from My Webpage</Text>
      <Text style={styles.description}>
        Here is a simple React Native app example.
      </Text>
      <Button
        title="Press Me"
        onPress={showAlert}
      />
    </View>
  );
}

const styles = StyleSheet.create({
  wrapper: {
    flex: 1,
    backgroundColor: 'yellow',
    alignItems: 'center',
    justifyContent: 'center',
    padding: 20,
  },
  title: {
    fontSize: 26,
    fontWeight: 'bold',
    marginBottom: 18,
  },
  description: {
    fontSize: 18,
    textAlign: 'center',
    marginBottom: 18,
  },
});

export default App;
