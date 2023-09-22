# TipsSDK

[![CI Status](https://img.shields.io/travis/Miguel/VitaleSDK.svg?style=flat)](https://travis-ci.org/Miguel/VitaleSDK)
[![Version](https://img.shields.io/cocoapods/v/VitaleSDK.svg?style=flat)](https://cocoapods.org/pods/VitaleSDK)
[![License](https://img.shields.io/cocoapods/l/VitaleSDK.svg?style=flat)](https://cocoapods.org/pods/VitaleSDK)
[![Platform](https://img.shields.io/cocoapods/p/VitaleSDK.svg?style=flat)](https://cocoapods.org/pods/VitaleSDK)

## Description
TipsSDK is a set of useful tips framework programmed in Swift for iOS and iPadOS.

## Installation

TipsSDK is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'TipsSDK', :git => 'https://github.com/miguelmunozfer/TipsSDK'
```


## Usage

### Simple 1-line setup

```swift
Tips.shared.showTips()

```

### Custom configuration
You can customize different Nutrition module interfaces using this functions:


#### Main color

Main SDK colour can be personalized. All buttons and main elements of the Nutrition module will turn the selected colour.

```swift
Tips.shared.setMainColor(color: MAIN_APP_COLOR)

```

