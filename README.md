
# Sample Test Cases
A React Native unit is the smallest testable part of a Reactive Native app.

There are a couple libraries that can help us out with unit testing for React Native
applications:

• React Test Renderer

• React Native Testing Library
## Deployment
Install through yarn
 ```bash
yarn add --dev react-native-testing-library

yarn global add expo-cli

React Native project called react-native-test:

expo init react-native-test
cd react-native-test
```
### Unit Testing
Unit testing is the practice of testing small, isolated pieces of code. React Native itself puts it
thusly:
Unit tests cover the smallest parts of code, like individual functions or classes.

#### Setup
```
{
"scripts": {
"test": "jest"
},
"jest": {
"preset": "react-native"
}
```
####
There are two things we test in components:
1. Interaction, meaning the component responds correctly to the user interaction
2. Output, meaning the component renders the correct output

#### Component Tests
React components are responsible for rendering your app, and users will directly interact with
their output.users. Component tests
could fall into both unit and integration testing, but because they are such a core part of React
Native,

#### Mocking
“Mocking” is when you replace some dependency of your code with your own
implementation.

• It could make the tests slow and unstable (because of the network requests involved)

• The service may return different data every time you run the test

• Third party services can go offline when you really need to run tests!
