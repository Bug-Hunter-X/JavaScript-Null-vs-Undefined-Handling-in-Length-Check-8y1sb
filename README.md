# JavaScript Null vs Undefined Handling in Length Check

This repository demonstrates a common, yet subtle, bug in JavaScript related to how null and undefined values are handled when checking the length of an object.

## Bug Description
The provided JavaScript function `foo` attempts to return the length of the input parameter 'a'. However, it incorrectly handles undefined values, leading to a runtime error when 'a' is undefined.

## Solution
The corrected function explicitly checks for both null and undefined values, ensuring a consistent return value of 0 in all such cases.  This avoids potential runtime errors and ensures predictable behavior.