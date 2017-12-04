# TsubameVIPER

## How to install

### Using script (easy) 
Only need execute this command in terminal:
```swift
sudo swift install.swift
```

If all it's ok you now could find your template in Xcode.

### Manual
Go to Application folder, browse to the Xcode application icon. Right-click it and choose 'Show Package Contents'. Then browse to:

`Contents/Developer/Platforms/iPhoneOS.platform/Developer/Library/Xcode/Templates/Project Templates/iOS` and add "TsubameVIPER" folder. Now you can find your template in Xcode.

## Generated code
This template generates all files that you need to create a new VIPER module in **protocol oriented** manner.

Unlike many other Viper template, this template encourages you to strictly apply the dependency rule between
`View` -> `Presenter` -> `Interactor` -> `Entity`,  `Presenter` -> `Router`, which means that the outer layers should depend on inner layers while inner layers neither see nor know about, nor are aware of, outer layers.
(eg. `View` only sees `Presenter`, `Presenter` only sees `Interactor` and `Router`, `Interactor` only sees `Entity`)

The feedback from inner layers to outlayers can be achieved by **closures, notifications or Rx observables**.

## Other VIPER MODULE GENERATORS

**Swift-VIPER-Module**: Generate Protocol oriented Viper modules. It also allows you to divide interactor into (input & output). Our current installation script is based on the installation script provided in this repository.  https://github.com/Juanpe/Swift-VIPER-Module

## References: 
**Clean Architecture**: This serie of tutorial is written for Android platform. But the core principle of clean architecture on dependency rule, abstraction and communication between layers can be shared on iOS platform as well.  http://five.agency/android-architecture-part-2-clean-architecture/ 

## Code Example: 
**TO DO**: An example app will be provided shorted to highlight the approach of closure driven VIPER architecture in iOS.
