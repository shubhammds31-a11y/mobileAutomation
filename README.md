## Installation

1. Install [XCode](https://apps.apple.com/us/app/xcode/id497799835?mt=12 "XCode")

2. Download and Install [Android Studio](https://developer.android.com/codelabs/basic-android-kotlin-compose-install-android-studio "Android Studio")

3. Download and Install [Python](https://www.python.org/downloads/ "Python")

4. Check Python installation

   `python3 -V`

5. Install [pip](https://pip.pypa.io/ "pip")

   `pip3 -V`

6. Install Appium 2.0
   `npm i -g appium@next`

7. Install Robot Framework

   `pip3 install robotframework`

8. Install Appium Library

   `pip3 install robotframework-appiumlibrary`

9. Download and install VSCode [VSCode](https://code.visualstudio.com/docs/?dv=osx "VSCode")

10. Install [Robot Code](https://marketplace.visualstudio.com/items?itemName=d-biehl.robotcode "Robot Code") extension from VSCode's Marketplace

11. Install Appium Drivers

    `appium driver install uiautomator2`

    `appium driver install xcuitest`

est cases are in `test-cases` directory and covers login and signup functionalities.

## File organization

```
|- robot-framework-mobile-automation-demo/                        // Home folder for robot appium mobile automation project
  |- configs/AppiumConfigs.robot                                  // Appium configurations file
  |- configs/ApplicationConfigs.robot                             // Application configurations file
  |- constants/*.robot                                            // Robot files for the constants
  |- object-repository/locators/*.robot                           // UI locators of the application
  |- object-repository/page-objects/CommonPo.robot                // Common keywords for the application
  |- object-repository/page-objects/*.robot                       // Page object keywords of the application
  |- test-cases/*.robot                                           // Test cases of the application
|- results                                                        // Test results will be saving here
|- .gitignore                                                     // Excluded the unnecessary files in the repo
|- README.md                                                      // This file
```

## Usage

    python3 -m robot -v PLATFORM_NAME:android -i Smoke -d results test-cases
