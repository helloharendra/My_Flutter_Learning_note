# Flutter

- introduction

### what
 - Frame work
 - open source
 - multi-plateform application from single codebase(cross pateform).
# why use Flutter
 
Flutter transforms the app development process.
Build, test, and deploy beautiful mobile,
 web, desktop, and embedded apps from a single codebase.

### who develope    
   - developed By Google. 
   - introduced in 2015.
   - released in 2017.

### installation


#### setup envoirement

- open the command palette. .
- shift+cmd+p on mac os.
- shift+ctrl+p on windows.

- type flutter new project 
- select  select flutter new  project
- select application
- select project path where you want to put your project.
- enter your Project name

- press enter 
#### Ooooo... its done
- you can do anything here that you want in your project.
- here mean lib/main.dart ## under lib folder main.dart is available.

# first flutter app
copy paste from official documentation
follow url 👇
https://codelabs.developers.google.com/codelabs/flutter-codelab-first#2

# Adding Button

ElevatedButton(onPressed: (){      
  print('Next Button Pressed');
},
child: Text('Next'), ),

# main () or main function
its only tell To run flutter app . that is defined in function MyFunction()
 Ex.
 void main(){
  runApp(MyFunction());
 }

 
#  Widgets are the elements from which you build every Flutter app.
#   As you can see, even the app itself is a widget.
Ex. 1.StatelessWidget
    2.StatefulWidget

 class myApp (){ #the starting point of your app.

 } 
 - MyAppState # defines state of your app
 - MyAppState # defines the data the app needs to function. Right now, it only contains a single variable with the - - -current random word pair. You will add to this later.
 - ChangeNotifier
 - way to manage app state in flutter. also maney powefull ways are avialable.
                 
- The state class extends ChangeNotifier which means that it can notify others about its own changes.

- Every widget defines a build() method that's automatically called every time the widget's circumstances change so that the widget is always up to date.
- MyHomePage tracks changes to the app's current state using the watch method.

- Scaffold () :  # it's a helpful widget and is found in the vast majority of real-world Flutter apps.
- Column () :   # is one of the most basic layout widgets in Flutter.

- WordPair # provides several helpful getters, such as asPascalCase or asSnakeCase. Here, we use asLowerCase

### Flutter Code Formatting 

https://docs.flutter.dev/development/tools/formatting 

Flutter code often involves building fairly deep tree-shaped data structures,
for example in a build method. To get good automatic formatting,
we recommend you adopt the optional trailing commas. The guideline for adding 
a trailing comma is simple: Always add a trailing comma at the end of a parameter 
list in functions, methods, and constructors where you care about keeping the 
formatting you crafted. This helps the automatic formatter to insert an appropriate
amount of line breaks for Flutter-style code.

- getNext()
- All that remains is to call the getNext method from the button's callback.
- Making app prettier
- Extract a widget
- The line responsible for showing the current word pair looks like this now: Text(appState.current.asLowerCase). To change it into something more complex, it's a good idea to extract this line into a separate widget. Having separate widgets for separate logical parts of your UI is an important way of managing complexity in Flutter.
### Add a Card

### refactor 
### extract widget 
- select text click on refactor 
- click on extract widget 
- Enter the name of widget
- a class will be created as your Entered Names
### padding
- select text
- right click
- select refactor
- select wrap with padding
- Press Enter

// Note: Flutter uses Composition over Inheritance whenever it can. Here, instead of padding being an attribute of Text, it's a widget!

// This way, widgets can focus on their single responsibility, and you, the developer, have total freedom in how to compose your UI. For example, you can use the Padding widget to pad text, images, buttons, your own custom widgets, or the whole app. The widget doesn't care what it's wrapping.

### Theme and Style

### Functionality
1. Select a layout widget.
2. Visible widget(text, image, Icons).
3. Add the visible widget to the layout widget.
4. Material apps.
5. Non-Material apps.

# Task done

- create a layout
- add image
- add title
- add subtitle
- add like rating icons
- add call icon
- Add label
- add route icon
- Add label
- add share icon
- Add label
- add text (discription)


## Creating responsive and adaptive apps

- LayoutBuilder class 'Builds a widget tree that can depend on the parent widget's size.'
- AspectRatio ('A widget that attempts to size the child to a specific aspect ratio.').
- CustomSingleChildLayout('A widget that defers the layout of its single child to a delegate.')

- SingleChildLayoutDelegate,(' which controls the layout of the child.')
- CustomMultiChildLayout ('which uses a delegate to position multiple children.')

- FittedBox ('Scales and positions its child within itself according to fit.')
- FractionallySizedBox
- LayoutBuilder 
- MediaQuery
- MediaQueryData
- OrientationBuilder


## Layout widgets

## Single child

- Align—Aligns-
    a child within itself. It takes a double value between -1 and 1, for both the vertical and horizontal alignment.

- AspectRatio
    Attempts to size the child to a specific aspect ratio.

- ConstrainedBox
    Imposes size constraints on its child, offering control over the minimum or maximum size.

- CustomSingleChildLayout—
    Uses a delegate function to position a single child. The delegate can determine the layout constraints and positioning for the child.
    
- Expanded and Flexible—
    Allows a child of a Row or Column to shrink or grow to fill any available space.

- FractionallySizedBox—
    Sizes its child to a fraction of the available space.

- LayoutBuilder—
    Builds a widget that can reflow itself based on its parents size.

- SingleChildScrollView—
    Adds scrolling to a single child. Often used with a Row or Column.

### Multichild

- Column, Row, and Flex—Lays out children in a single horizontal or vertical run. Both Column and Row extend the Flex widget.

- CustomMultiChildLayout—Uses a delegate function to position multiple children during the layout phase.

- Flow—Similar to CustomMultiChildLayout, but more efficient because it’s performed during the paint phase rather than the layout phase.

- ListView, GridView, and CustomScrollView—Provides scrollable lists of children.

- Stack—Layers and positions multiple children relative to the edges of the Stack. Functions similarly to position-fixed in CSS.

- Table—Uses a classic table layout algorithm for its children, combining multiple rows and columns.

- Wrap—Displays its children in multiple horizontal or vertical runs.



