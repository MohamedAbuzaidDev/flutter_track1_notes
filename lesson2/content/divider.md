# What is the Divider Widget?

**Definition:** The Divider widget in Flutter is used to create a horizontal line that visually separates content. It is commonly used in lists, forms, and sections to create clear boundaries.

**Purpose:** Helps in improving the readability of the UI by visually separating content, making the interface cleaner and more organized.

# How the Divider Works

- Divider creates a thin, horizontal line across its parent widget, typically taking up the full width.
---
- By default, it has a thickness of 1 pixel and stretches across the full width of its parent widget unless you specify a custom indent or endIndent.

```dart
Divider(
  color: Colors.black,
  thickness: 2,
  height: 50, // Height: Total vertical space taken up by the divider, including the line and padding. It's a combination of padding above and below the divider.
  indent: 20,
  endIndent: 20, // Indent and EndIndent: Define how much space is left blank on the left and right sides of the divider, respectively.
);
```

# Types

- Divider
- VerticalDivider