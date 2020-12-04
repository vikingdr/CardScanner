# CardScanner

## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.

|   |   |   |
|---|---|---|
|![](Screenshots/sample.gif)|![](Screenshots/sample2.gif)|![](Screenshots/sample3.gif)|



## Requirements

- iOS 13 or newer
- Swift 5

## Installation

CardScanner is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'CardScanner'
```

To Use:


```Swift
import CardScanner 
```

And simple call 

```Swift
let scannerView = CardScanner.getScanner { card, date, cvv in
    self.resultsLabel.text = "\(card) \(date) \(cvv)"
}
present(scannerView, animated: true, completion: nil)
```

Currently working with:
- Number 15 or 16 digits
- CVV 3 digits
- Date MM/YYYY or MM/YY



Do not forget add `NSCameraUsageDescription` to your Info.plist

You can custom the texts using the scannerView.:

- hintTopText
- hintBottomText
- buttonConfirmTitle
- buttonConfirmBackgroundColor

## Author

Matthew James, matt@vikingdr.com

If do you like, give your ⭐️

## License

CardScanner is available under the MIT license. See the LICENSE file for more info.
