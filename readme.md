# 1. Difference Between any, unknown, and never Types

### `any`
- Allows assignment of any value and calling any method
- Should be avoided when possible as it defeats TypeScript's type safety

### `unknown`
- Requires type checking before performing operations
- Good for values of unknown type that need verification

### `never`
- Represents values that should never occur
- Used for functions that always throw or never return

---

# 2. What is the use of enums in TypeScript? Provide an example of a numeric and string enum.

## Use of Enums in TypeScript
Enums allow a developer to define a set of named constants. Using enums can make it easier to document intent, or create a set of distinct cases. TypeScript provides both numeric and string-based enums.

### Numeric Enum
enum Direction {
  Up,      // 0
  Down,    // 1
  Left,    // 2
  Right    // 3
}

let move: Direction = Direction.Left;
console.log(move); // Output: 2

### String Enums
enum Color {
  Red = "RED",
  Green = "GREEN",
  Blue = "BLUE"
}

let favorite: Color = Color.Green;
console.log(favorite); // Output: "GREEN"
