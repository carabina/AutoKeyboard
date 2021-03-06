# AutoKeyboard for iOS written in Swift 3.0

Automatic Keyboard handling with ease. It is fully automatic keyboard handling. Like in android no need to resize views when keyboard appears. It updates constraints which are bounded with `bottomLayoutGuide`. Feels like `bottomLayoutGuide` moves UP and DOWN with keyboard. Just need to `register` and `unResgister` thats it.

## []()
![alt tag](https://github.com/chanonly123/AutoKeyboard/blob/master/demo.gif)

## Features
- UIViewController extension, no need to extend classes.
- Device rotation supported.
- Multiple UIViewController support.
- Extremely easy integration.
- Automatic bottom constraints changes with keyboard
- Resizing with animation.
- No need to write extra code.
- Just `registerAutoKeyboard ` and `unRegisterAutoKeyboard `

## Runtime Requirements

- iOS8.0 or later
- Xcode 8.0 - Swift 3.0 or later

## Usage
![Alt text](https://github.com/chanonly123/AutoKeyboard/blob/master/help.png)<br />
- Add constrainsts to `bottomLayoutGuide` and they will update when keyboard appears.
- And Register your specific ViewController, you should also unregister.
```
    override func viewWillAppear(_ animated: Bool) {
        registerAutoKeyboard()
    }
    
    override func viewWillDisappear(_ animated: Bool) {
        unRegisterAutoKeyboard()
    }
```
## Installing
### CocoaPods
To integrate AutoKeyboard into your Xcode project using CocoaPods, specify it in your `Podfile` and run `pod install`.
```bash
platform :ios, '8.0'
use_frameworks!
pod 'AutoKeyboard'
```
And `import AutoKeyboard`
### Carthage
Coming soon

## Contributing

Contributions are always welcome!
Contact `chan.only.123@gmail.com`

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Inspired by [IQKeyboardManager](https://github.com/hackiftekhar/IQKeyboardManager)
* Motivated by [KeyboardObserver](https://github.com/morizotter/KeyboardObserver)
