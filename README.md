# Unexpected String Concatenation in JavaScript

This repository demonstrates a common JavaScript bug caused by the language's loose typing system.  When performing arithmetic operations with mixed data types (e.g., numbers and strings), JavaScript may perform string concatenation instead of numerical addition, leading to unexpected results.

## The Bug

The `foo` function attempts to add two values. However, because one of the inputs is a string, JavaScript treats the `+` operator as a string concatenation operator, resulting in the output '12' instead of the expected numerical sum 3.

## The Solution

The solution involves explicitly type-checking the inputs or converting them to numbers before performing the addition to enforce the desired behavior.  This ensures that the `+` operator is used for numerical addition as intended.