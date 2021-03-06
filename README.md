
# WebViewANE 

WebView Adobe Air Native Extension for OSX 10.10+, Windows Desktop, iOS 9.0+ and Android21+.
This ANE provides access to a more modern webview from AIR.

Sample client included

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=5UR2T52J633RC)


## Windows
The Windows version utilises the [CefSharp WinForms](https://github.com/cefsharp/CefSharp) version of Chrome Embedded Framework.

##### Windows Installation - Important!

* Unzip the contents of cef_binaries.zip into the bin folder of your AIRSDK. 
* Copy the contents of the "cef_sharp_libs" folder into the bin folder of your AIRSDK. 
The location of this will vary depending on your IDE or. These dlls and other cef files need to reside in the folder where adl.exe is run from.
* For release builds, these files need to be packaged in the same folder as your exe
* CEF was built with MS Visual Studio 2013. As such your machine (and user's machines) will need to have Microsoft Visual C++ 2013 Redistributable (x86) runtime installed. https://github.com/cefsharp/CefSharp/wiki/Frequently-asked-questions#Including_vcredist
* This ANE was built with MS Visual Studio 2015. As such your machine (and user's machines) will need to have Microsoft Visual C++ 2015 Redistributable (x86) runtime installed. Windows 10 machines will have this but perhaps not Windows 7.
https://www.microsoft.com/en-us/download/details.aspx?id=48145
* The Cef view and processes can only be attached once to your app. Therefore only one instance can be created and used.

## OSX

The OSX version utilises the native WKWebView.


## iOS

The iOS version utilises the native WKWebView.
The iOS version is written in Swift and uses a new way of writing ANEs for iOS. See this repo for more details https://github.com/tuarua/Swift-IOS-ANE

### Running on Simulator

The example project can be run on the Simulator from IntelliJ

### Running on Device !

The example project needs to be built and signed in the correct manner.
An AIR based packaging tool is provided at https://github.com/tuarua/AIR-iOS-Packager

## Android

The Android version utilises the native WebView. 

##

![alt tag](https://raw.githubusercontent.com/tuarua/WebViewANE/master/screenshots/screenshot1.jpg)



### References
* [https://developer.apple.com/reference/webkit/wkwebview]
* [https://github.com/cefsharp/CefSharp]
