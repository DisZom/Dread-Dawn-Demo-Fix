# Dread Dawn Demo Fix
A simple fix that allows you to run demo of Dread Dawn.
The copyright belongs to the original authors.
## Prerequisites

#### 1. You need the Dread Dawn demo files to use this fix
I do not know where you can get them
#### 2. Download and install Java JRE 17 and JavaFX SDK.
I checked it works on: [JRE 17 by Adoptium](https://adoptium.net/temurin/releases/?os=windows&package=jre&version=17&arch=x64) and [OpenJFX](https://gluonhq.com/products/javafx/).
After installing JavaFX, go to where you installed it and rename it javafx-swt.jar on javafx.swt.jar in the lib folder.

## Installation
#### Ready-made version
1. Download the [Game.jar](https://github.com/DisZom/Dread-Dawn-Demo-Fix/blob/main/Game.jar) and move it to the Dread Dawn root folder
2. Create a start.bat and paste this: 
```bat
 <Path to java.exe> --module-path <Path to JavaFX\lib> --add-modules javafx.base,javafx.controls,javafx.fxml,javafx.graphics,javafx.media,javafx.web,javafx.swt -jar Game.jar
```
3. Run start.bat and enjoy the demo

#### Manual
1. You need to get the jav.jar from the Temp folder while the original exe file is running.
2. Open the jav.jar as an archive and extract from the Game folder MyPanel.class and ReaderImage.class
3. You need to open these files in any Java bytecode editor.
4. Find the bytecode: sipush 2024 and change it to any larger one (for example, sipush 3024) and save it.
5. Return these files back to jav.jar and rename jav.jar in Game.jar
6. Move it to the Dread Dawn root folder
7. Create a start.bat and paste this: 
```bat
 <Path to java.exe> --module-path <Path to JavaFX\lib> --add-modules javafx.base,javafx.controls,javafx.fxml,javafx.graphics,javafx.media,javafx.web,javafx.swt -jar Game.jar
```
8. Run start.bat and enjoy the demo
