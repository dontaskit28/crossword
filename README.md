# NEW:  Transpose Matrix feature added
# Crossword [![pub package](https://img.shields.io/pub/v/crossword.svg)](https://pub.dartlang.org/packages/crossword)

<br>
<p align="center">
<img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/m/amonc/crossword">
<img alt="GitHub contributors" src="https://img.shields.io/github/contributors/amonc/crossword">
<img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/amonc/crossword?style=social">
<img alt="GitHub" src="https://img.shields.io/github/license/amonc/crossword">
<img alt="Pub Version" src="https://img.shields.io/pub/v/crossword">
<img alt="Pub Likes" src="https://img.shields.io/pub/likes/crossword">
<img alt="Pub Points" src="https://img.shields.io/pub/points/crossword">
<img alt="Pub Popularity" src="https://img.shields.io/pub/popularity/crossword">

</p>

</br>

`Crossword` is a comprehensive solution for seamlessly integrating a crossword puzzle-solving user interface into your Flutter app. With this package, you can effortlessly provide users with an interactive and enjoyable crossword puzzle-solving experience within your application.

<img src="https://github.com/Amonc/crossword/assets/23643271/a2abcac4-2540-4e46-b398-366265c5fbc2" width="270">

## Features

- **Customizable Crossword Widget:**
  The package offers a customizable crossword widget that can be easily integrated into any Flutter app. You can adjust the widget's appearance, size, and layout to match your app's design and theme.

- **User-Friendly Interface:**
  The user interface is designed with simplicity and ease of use in mind. Users can intuitively navigate through the puzzle, pan, and select the letters to choose words.
  
- **Clue Management:**
  Manage crossword clues effortlessly with this package by passing the list of words into the `Crossword` widget.

## Getting started

## Installation

You just need to add `crossword` as a [dependency in your pubspec.yaml file](https://flutter.io/using-packages/).

```yaml
dependencies:
  crossword: ^0.0.5
```

Import the package in your Dart code and instantiate the `Crossword` widget.

## Example

To get started add the `Crossword` widget. 
- `letters` : takes all the letters as a two-dimentional `List`
- `spacing` : controls the `horizontal` and `vertical` spacing in between letters
- `onLineDrawn` : returns a `List` of words created based on user interactions on the `Crossword panel`
- `hints` : takes a `List` of words as clues

```dart
Crossword(
          letters: letters:[
                    ["F", "L", "U", "T", "T", "E", "R", "W", "U", "D", "B", "C"],
                    ["R", "M", "I", "O", "P", "U", "I", "Q", "R", "L", "E", "G"],
                    ["T", "V", "D", "I", "R", "I", "M", "U", "A", "H", "E", "A"],
                    ["D", "A", "R", "T", "N", "S", "T", "O", "Y", "J", "R", "M"],
                    ["O", "G", "A", "M", "E", "S", "C", "O", "L", "O", "R", "O"],
                    ["S", "R", "T", "I", "I", "I", "F", "X", "S", "P", "E", "D"],
                    ["Y", "S", "N", "E", "T", "M", "M", "C", "E", "A", "T", "S"],
                    ["W", "E", "T", "P", "A", "T", "D", "Y", "L", "M", "N", "U"],
                    ["O", "T", "E", "H", "R", "O", "G", "P", "T", "U", "O", "E"],
                    ["K", "R", "R", "C", "G", "A", "M", "E", "S", "S", "T", "S"],
                    ["S", "E", "S", "T", "L", "A", "O", "P", "U", "P", "E", "S"]
          ],
          spacing: const Offset(30, 30),
          onLineDrawn: (List<String> words) {},
          hints: const ["Flutter", "Dart", "Games", "Colors"],
        )
```

## Additional parameters
- `acceptReversedDirection`: accepts a `bool` to identify while creating the words by touching in the reversed direction, is enabled or not
- `drawCrossLine`:  accepts a `bool`, and identifies if the user can interact in the `Cross` direction or not.
- `drawVerticalLine`:  accepts a `bool`, and identifies if the user can interact in the `Vertical` direction or not. 
- `drawHorizontalLine`: accepts a `bool`, and identifies if the user can interact in the `Horizontal` direction or not.
  
> `drawCrossLine`, `drawVerticalLine`, `drawHorizontalLine` can't be set as `false` altogether.

- `lineDecoration`: Decorate lines to update colors based on the input and clues
- `textStyle`: Add styles to the crossword letters
- `transposeMatrix`: Transpose the 2x2 matrix



