# Recipe App -- Flutter Assignment

## Assignment Question

Parse the provided JSON containing a list of food recipes and display
the recipe titles in a `ListView` widget in Flutter.

**Focus on:** - JSON parsing - Data modelling - UI rendering

## Provided JSON

``` json
{
  "recipes": \[
    {
      "title": "Pasta Carbonara",
      "description": "Creamy pasta dish with bacon and cheese.",
      "ingredients": \["spaghetti", "bacon", "egg", "cheese"]
    },
    {
      "title": "Caprese Salad",
      "description": "Simple and refreshing salad with tomatoes, mozzarella, and basil.",
      "ingredients": \["tomatoes", "mozzarella", "basil"]
    },
    {
      "title": "Banana Smoothie",
      "description": "Healthy and creamy smoothie with bananas and milk.",
      "ingredients": \["bananas", "milk"]
    },
    {
      "title": "Chicken Stir-Fry",
      "description": "Quick and flavorful stir-fried chicken with vegetables.",
      "ingredients": \["chicken breast", "broccoli", "carrot", "soy sauce"]
    },
    {
      "title": "Grilled Salmon",
      "description": "Delicious grilled salmon with lemon and herbs.",
      "ingredients": \["salmon fillet", "lemon", "olive oil", "dill"]
    },
    {
      "title": "Vegetable Curry",
      "description": "Spicy and aromatic vegetable curry.",
      "ingredients": \["mixed vegetables", "coconut milk", "curry powder"]
    },
    {
      "title": "Berry Parfait",
      "description": "Layered dessert with fresh berries and yogurt.",
      "ingredients": \["berries", "yogurt", "granola"]
    }
  ]
}
```

## Project Overview

This Flutter application demonstrates how to decode JSON data, convert
each recipe into a Dart model object, and display the recipe titles in a
scrollable `ListView`.

## Features

* Parses the provided JSON string using `jsonDecode()` from
`dart:convert`.
* Defines a `Recipe` data model.
* Uses a `fromJson()` factory constructor to create `Recipe` objects.
* Displays all seven recipe titles with `ListView.builder()`.

## Project Structure

``` text
lib/
├── main.dart
├── models/
│   └── recipe.dart
└── data/
    └── recipe\_data.dart
```

## Implementation Summary

1. **JSON parsing:** `jsonDecode()` converts the JSON string into Dart
data.
2. **Data modelling:** `Recipe.fromJson()` maps each JSON recipe to a
strongly typed `Recipe` object.
3. **UI rendering:** `ListView.builder()` builds a list item for each
recipe and displays its title.

## How to Run

Make sure Flutter is installed and a device or emulator is available.
From the project root, run:

``` bash
flutter pub get
flutter run
```

To check the project for analyzer issues, run:

``` bash
flutter analyze
```

## Expected Output

The app displays these seven recipe titles in a scrollable list:

1. Pasta Carbonara
2. Caprese Salad
3. Banana Smoothie
4. Chicken Stir-Fry
5. Grilled Salmon
6. Vegetable Curry
7. Berry Parfait

## Technologies Used

* Flutter
* Dart
* JSON
* `dart:convert`

## Author

shafin-23

