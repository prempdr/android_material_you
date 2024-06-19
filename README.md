# Implementing Material You Colors on your App

[![forthebadge](https://forthebadge.com/images/badges/built-for-android.svg)](https://forthebadge.com)
[![forthebadge](http://forthebadge.com/images/badges/built-with-love.svg)](http://forthebadge.com)

Implement android's new `Material You` colors for `API 31+` with supports for `API 25+`

 ![image](ss_1.png)  ![image](ss_2.png)

# Table of contents

- [Installation](#installation)
- [Recommended configurations](#recommended-configurations)
- [Custom configurations](#custom-configurations)
- [Updating](#updating)
- [Uninstallation](#uninstallation)
- [Contributing](#contributing)
- [License](#license)

# Installation

[(Back to top)](#table-of-contents)

1. Make your own theme files from [Here](https://material-foundation.github.io/material-theme-builder/) , _**you can add your own colors**_
   - [x] (you can also use this project files)
2. Copy those files to your projects respective directories, both `light` and `dark` variant
3. On `your activity.java` file use :
   ```
   if( android.os.Build.VERSION.SDK_INT >= android.os.Build.VERSION_CODES.S){
            DynamicColors.applyToActivityIfAvailable(this);
        }
   ```
   before `setContentView` line

   Here see the usage:
   ![image](ss_3.png)

4. Have a look at the color usages:
   - for backgrounds use `?attr/colorSurfaceContainer`
   - for backgrounds text `?attr/colorOnBackground`
   - for cards use `?attr/colorSurface`
   - for cards text `?attr/colorOnSurface`
   - fot buttons `?attr/colorPrimary` or `?attr/colorSecondary` or `?attr/colorTertiary`
   
   Here see the usage:
   ![image](ss_4.png) ![image](ss_5.png) ![image](ss_6.png)

5. More colors:
   ![image](ss_7.png)


[(Back to top)](#table-of-contents)
