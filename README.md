# FutureKit
A Swift based Future/Promises Library for IOS and OS X.   


FutureKit is a iOS implementation of Futures and Promises, but modified specifically for iOS/OSX programmers.

FutureKit sues Swift generic classes, to allow you to easily deal with asynchronous/multi-threaded issues when coding for iOS or OSX.

- is 100% Swift.  And supports Swift 1.2 and XCode 6.3.

- is type safe.  It uses Swift Generics classes that can automatically infer the type you wish to return from asynchronous logic.  And supports all Swift types (Both 'Any' types, and 'AnyObject/NSObject' types!)

- uses simple to understand methods (onComplete/onSuccess/onFail etc) that let's you simplify complex asynchronous operations into clear and simple to understand logic.

- is highly composable, since any existing Future can be used to generate a new Future.  And Errors can be automatically passed through, simplifying error handling logic.

- works well editing code within XCode 6.3 auto-completion.  The combination of type-inference and code-completion makes FutureKit coding fast and easy.

- simplifies the use of Apple GCD by using Executors - a simple Swift enumeration that attracts the most common iOS/OSX Dispatch Queues (Main,Default,Background, etc).  Allowing you to guarantee that logic will always be executed in the context you want.  (You never have to worry about having to call the correct dispatch_async() function again).  

- is highly tunable, allowing you to configure how the primary Executors (Immediate vs Async) execute, and what sort Thread Synchronization FutureKit will use (Barriers - Locks, etc).  Allowing you to tune FutureKit's logic to match what you need.  



# Documentation

FutureKit documentation is being written as XCode Playgrounds.  The best way to start is to open the FutureKit.workspace and then opening the Playground inside.  (If you open the Playgrounds outside of the workspace, then FutureKit module may not import correctly).
The XCode Playgrounds probably require XCode 6.3 (in order to see the Markup correctly)

If you are impatient, or not near your copy of XCode, you can try to read the first intro "raw" playground here:
https://github.com/FutureKit/FutureKit/blob/master/FutureKit-Future.playground/Contents.swift

There is also docs directory, that is generated using jazzy. https://github.com/realm/jazzy and the embedded documentation.  The plan is to get as close to 100% as possible (We are at 20%!).  So currently there is a lot of missing documentation.





