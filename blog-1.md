# Why `any` is Called a Type Safety Hole and Why `unknown` is Safer in TypeScript

## Introduction

TypeScript is popular because it helps developers write safer and more predictable code using types. But sometimes we work with data whose type is unknown, especially when receiving API responses or user input.

In these situations, many beginners use `any`. Although `any` seems convenient, it can create dangerous bugs. `any` is the **Type Safety Hole**।

On the other hand, TypeScript provides a safer alternative called `unknown`.


# What is `any`?

The `any` type disables TypeScript checking.

When a variable is `any`, TypeScript allows everything.

```ts
let value: any = "Hello";

value = 10;
value.toUpperCase(); // No error in TypeScript