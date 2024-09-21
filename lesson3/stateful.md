# What is a StatefulWidget?

**Definition:** A StatefulWidget is a widget in Flutter that can maintain state across its lifecycle. It is used when the UI needs to change dynamically based on user input or other factors.

## Example

```dart
class MyStatefulWidget extends StatefulWidget {
  @override
  _MyStatefulWidgetState createState() => _MyStatefulWidgetState();
}

class _MyStatefulWidgetState extends State<MyStatefulWidget> {
  @override
  Widget build(BuildContext context) {
    return Container();
  }
}
```

# Understanding State and StatefulWidget

- The StatefulWidget itself is immutable, meaning it doesn’t change, but its state can.

- The mutable part of a StatefulWidget is handled by a separate State class, which maintains the widget's state over time.

- A StatefulWidget consists of two parts:

    - **The widget:** Defines the structure of the UI.
    - **The state:** Contains mutable data that can change during the widget's lifetime.

# Lifecycle of a StatefulWidget

1. **createState():**
   
   - Called when the StatefulWidget is created. It returns an instance of the State class.
  
   - Example:
```dart
@override
_MyStatefulWidgetState createState() => _MyStatefulWidgetState();
```

2. **initState():**

    - Called once when the state object is created. This is where you can initialize data or set up listeners.

    - Example:
```dart
@override
void initState() {
  super.initState();
  // Initialization logic here
}
```

3. **build():**

    - Called every time the state changes or is rebuilt. This method constructs the UI.
  
    - Example:
```dart
@override
Widget build(BuildContext context) {
  return Container();
}
```

4. **setState():**

    - The core function of the StatefulWidget. Whenever you want to update the UI, you call setState(). This triggers a rebuild of the widget tree with the updated state.

    - Example:

```dart
void updateUI() {
  setState(() {
    // Update the state variables
  });
}
```

5. **dispose():**

    - Called when the widget is permanently removed from the widget tree. You can clean up resources here (e.g., closing streams, stopping timers).

    - Example:

```dart
@override
void dispose() {
  // Clean up resources
  super.dispose();
}
```

# Key Differences Between StatelessWidget and StatefulWidget

- **StatelessWidget:** Used for widgets that don’t need to change after being built.

- **StatefulWidget:** Used when the widget needs to update its UI based on user interaction or other factors.

| **Aspect**           | **StatelessWidget**               | **StatefulWidget**                |
|----------------------|-----------------------------------|-----------------------------------|
| **State Management**  | No internal state                | Manages internal state            |
| **UI Updates**        | Doesn't change after build        | Can change during its lifetime    |
| **Performance**       | Lightweight                      | Slightly heavier due to state     |