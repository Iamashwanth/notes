# 4. Classes:

* Representation is part of the definition for concrete types. Even if it’s just a pointer to the data stored elsewhere, it is present in each object of a concrete class.
* Functions defined in a class are inline by default.
* const specifier on functions indicate they they do not modify the object for which they are called.
* Operations that do not require direct access to representation of the class can be defined separately from the class definition
* Try to compose complex operations using the simple ones instead of accessing class representation every time.
* A class with a pure virtual function is called an abstract class.
* Abstract classes do have destructors because someone destroying it through a pointer has no idea what resources are owned by its implementations.
* Member destructor is implicitly invoked by the class destructor.
* If the object passed to dynamic cast is not of the expected type or a class derived from the expected type, it returns a null. When casting a reference to different type is unacceptable, bad cast is thrown.
* Functions returning pointer to an object allocated on free store are dangerous. unique_ptr fixes this problem by freeing them when they goe out of scope.
