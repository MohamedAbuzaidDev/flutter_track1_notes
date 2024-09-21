# What are Row and Column in Flutter?

- **Definition:**
    - **Row:** Arranges its children horizontally in a line.
    - **Column:** Arranges its children vertically in a line.

- **Purpose:** They are the primary widgets for arranging multiple child widgets either horizontally or vertically, making them foundational building blocks for any UI.

# Understanding Layout Behavior

- **Main Axis:**
    - **For a Row**, the main axis is horizontal.
    - **For a Column**, the main axis is vertical.

- **Cross Axis:**
    - **For a Row**, the cross axis is vertical.
    - **For a Column**, the cross axis is horizontal

# Key Properties of Row & Column

```dart
Row(
    mainAxisAlignment: MainAxisAlignment.start,
    crossAxisAlignment: CrossAxisAlignment.start,
    mainAxisSize: MainAxisSize.max,
    children: [
        Text('Item 1'),
        Text('Item 2'),
        Text('Item 3'),
    ],
);
```