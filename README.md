# FaceSearchSDK
FaceSearchSDK by FaceX.io

# FaceSearchSDK
> FaceSearchSDK by FaceX.io in Swift

![Xcode 9.0+](https://img.shields.io/badge/Xcode-9.0%2B-blue.svg)
![iOS 10.0+](https://img.shields.io/badge/iOS-8.0%2B-blue.svg)
![Swift 4.0+](https://img.shields.io/badge/Swift-4.0%2B-orange.svg)
[![Build Status](https://travis-ci.org/TBXark/TKRadarChart.svg?branch=master)](https://travis-ci.org/TBXark/TKRadarChart)
[![CocoaPods](http://img.shields.io/cocoapods/v/TKRadarChart.svg?style=flat)](http://cocoapods.org/?q=TKRadarChart)
[![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage)
[![License MIT](https://img.shields.io/badge/license-MIT-green.svg?style=flat)](https://raw.githubusercontent.com/TBXark/TKRadarChart/master/LICENSE)


![](DemoImage/example.png)

## Requirements

- iOS 10.0+
- Xcode 9.0
- Swift 4.0

## Installation

#### CocoaPods
You can use [CocoaPods](http://cocoapods.org/) to install `FaceSearchSDK` by adding it to your `Podfile`:

```ruby
platform :ios, '10.0'
use_frameworks!
pod 'FaceSearchSDK'
```

To get the full benefits import `FaceSearchSDK` wherever you import UIKit

``` swift
import UIKit
import FaceSearchSDK
```

Congratulations!  

## Usage example



### TKRadarChartDelegate

This represents the success and errors of the FaceSearchSDK.

```swift
protocol TKRadarChartDelegate: class {
    func colorOfTitleForRadarChart(_ radarChart: TKRadarChart) -> UIColor
    func colorOfLineForRadarChart(_ radarChart: TKRadarChart) -> UIColor
    func colorOfFillStepForRadarChart(_ radarChart: TKRadarChart, step: Int) -> UIColor

    func colorOfSectionFillForRadarChart(_ radarChart: TKRadarChart, section: Int) -> UIColor
    func colorOfSectionBorderForRadarChart(_ radarChart: TKRadarChart, section: Int) -> UIColor
}
```


## Release History

* 1.0.1
  Complete  functions, add Cocoapod and Carthage support

## Meta

FaceX – [@FaceX](https://facex.io) – team@facex.io

Distributed under the license. See ``LICENSE`` for more information.

[https://github.com/FaceSearchSDK](https://github.com/FaceSearchSDK)

[swift-image]:https://img.shields.io/badge/swift-3.0-orange.svg
[swift-url]: https://swift.org/
[license-image]: https://img.shields.io/badge/License-MIT-blue.svg
[license-url]: LICENSE
[travis-image]: https://img.shields.io/travis/dbader/node-datadog-metrics/master.svg?style=flat-square
[travis-url]: https://travis-ci.org/dbader/node-datadog-metrics
[codebeat-image]: https://codebeat.co/badges/c19b47ea-2f9d-45df-8458-b2d952fe9dad
[codebeat-url]: https://codebeat.co/projects/github-com-vsouza-awesomeios-com
