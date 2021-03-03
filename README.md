# React-Native-Course-Blog

Start up steps:

-Download Node at nodejs.org/download/ if npm error

Preliminary Steps:
-Make project folder
-Run "npm install"

1. Install Expo Cli: npx expo-cli init 'project name' --npm
2. Choose Blank
3. Change {name} to name of project
4. Run "cd 'project name'"
5. Run "npm install react-navigation"
6. Run "npm start"

Setting Up JSON Server:
1. In workspace, above project, run "mkdir jsonserver"
2. Move into jsonserver/ folder
3. Run "npm init"
4. Run "npm install json-server ngrok"
5. Run "code ." to open it in a new code editor
6. Create and edit file called "db.json"
7. Edit package.json
8. Run "npm run db" in json path in a different terminal
9. Run "npm run tunnel" in json path in a different terminal
10. Add ngrok forwarding link to jsonServer.js (update each time) in main app
11. Open another terminal in main project and run "npm install axios"

For accessing any server using ngrok:
npm install -g ngrok

For starting up full tracker app:
1. Run "npm start" in one terminal under the project
2. Run "npm run dev" in a different terminal under tracker-server
3. Run "ngrok http 3000" in a different third terminal under the project 
4. Replace baseURL in tracker.js with new ngrok URL 
5. Test user to sign in is:
    -Email: test1@test.com
    -Password: mypassword

------------------------------------------------------------------------

React js template (plus a little excess):

import React from 'react';
import { View, Text, StyleSheet } from 'react-native';

const SearchScreen = () => {
    return (
        <View>
            <Text>Search Screen</Text>
        </View>
    );
};

const styles = StyleSheet.create({});

export default SearchScreen;



import { createAppContainer } from 'react-navigation';
import { createStackNavigator } from 'react-navigation-stack';

import { createAppContainer, createSwitchNavigator } from 'react-navigation';
import { createStackNavigator } from 'react-navigation-stack';
import { createBottomTabNavigator } from 'react-navigation-tabs';

------------------------------------------------------------------------

Resources:

Free hosted mongodb: cloud.mongodb.com
Postman: getpostman.com
Json web token: https://jwt.io/
React Native Elements: https://reactnativeelements.com/docs/overview
React Native Maps: npx expo-cli install react-native-maps
Expo Location for Tracking: npx expo-cli install expo-location

------------------------------------------------------------------------

Track-server start up (tracker app):

npm run dev

------------------------------------------------------------------------

Json-server start up (blog app):

https://www.npmjs.com/package/json-server
npm start
npm run db
npm run tunnel

package.json changes:
Replace what's under scripts with this for example:
"db": "json-server -w db.json",
"tunnel": "ngrok http 3000"

------------------------------------------------------------------------

Client ID:

fgKjGSRla5T1Qtyawjic5A

------------------------------------------------------------------------

API Key:

gcoOP0_jkeAFVR6lx0dr8_vt0Kr_eFnndD4vEcfCNFBBSTxdd5XQ8vJEX3kVPQo1bynejJr3UIqFxrDDKI2WRwFkCHQGeXytXWDasoLpWzSj5X_mDyFxadmeJEVUXXYx

------------------------------------------------------------------------

VS Code Git authentication token:

vscode://vscode.github-authentication/did-authenticate?windowid=1&code=d6429a6c005643579661&state=194470aa-e03e-4c3a-a2e4-f3e204cf1cf7

------------------------------------------------------------------------

Please note down the Temporary Application ID : AAXA2335ZRJHJXZ