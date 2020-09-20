# Sign In Button

A Flutter plugin for generating sign in buttons for different social media accounts.

dart.pub = https://pub.dev/packages/sign_button

## Getting Started

You must add the library as a dependency to your project.
```yaml
dependencies:
 sign_button: ^0.0.9
```

You should then run `flutter packages get`

Now in your Dart code, you can use:

```dart
import 'package:sign_button/sign_button.dart'
```

## Usage Example

It very simple!

```dart
SignInButton(
  buttonType: ButtonType.google,
  onPressed: () {
   print('click');
  })
```

<img src = "https://github.com/emreesen27/Flutter-Sign-Button/blob/assets/btns.png?raw=true">

ButtonSize
```dart
SignInButton(
  buttonType: ButtonType.google,
  buttonSize: ButtonSize.large, // small(default), medium, large
  onPressed: () {
   print('click');
  })
```
<img src = "https://github.com/emreesen27/Flutter-Sign-Button/blob/assets/size.png?raw=true">

ImagePosition
```dart
SignInButton(
  imagePosition: ImagePosition.left, // left or right
  buttonType: ButtonType.google,
  onPressed: () {
   print('click');
  })
```
<img src = "https://github.com/emreesen27/Flutter-Sign-Button/blob/assets/position.png?raw=true">

```dart
SignInButton(
 buttonType: ButtonType.pinterest,
 imagePosition: ImagePosition.right,
 //[buttonSize] You can also use this in combination with [width]. Increases the font and icon size of the button.
 buttonSize: ButtonSize.large,
 btnTextColor: Colors.grey,
 btnColor: Colors.white,
 width: 140,
 //[width] Use if you change the text value.
 btnText: 'Pinterest',
 onPressed: () {
  print('click');
 })
```

<img src = "https://github.com/emreesen27/Flutter-Sign-Button/blob/assets/custom.png?raw=true">


## Other properties
- btnText 
- btnColor
- btnTextColor
- elevation
- width // You can change the value of width when the text size becomes too small.
- padding // padding value is automatically adjusted according to the button size. You can give a value if you want.
