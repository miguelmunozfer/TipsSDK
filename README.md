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


## Handling Tips Events

To enable event handling in your application, you need to set the `eventsDelegate` of the `TipsEvents` singleton to an appropriate delegate that conforms to the `TipsEventsDelegate` protocol. Below is an example of how to set up your `ViewController` to handle these events.

### Step 1: Set the Delegate

First, ensure your `ViewController` or other appropriate class sets itself as the delegate to receive training events:

```swift
TipsEvents.shared.eventsDelegate = self

```

### Step 2: Implement the Delegate Protocol

Extend your ViewController to conform to the TipsEventsDelegate protocol. Implement the required methods to handle the events you are interested in. For example, to handle an event and print its name:

```swift
extension ViewController: TipsEventsDelegate {
    func sendEvent(_ event: TipEvent) {
        print(event.eventName ?? "")
    }
}

```

### Custom configuration
You can customize different Nutrition module interfaces using this functions:


#### Main color

Main SDK colour can be personalized. All buttons and main elements of the Nutrition module will turn the selected colour.

```swift
Tips.shared.setMainColor(color: MAIN_APP_COLOR)

```

