# TypeScript Blog

## 🔹 1.What is the use of enums in TypeScript? Provide an example of a numeric and string enum.

### What is an Enum?

Enums (short for enumerations) in TypeScript allow us to define a set of named constants. They are useful when we have a fixed set of values that a variable can take, such as days of the week, roles in a system, or statuses. Enums make the code more readable and type-safe by restricting the values to a predefined list.

### Why Use Enums?

- Readability: Enums give meaningful names to values, making the code easier to understand.
- Type Safety: TypeScript ensures that only valid enum values are used, reducing errors.
- Organization: Enums group related constants together, improving code structure.

### 🔸 Numeric Enum Example:

```typescript
enum Day {
  Monday,    // 0
  Tuesday,   // 1
  Wednesday, // 2
  Thursday,  // 3
  Friday,    // 4
  Saturday,  // 5
  Sunday     // 6
}

const today: Day = Day.Monday;
console.log(today); // Output: 0
console.log(Day[today]); // Output: "Monday"

###🔸 String Enum Example:
enum Role {
  Admin = "ADMIN",
  User = "USER",
  Guest = "GUEST"
}

const userRole: Role = Role.Admin;
console.log(userRole); // Output: "ADMIN"


```
