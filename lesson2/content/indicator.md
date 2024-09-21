# What Are Indicators in Flutter?

**Definition:** In Flutter, spinners are visual indicators used to show that a task is in progress or that the app is waiting for an action to complete.

**Purpose:** To inform the user that an operation (e.g., data fetching, file uploading, or loading a new screen) is ongoing, which prevents confusion and improves the user experience.

# Types of Progress Indicators in Flutter

## CircularProgressIndicator

```dart
CircularProgressIndicator(
  valueColor: AlwaysStoppedAnimation<Color>(Colors.blue),
  strokeWidth: 6.0,
  backgroundColor: Colors.grey[200],
);
```

```dart
// Determinate Progress Example
CircularProgressIndicator(
  value: 0.7, // 70% progress
  valueColor: AlwaysStoppedAnimation<Color>(Colors.green),
);
```


## LinearProgressIndicator

```dart
LinearProgressIndicator(
  valueColor: AlwaysStoppedAnimation<Color>(Colors.red),
  backgroundColor: Colors.grey[300],
  minHeight: 10,
);
```

```dart
// Determinate Progress Example
LinearProgressIndicator(
  value: 0.5, // 50% progress
  valueColor: AlwaysStoppedAnimation<Color>(Colors.green),
  backgroundColor: Colors.grey[200],
);
```

# Indeterminate vs Determinate Progress Indicators

**Indeterminate:** The indicator displays a continuous animation because the duration of the process is unknown. It tells the user that something is happening but doesn’t provide progress information.

**Determinate:** The indicator shows a measurable amount of progress, often used for file uploads, downloads, or any operation with a known completion percentage.