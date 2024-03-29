INSTRUCTIONS ON HOW TO SET UP AND RUN THE APPLICATION

1)	Download the project zip file from the GitHub. You can do this by going to Code -> Download ZIP.
2)	Open a new empty project in Android Studio.
3)	Give the name 'toDoListApp' and select 'Kotlin DSL' as the Build configuration language.
4)	Copy files from the downloaded zip folder and paste them into the 'toDoListApp' folder.
5)	In the toolbar, select your app from the run configurations menu.
6)	In the target device menu, select the device that you want to run your app on.
 
If you don’t have any devices configured, you need to either create an Android Virtual Device to use the Android Emulator or connect to physical device.
7)	Click Run.

CONNECTION TO A PHYSICAL DEVICE
1)	Open the settings in your mobile phone. Go to the ‘About Phone’ option. You will find Software version.
2)	Click on the Software version until you go into developer mode.
3)	Open developer options and enable ‘Developer Options’ and ‘USB Debugging’.
4)	Connect your mobile phone to your workstation(laptop) using a USB cable and select mode as ‘FILE TRANSFER’.
5)	Allow the Android Studio to install application in your mobile.

SCREENSHOTS OF THE APPLICATION
1)	After installing the application in the mobile.
   
   <img src="/images/1.jpg" height="400">

2)	Home page in light and dark modes
   
   <img src="/images/2.jpg" height="400"> <img src="/images/3.jpg" height="400">
       
3)	Options in home page in light and dark modes

   <img src="/images/4.jpg" height="400"> <img src="/images/5.jpg" height="400">
       
4)	New Task in light and dark modes

   <img src="/images/6.jpg" height="400"> <img src="/images/7.jpg" height="400">

5)	Categories and Tasks in progress in light and dark modes

   <img src="/images/8.jpg" height="400"> <img src="/images/9.jpg" height="400">
       
6)	Tasks in Progress in a category in light and dark modes

   <img src="/images/10.jpg" height="400"> <img src="/images/11.jpg" height="400">
      
7)	Completed Tasks in light and dark modes

   <img src="/images/12.jpg" height="400"> <img src="/images/13.jpg" height="400">
   <img src="/images/14.jpg" height="400"> <img src="/images/15.jpg" height="400">
       
8)	Settings light and dark mode

   <img src="/images/16.jpg" height="400"> <img src="/images/17.jpg" height="400">
       
9)	Task Notification

    <img src="/images/18.jpg" height="400"> <img src="/images/19.jpg" height="400">


## Tech stack & Open-source libraries
- Minimum SDK level 26
- [Kotlin](https://kotlinlang.org/)
  - Lifecycle: Observe Android lifecycles and handle UI states upon the lifecycle changes.
  - ViewModel: Manages UI-related data holder and lifecycle aware. Allows data to survive configuration changes such as screen rotations.
  - DataBinding: Binds UI components in your layouts to data sources in your app using a declarative format rather than programmatically.
  - Room: Constructs Database by providing an abstraction layer over SQLite to allow fluent database access.
  - Navigation Component Graphs - To use single activity multiple fragment architecture.
  - [Hilt](https://dagger.dev/hilt/): For dependency injection.
  - [Coroutines](https://github.com/Kotlin/kotlinx.coroutines) For asynchronous programming.
- Architecture
  - MVVM Architecture (View - DataBinding - ViewModel - Model)
  - Repository Pattern
- [Material-Components](https://github.com/material-components/material-components-android): Material design components for building ripple animation, and CardView.
- [ColorPicker](https://github.com/QuadFlask/colorpicker): Simple android color picker with color wheel and lightness bar.

## Architecture
**ToDoListApp** is based on the MVVM architecture and the Repository pattern, which follows the [Google's official architecture guidance](https://developer.android.com/topic/architecture).

![architecture](figure/figure0.png)

## Room Database Structure
![database structure](figure/RoomDBStructure.png)
