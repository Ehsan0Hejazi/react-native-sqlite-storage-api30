# react-native-sqlite-storage-api30
Because the original package is not updated for so long,
This is just an update for solving the problem on android 11 and above when switching to API 30 due to security issues

# Installation
npm i --save react-native-sqlite-storage-api30

# Config
in react-native.config.js ==>

dependencies: {
      "react-native-sqlite-storage-api30": {
        platforms: {
          android: {
            sourceDir:
              "../node_modules/react-native-sqlite-storage-api30/platforms/android-native",
            packageImportPath: "import io.liteglue.SQLitePluginPackage;",
            packageInstance: "new SQLitePluginPackage()"
          }
        }
      }
}


# Doc
refer to : https://github.com/andpor/react-native-sqlite-storage