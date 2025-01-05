# Unexpected Type Coercion with Null Comparisons

This repository demonstrates a common JavaScript bug related to type coercion when comparing values to `null` using loose equality (`==`).

## The Bug

The provided JavaScript function `foo` aims to add two numbers. If either input is `null`, it returns `null`. However, the loose equality check (`===`) is used. In JavaScript, loose equality (`==`) can lead to unexpected type coercion. This can cause issues when comparing numerical values and null, particularly with falsy values like 0.

## The Solution

The solution utilizes strict equality (`===`) to prevent type coercion. Strict equality checks for both value and type, avoiding the unexpected behavior caused by loose equality.