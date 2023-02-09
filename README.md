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

# developer    
    developed By Google.
  ###  
    introduced in 2015.
    released in 2017.

# instalation


# setup envoirement

open the command palette. .
shift+cmd+p on mac os.
shift+ctrl+p on windows.

type flutter new project 
select  select flutter new  project
select application
select project path where you want to put your project.
enter your Project name

press enter 
Ooooo... its done
you can do anything here that you want in your project.
here mean lib/main.dart ## under lib folder main.dart is available.

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
 MyAppState # defines state of your app
 MyAppState # defines the data the app needs to function. Right now, it only contains a single variable with the current random word pair. You will add to this later.
 ChangeNotifier  # way to manage app state in flutter. also maney powefull ways are avialable.
                 # The state class extends ChangeNotifier which means that it can notify others about its own changes.

# Every widget defines a build() method that's automatically called every time the widget's circumstances change so that the widget is always up to date.
# MyHomePage tracks changes to the app's current state using the watch method.

Scaffold () :  # it's a helpful widget and is found in the vast majority of real-world Flutter apps.
Column () :   # is one of the most basic layout widgets in Flutter.

WordPair # provides several helpful getters, such as asPascalCase or asSnakeCase. Here, we use asLowerCase

Flutter Code Formatting 

https://docs.flutter.dev/development/tools/formatting 
