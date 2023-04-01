For application which operates on various sequence STL containers with elements of type:
```
struct Data {
    std::uint8_t x;
    double y;
};
```
* Let container elements with x bigger than given threshold ```x_threshold``` be subset A.
* Let container elements with x smaller or equal to given threshold ```x_threshold``` be subset B.

Implement library with function which:
1. Reorders the container in such a way, that subset A preceeds subset B.
2. Reorders elements of subset B in such a way, that given number ```n``` of elements has smallest value of y and this n elements are in ascending order of y. Let this ```n``` elements be subset C.
3. Accepts callback as a parameter and applies it to elements of subset C. Callback takes ```Data&``` as parameter and returns no result.


Non-functional requirements:
* Source code should be stored in gitlab (e.g. http://gitlab.com)
* Create unit tests for the library
* Run unit tests in gitlab CI

