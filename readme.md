### This is a min react-native [hot-code-push](https://github.com/Microsoft/react-native-code-push) POC.
To test code-push function, follow these steps:
1. git clone this repo
2. npm i
3. install the latest version of [react-native](https://facebook.github.io/react-native/)
4. react-native link pushPOC  (pushPOC is the app name for this)
5. react-native run-ios/react-native run-andoid
6. modify some text on index.ios.js
7. refresh the simulator, the changes won't apply, beacuse we change the debug code source from jsBundle to coddepush budleURL in AppDelegate.m
8. On terminal,  `code-push release-react pushPOC ios`, this action will upgrade the codepush bundle online. 
9. re-run your app on simulator, refresh. changes not happend.(automatic updadte had been disabled for clearly testing.)
10. click check for upadtes, update dialog will show up.

[A video tutorial For setup codepush for react-native apps:](https://www.youtube.com/watch?v=f6I9y7V-Ibk)