# Data Model

_Objects_ are Nyx's abstraction for data. All data in a Nyx program is represented by objects or by relations between objects. Even Nyx source code itself is represented by objects.

Every object has an identity, a type, and a value. An object's _identity_ never changes once it has been created; identity is an immutable property of an object. Each individual object has an id represented by an integer value. If two bindings each hold a reference to the same integer id, they both reference the same object.

An object's _type_ defines the set of allowable operations on an object. Like its identity, an object's type is an immutable property.

An object's _value_ is the set of data attributes of which an object is the collection. Unlike identity and type, for some objects the value can change. These objects are called mutable; objects whose value cannot change are called immutable.