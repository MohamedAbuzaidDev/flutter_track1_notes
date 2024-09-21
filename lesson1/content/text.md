# EX 1

**props:** style, textAlign, textDirection, overflow, maxLines, textScaler

```dart
Text('Text 1', 
  style: TextStyle(
    fontSize: 30,
  ),
  textAlign: TextAlign.center,
  textScaler: TextScaler.linear(1.5),
)
```

# EX 2

```dart
DefaultTextStyle(
  style: TextStyle(
    fontSize: 40,
    color: Colors.red
  ), 
  child: Column(
    mainAxisAlignment: MainAxisAlignment.center,
    children: [
      Icon(Icons.home, size: 30,),
      Text('Text 2')
    ],
  )
)
```

# EX 3

```dart
RichText(
  text: const TextSpan(
    text: 'Hello ',
    style: TextStyle(
      fontSize: 24, 
      color: Colors.black
    ),
    children: <TextSpan>[
      TextSpan(
        text: 'Flutter', 
        style: TextStyle(
          fontWeight: FontWeight.bold, 
          color: Colors.red
        )
      ),
      TextSpan(text: '!'),
    ],
  ),
)
```

# EX 4

```dart
RichText(
  text: const TextSpan(
    children: [
      TextSpan(
        text: 'Home ', 
        style: TextStyle(
        fontSize: 30
        )
      ),
      WidgetSpan(
        child: Icon(
          Icons.home, 
          size: 24
        ),
      ),
    ],
  ),
)
```