# TFTransparentNavigationBar

[![CI Status](http://img.shields.io/travis/Ales Kocur/TFTransparentNavigationBar.svg?style=flat)](https://travis-ci.org/Ales Kocur/TFTransparentNavigationBar)
[![Version](https://img.shields.io/cocoapods/v/TFTransparentNavigationBar.svg?style=flat)](http://cocoapods.org/pods/TFTransparentNavigationBar)
[![License](https://img.shields.io/cocoapods/l/TFTransparentNavigationBar.svg?style=flat)](http://cocoapods.org/pods/TFTransparentNavigationBar)
[![Platform](https://img.shields.io/cocoapods/p/TFTransparentNavigationBar.svg?style=flat)](http://cocoapods.org/pods/TFTransparentNavigationBar)

![preview](https://github.com/thefuntasty/TFTransparentNavigationBar/blob/master/Example/TFTransparentNavigationBar/preview.gif)

## Usage

In order to make transparent navigation bar you need set your navigation controller class to TFNavigationController. Then in your controllers implement TFTransparentNavigationBarProtocol which has only one method `navigationControllerBarPushStyle() -> TFNavigationBarStyle`. You have to return if your bar should be `.Solid` or `.Transparent`. The default style is .Solid therefore you can implement the protocol only for controllers you want to have a transparent bar. 

## Requirements

iOS 8 and later, Swift 2.0. No Apple-private API used.

## Known bugs

- ~~Navigation bar keeps title during pop transition FIXED (but still problem with interactive transition)~~
- ~~First transition to controller with transparent navbar moves with fromView frame~~
- ~~Setting a VC with `.Transparent` as a root VC for an instance of `TFNavigationController` doesn't make the navigation bar transparent~~
- Simple crossfade animation is applied to the navigation bar: http://stackoverflow.com/a/21614376/1161723

## Installation

TFTransparentNavigationBar is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod "TFTransparentNavigationBar"
```

## Author

Ales Kocur, ales@thefuntasty.com

## License

TFTransparentNavigationBar is available under the MIT license. See the LICENSE file for more info.
