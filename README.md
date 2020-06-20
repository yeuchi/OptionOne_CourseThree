# OptionOne_CourseThree
Course #3 Swift Design Development : Option #1

For all the lesson projects in Course #3, see below repository.
https://github.com/yeuchi/SwiftDesignDev

## Course
Coursera University of Toronto iOS App Development with Swift Specialization Courses:
Course 3 : App Design and Development for iOS with Professor Parham Aarabi.

https://www.coursera.org/learn/ios-app-design-development

Course Forum
https://www.coursera.org/learn/ios-app-design-development/discussions

### Option 1: iPhone App
- For Option 1, you will build an iPhone app with the following requirements:
- Your app must have user interaction in the form of a scrollview, gesture recognizers or custom touch handling.
- Your app must have at least three view controllers that all play a role in the app.
- Your app must have data that persists between app sessions and/or networking functionality.

### Rubric

#### SUBMISSION: 
Make sure all your project files are in a single folder with the main Xcode project file (with the .xcodeproj extension) at the top level. Zip the folder first using the Mac’s compression command. (In Finder, right-click the folder and select “Compress”.) Upload this zipped archive for review. Your peer reviewers will download your zipped file and run the project in their own Xcode.

#### LANGUAGE: 
Submissions must be in English

#### Review criterialess 
To evaluate your peers in the best way possible, you should briefly review the work of your peers using the buttons near the top of this screen before giving scores and feedback on any of them. This will help open your eyes to what others have done.
You will be asked to provide feedback to your peers in the following areas:
- Does the app fulfill the three requirements for each option? 2pts per requirement.
- Does the app provide useful or interesting functionality? 1 pt
- Does the app have a nice, structured user interface? 1pt


### Project OptionOne Implementation 

#### Data Persistence : Setting -> OptionOne

From Mike Spears' lesson, I added a Bundle Setting file to store UserDefaults (Kittens, Pugs, Pizza). \
<img width="500" alt="settings" src="https://user-images.githubusercontent.com/1282659/85211930-73657180-b313-11ea-8bfc-1b6fd1745b31.png">

Simulation results are functional as follows. \
<img width="220" alt="option1" src="https://user-images.githubusercontent.com/1282659/85211933-76f8f880-b313-11ea-9474-05b86c81231c.png"> <img width="220" alt="searchTag" src="https://user-images.githubusercontent.com/1282659/85212606-16b98500-b31a-11ea-9b78-645103a37b35.png"> <img width="220" alt="selection" src="https://user-images.githubusercontent.com/1282659/85212583-da862480-b319-11ea-8a6a-828902bc61ae.png">

#### Network Request : Button -> New File

Instead of loading image from camera or album, we can load from Flickr's selections. \
<img width="220" alt="flickr" src="https://user-images.githubusercontent.com/1282659/85212011-259d3900-b314-11ea-81a9-7ab8a1a57d6e.png"> <img width="220" alt="loaded" src="https://user-images.githubusercontent.com/1282659/85212013-29c95680-b314-11ea-9adf-b4a9601c9906.png">

#### ScrollView Pan & Zoom & double-tap

Per Jack Wu's instruction, below illustrates zoom by double tap, mouse-drag-pan and option-key-mouse-move-zoom. \
<img width="220" alt="doubleTap" src="https://user-images.githubusercontent.com/1282659/85212023-42397100-b314-11ea-9356-30db58f68064.png"> <img width="220" alt="pan" src="https://user-images.githubusercontent.com/1282659/85212027-46658e80-b314-11ea-88b8-3069396609a0.png"> <img width="220" alt="option_mouse" src="https://user-images.githubusercontent.com/1282659/85212028-4796bb80-b314-11ea-9422-9b01af995b1f.png"> <img width="220" alt="pan2" src="https://user-images.githubusercontent.com/1282659/85212692-e6261b00-b31a-11ea-86d3-e0b3c6f07fb8.png">

#### Filter - Image Processing - Spatial Convolution

!!! Please pardon the 'SLOW' processing time when image is LARGE !!!
Below demonstrates execution of a sharpening filter.
<img width="220" alt="filter_list" src="https://user-images.githubusercontent.com/1282659/85212682-c55dc580-b31a-11ea-813a-21add3be6270.png"> <img width="220" alt="sharpen" src="https://user-images.githubusercontent.com/1282659/85212683-c68ef280-b31a-11ea-82ce-b98a7e434873.png">

# IDE
XCode 11.1 require considerable changes on constraints for scrollview panning and zoom to work properly.
Keeping it simple, I use XCode 10.1 Swift 4.2 to implement these features.  It will still build and execute in XCode 11.1 fine.  Detail articles are available in my lesson repository <sup>[1]</sup>

# Simulator
All testings were performed with an iPhone 8 (16B91) portrait mode.
Above screenshots were produced on a MacBookPro OS Catalina.

# References 

1. Course #3 Swift Design and Development exercise, re-implemented by Chi T. Yeung, June 20, 2020
https://github.com/yeuchi/SwiftDesignDev






