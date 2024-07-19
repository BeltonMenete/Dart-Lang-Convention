# Dart-Lang-Convention

This guide is my secret weapon for writing beautiful, easy-to-understand Dart code. 

## Table of Contents
1. [File Organization](#file-organization)
2. [Naming Conventions](#naming-conventions)
3. [Comments](#comments)
4. [Best Practices](#best-practices)

## File Organization

- **File Names**: Use `snake_case` for file names. Example: `my_file.dart`
- **Directory Structure**: Organize files by feature or functionality, not by type. 

<mark>Do</mark> name packages, directories, and source files using `lowercase_with_underscores` **(snake_case)**

````code
// Good
  my_package
└─ lib
   └─ file_system.dart
   └─ slider_menu.dart
````
````code
// Bad
mypackage
└─ lib
   └─ file-system.dart
   └─ SliderMenu.dart
````


## Naming Conventions

- **Classes**: Use `PascalCase` for class names. Example: `MyClass`
- **Methods and Variables**: Use `camelCase` for method and variable names. Example: `myVariable`, `calculateTotal()`
- **Constants**: Use `ALL_CAPS` with underscores for constants. Example: `MAX_COUNT`
- **Libraries**: Use `snake_case` for library names. Example: `my_library`


<mark>Do</mark> name import prefixes using `lowercase_with_underscores` **(snake_case)**

````code
// Good
import 'package:angular_components/angular_components.dart' as angular_components;

// Bad
import 'package:angular_components/angular_components.dart' as angularComponents;
````

## Comments

- **Documentation Comments**: Use `///` for documentation comments. Place them before declarations.

````dart
/// This is a documentation comment for the class.
class MyClass {
  /// This method does something.
  void doSomething() {}
}
````

## Best Practices
Avoid Globals: Minimize the use of global variables.

Error Handling: Use exceptions for error handling and provide meaningful error messages.

Avoid Deep Nesting: Refactor code to avoid deep nesting of functions and loops.

Null Safety: Make use of Dart's null safety features to prevent null reference errors.

````dart
String? nullableString;
String nonNullableString = "Hello";
Asynchronous Programming: Use async and await for asynchronous programming.
````

````dart
Future<void> fetchData() async {
  var data = await getData();
  // process data
}
````
## Conclusion
Adhering to these conventions will help maintain a high standard of code quality and readability in your Dart projects. Happy coding!

--> Feel free to adjust any part of the guide to better suit your specific needs or prefer


