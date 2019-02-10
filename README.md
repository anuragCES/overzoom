# overzoom
overzoom issue on react-native-maps iOS


react-native-maps has a bug on iOS, that consists on requesting tiles 1z+ than specified.
So if you are on zoom 20, rather than requesting tiles z20, will request tiles z21.

This repo basically recreates that issue.
Just clone the project

```
$ npm i
$ npm i -g expo-cli
$ expo start
$ i
```
and head to the settings link on the app.

You must have xCode properly installed.

Then download Charles proxy (https://www.charlesproxy.com/)
and observe how tiles are requested.
