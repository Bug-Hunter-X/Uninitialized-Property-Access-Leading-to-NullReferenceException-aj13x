# Uninitialized Property Access Leading to NullReferenceException in C#

This repository demonstrates a common error in C#: attempting to access a property of a class before it has been assigned a value.  This often leads to a `NullReferenceException` at runtime.

The `bug.cs` file contains the problematic code, while `bugSolution.cs` provides a corrected version.

## Bug Description

The `MyClass` class has a property `MyProperty` of type `int`.  The `MyMethod` attempts to use this property in a calculation without first ensuring it has a value.  If `MyProperty` is not explicitly set before calling `MyMethod`, this results in a `NullReferenceException`. 

## Solution

The solution involves initializing the property either in the constructor or before using it in `MyMethod`. The `bugSolution.cs` file shows the corrected code, demonstrating how to handle this issue.