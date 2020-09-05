# Collections & Enums

## Collections (C#)
1. Collections provide a more flexible way to work with groups of objects. Unlike arrays, the group of objects you work with can grow and shrink dynamically as the needs of the application change. For some collections, you can assign a key to any object that you put into the collection so that you can quickly retrieve the object by using the key.

1. A collection is a class, so you must declare an instance of the class before you can add elements to that collection.

### Using a Simple Collection
- The examples in this section use the generic List<T> class, which enables you to work with a strongly typed list of objects.
- The following example creates a list of strings and then iterates through the strings by using a foreach statement.

#### Many common collections are provided by .NET. Each type of collection is designed for a specific purpose.

  - Some of the common collection classes are described in this section:

   1.  System.Collections.Generic classes

   1.  System.Collections.Concurrent classes

   1.  System.Collections classes

 -- Many common collections are provided by .NET. Each type of collection is designed for a specific purpose. Some of the common collection classes are described in this section:

##### Enumeration types (C# reference)
 1. An enumeration type (or enum type) is a value type defined by a set of named constants of the underlying integral numeric type. To define an enumeration type, use the enum keyword and specify the names of enum members
 
###### Enumeration types as bit flags
  -- If you want an enumeration type to represent a combination of choices, define enum members for those choices such that an individual choice is a bit field. That is, the associated values of those enum members should be the powers of two. Then, you can use the bitwise logical operators | or & to combine choices or intersect combinations of choices, respectively. To indicate that an enumeration type declares bit fields, apply the Flags attribute to it. As the following example shows, you can also include some typical combinations in the definition of an enumeration type.


 
 




