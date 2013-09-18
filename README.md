#Spark iOS Framework [![Build Status](https://magnum.travis-ci.com/epam/spark-ios-framework.png?token=o3R2wxGct9xoZkZhni3K&branch=dev)](https://magnum.travis-ci.com/epam/spark-ios-framework)
===================
Spark iOS Framework is all that you need besides UI.
Or a set of reusable components taking advantage of extra dimension [Attribute-Oriented Programming](https://en.wikipedia.org/wiki/Attribute-oriented_programming) adds.

* Source: [github.com/epam/spark-ios-framework](github.com/epam/spark-ios-framework)
* Homepage: [sparkiosframework.com](http://sparkiosframework.com)
* Twitter: [@sparkiosframework](https://twitter.com/sparkiosframework)

##Components

**Core** - support for attributes, reflection and helper-extensions on Foundation classes.  
**Observation** - unification of KVO and NSNotifications with block-based callbacks.  
**Serialization** - attribute-based JSON and XML parsers for easy DOM (de)serializations.  
**Services** - implementation of Service Locator pattern, centralized replacement for singletons.  
**Logger** - attribute-based logger.  
**Web Services** - attribute-based HTTP client API.  

##Requirements

Spark requires **iOS 5.0** and above. Compatibility with **4.3** and older is not tested.

Spark initially designed to use **ARC**. 

##Jump Start

Add `pod 'spark-ios-framework'` to your `Podfile` if you already use **CocoaPods**.

Otherwise follow next steps:

* Create a project
* Copy [`Podfile`](https://github.com/edl00k/spark-ios-framework/blob/support-pods/Cocoapods/Podfile) to the project root.

* Go to project root in terminal and nstall dependencies:

        $ pod install

*From now, use generated Xcode workspace instead of the project file only*
 
* Copy [`SparkAttributesCodeGenerator`](https://github.com/edl00k/spark-ios-framework/tree/master/tools/binaries) into new directory `binaries` in project root. It will be used for **attributes** preprocessing.

* Verify that **Run Script** with `SparkAttributesCodeGenerator` is in **"Build Phases"** before **Compile Sources** for all targets including `Pods.xcodeproj` points to valid path.

##Documentation

Documentation for all components can be found in **Documents** folder.

To use **Spark API Reference** create symlink to `Spark.docset`from documents
 
	ln -s Spark.docset ~/Library/Developer/Shared/Documentation/DocSets/Spark.docset

##License
Spark is made available under the terms of the [BSD v3](http://opensource.org/licenses/BSD-3-Clause). See the LICENSE file that accompanies this distribution for the full text of the license.





