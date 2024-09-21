# What is the Spacer Widget?

**Definition:** The Spacer widget is used to create adjustable, flexible empty space between widgets in a `Row`, `Column`, or `Flex`. It helps in distributing space efficiently between widgets without hardcoding margins or paddings.

**Purpose:** It allows for flexible layout design where space can be dynamically adjusted between or around widgets, ensuring a responsive UI.

# Examples

```dart
Row(
  children: [
    Icon(Icons.home),
    Spacer(),
    Icon(Icons.search),
  ],
);
```

```dart
Row(
  children: [
    Icon(Icons.home),
    Spacer(flex: 2), // Takes twice the space
    Icon(Icons.search),
    Spacer(flex: 1), // Takes one unit of space
    Icon(Icons.settings),
  ],
);
```