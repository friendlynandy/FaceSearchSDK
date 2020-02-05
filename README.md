# FaceSearchSDK
FaceSearchSDK by FaceX.io

# FaceSearchSDK
> FaceSearchSDK by FaceX.io in Swift

![Xcode 9.0+](https://img.shields.io/badge/Xcode-9.0%2B-blue.svg)
![iOS 10.0+](https://img.shields.io/badge/iOS-8.0%2B-blue.svg)
![Swift 4.0+](https://img.shields.io/badge/Swift-4.0%2B-orange.svg)
[![CocoaPods](http://img.shields.io/cocoapods/v/FaceSearchSDK.svg?style=flat)](http://cocoapods.org/?q=FaceSearchSDK)
[![Updated](https://img.shields.io/github/last-commit/friendlynandy/FaceSearchSDK)](https://img.shields.io/github/last-commit/friendlynandy/FaceSearchSDK)
[![Licence](https://img.shields.io/cocoapods/l/FaceSearchSDK?color=red&logo=red)](https://img.shields.io/cocoapods/l/FaceSearchSDK?color=red&logo=red)


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

###### To get the full benefits import `FaceSearchSDK` wherever you import UIKit

``` swift
import UIKit
import FaceSearchSDK
```

##### Get `FaceSearchSDK.plist` from Facex.io user dashboard and add it to your project to start using.

Congratulations!  

### Usage example

#### Outdoor Mode (Automatic detection and result)
```swift

    let faceSearch = FaceSearch()
    faceSearch.delegate = self
    faceSearch.startOutdoorMode()
    
```
#### Manual Usage
```swift

    let faceSearch = FaceSearch()
    faceSearch.delegate = self
    
    

        faceS.searchFaceInDBWithImage(image:YOUR_IMAGE) { (responce, error) in
                 // Do your stuff   
        }
        
        faceS.addPersonToDBWithAdminApproval(name: "NAME", image: YOUR_IMAGE) { (suucess, error) in
                // Do your stuff
        }
        
        faceS.addPersonToDBForApproval(image: YOUR_IMAGE) { (suucess, error) in
                // Do your stuff
        }

```


### FaceSearchDelegate

This represents the success and errors of the FaceSearchSDK.

```swift
protocol FaceSearchDelegate: class {

    func faceSearchPersonDetectedDelegate(responce:NSDictionary, error:NSError?)
    
    func faceSearchErrorDelegate(error:NSError)
    
}
```


## Release History

* 1.0.1
  Complete  functions, add Cocoapod and Carthage support

## Meta

FaceX – [@FaceX](https://facex.io) – team@facex.io

Distributed under the license. See ``LICENSE`` for more information.

[https://github.com/FaceSearchSDK](https://friendlynandy.github.io/FaceSearchSDK/)

[swift-image]:https://img.shields.io/badge/swift-3.0-orange.svg
[swift-url]: https://swift.org/
[license-image]: https://img.shields.io/cocoapods/l/FaceSearchSDK?color=red&logo=red
[license-url]: LICENSE
