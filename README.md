### ENSEACK 2023

 
# TODOs

Work on the powerpoint, work on the shiny, work on the bridge C/Dart. 

# About Flutter

Flutter is a 500MB package. 

# Dart/C bridge 

For the C/Dart bridge there is the ffi package that is a native Dart package I believe. This package looks easy to use but is not since I don’t know flutter that much. 

https://docs.flutter.dev/development/platform-integration/ios/c-interop 

Here is documentation that supposedly can run C within dart. 

I was NOT able to run a hello world because I don’t have a mac or a Windows. Also notice that the hello world needs to work on iOS iphone as well before running the complete C code. And I don’t even know how to access the camera in C using the ffi api. 

Here are the two githubs I tried. 

(much more reliable) (more stars) https://github.com/dart-lang/samples/blob/master/ffi/hello_world/hello.dart 

https://github.com/sensuikan1973/Dart_FFI_Hello_World 

# The UI

The Ui : black and white reminding the design and the aspect of the apriltags. If I have some time I will work on a very simple logo. 

The Ui will be simple, the map will be a flutter canvas displaying a saved picture and the picture is moved depending on the location of the user. 

# Concept, core of the app

Location of the user on the map (the picutre) will be determined by mainly 2 modules. First the apriltags c app is sending/printing on console its “thing”, let’s call what comes out of the apriltags positioning relative to apriltag with id “id” in short relative id location. Then this location is processed by the second module which determines the room the user is in using apriltag’s id, and then his position in the room using the relative position to the apriltag. Translate that into pixel position and you’re done. 

Great now with the pixel position the canvas wil position the picture (the map) to display the position of the user on the map in the middle, that’s my part. 

Send  