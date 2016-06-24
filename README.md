# Rxswift MVVM Architecture

# Swfit code style
[github version](https://github.com/github/swift-style-guide)

[raywenderlich.com version](https://github.com/raywenderlich/swift-style-guide)

[netguru version](https://github.com/netguru/swift-style-guide)

[Linkin version](https://github.com/linkedin/swift-style-guide)

# MVVM
The architecture of our ios apps is based on the [MVVM] (https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93viewmodel)

* __View (UI layer)__: This is where view, viewController, and other native components, also handles user interactions and inputs. The View is rather synchronized with the viewmodel, active and contains behaviors, events and data binding information.

* __ViewModel__: The viewmodel in MVVM is responsible for presentation separation and exposes methods and commands to manage the state of a view and manipulate the model.

* __Model (Data Layer)__:this is responsible for retrieving, saving, caching and massaging data. It can communicate with local databases and other data stores as well as with restful APIs or third party SDKs.


![MVVM](https://upload.wikimedia.org/wikipedia/commons/thumb/8/87/MVVMPattern.png/660px-MVVMPattern.png)

![MVVM](http://cases.azoft.com/images/2015/12/pattern-mvvm-scheme.png)

![MVVM](http://www.sprynthesis.com/assets/images/MCVMVMV.gif)

# Project Structure

```
SampleApp
├── App
│   └── AppDelegate
├── Enums
├── Extensions
├── Externals
├── Globals
├── Helpers
├── Models
├── Networking
├── Protocols
├── Resources
│   ├── LaunchScreen.storyboard
│   ├── Localizable.strings
│   └── Info.plist
├── Structs
├── ViewControllers
├── ViewModels
└── Views
```

## Dependencies

- [Moya](https://github.com/Moya/Moya): Network abstraction layer written in Swift.
- [Kingfisher](https://github.com/onevcat/Kingfisher): A lightweight and pure Swift implemented library for downloading and caching image from the web.
- [ObjectMapper](https://github.com/Hearst-DD/ObjectMapper): Simple JSON Object mapping written in Swift
- [Moya-ObjectMapper](https://github.com/ivanbruel/Moya-ObjectMapper):(optional) ObjectMapper bindings for Moya and RxSwift
- [Moya-ModelMapper](https://github.com/sunshinejr/Moya-ModelMapper):(optional) bindings for Moya for easier JSON serialization with RxSwift and ReactiveCocoa bindings
- [SwiftyJSON](https://github.com/SwiftyJSON/SwiftyJSON):(optional) SwiftyJSON makes it easy to deal with JSON data in Swift.
- [RxSwift](https://github.com/ReactiveX/RxSwift): Reactive Programming in Swift
- [RxCocoa](https://github.com/ReactiveX/RxSwift/tree/master/RxCocoa/iOS): A bundle with common-usage iOS reactive extensions.
- [NSObject+Rx](https://github.com/RxSwiftCommunity/NSObject-Rx): Handy RxSwift extensions on NSObject, including rx_disposeBag.
- [RxOptional](https://github.com/RxSwiftCommunity/RxOptional): RxSwift extensions for Swift optionals and "Occupiable" types.
- [KeychainSwift](https://github.com/marketplacer/keychain-swift): Helper functions for saving text in Keychain securely for iOS, OS X, tvOS and watchOS.
- [Result](https://github.com/antitypical/Result): This is a Swift µframework providing Result<Value, Error>.
- [Device](https://github.com/Ekhoo/Device): Device detect the current  device model and screen size.
- [Cell-Rx](https://github.com/ivanbruel/Cell-Rx): Cell+Rx provides a similar API to NSObject+Rx but for cells who are reused along the way.

Unit Test

- [Quick](https://github.com/Quick/Quick): Quick is a behavior-driven development framework for Swift and Objective-C.
- [Nimble](https://github.com/Quick/Nimble): Use Nimble to express the expected outcomes of Swift or Objective-C expressions.
- [RxBlocking](https://github.com/ReactiveX/RxSwift/tree/master/RxBlocking): Set of blocking operators for easy unit testing.
- [RxTests](https://github.com/ReactiveX/RxSwift/tree/master/RxTests): 


# Xcode Plugin

- [XAlign] (https://peterwitham.com/xcode/xcode-plugin-xalign/)
- [Swimat] (https://github.com/Jintin/Swimat)

# Reference

- http://www.sprynthesis.com/2014/12/06/reactivecocoa-mvvm-introduction/
- https://github.com/ReactiveX/RxSwift
- https://github.com/tailec/boilerplate
- https://github.com/DroidsOnRoids/RxSwiftExamples
- https://github.com/ivanbruel/Reddit-MVVM-Benchmark
- https://github.com/tryswift/RxPagination
