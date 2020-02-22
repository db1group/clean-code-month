# Methods

## Methods Should Do One Thing

Loops, exception handling, …encapsulate in sub-methods	

## Methods Should Descend 1 Level of Abstraction

The statements within a method should all be written at the same level of abstraction, which should be one level below the operation described by the name of the function.	

## Method with Too Many Arguments

Prefer fewer arguments. Maybe functionality can be outsourced to a dedicated class that holds the information in fields.

## Method with Out/Ref Arguments 

Prevent usage. Return complex object holding all values, split into several methods. If your method must change the state of something, have it change the state of the object it is called on.

## Selector / Flag Arguments 

`public int Foo(bool flag)`

Split method into several independent methods that can be called from the client without the flag.

## Inappropriate Static 

Static method that should be an instance method