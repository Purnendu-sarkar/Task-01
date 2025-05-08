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


## 🔹 2. What is type inference in TypeScript? Why is it helpful?

### What is type inference in TypeScript?
Type inference is a feature of TypeScript where the compiler automatically determines the type of a variable or expression without you explicitly specifying it.


### Why is Type Inference Helpful?
Less code: You write fewer type annotations

Smarter tooling: IDEs can suggest completions based on inferred types

Error prevention: Catch mistakes early without manually defining types

Faster development: Makes code easier to write and maintain
