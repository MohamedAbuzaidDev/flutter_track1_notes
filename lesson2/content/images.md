# Overview of the Image Widget

**Definition:** The `Image` widget in Flutter is used to display images in your app. It can display images from multiple sources like assets, the network, or files.

**Purpose:** It's an essential widget for adding visuals to your app, making the UI more engaging and informative.

# Types of Image Sources

## Image from Assets (Image.asset):

- Used for displaying images packaged with your app.
- Example:

```dart
Image.asset(
  'assets/images/logo.png',
  width: 100,
  height: 100,
  fit: BoxFit.cover,
);
```

- Always declare images in the `pubspec.yaml` under the assets section to ensure they are bundled with the app:

```yaml
flutter:
  assets:
    - assets/images/logo.png
```

- you can declare the folder containing images:

```yaml
flutter:
  assets:
    - assets/images/
```

## Image from Network (Image.network):

- Used for loading images from a URL.
- Example:

```dart
Image.network(
  'https://example.com/image.jpg',
  width: 150,
  height: 150,
  fit: BoxFit.cover,
)
```