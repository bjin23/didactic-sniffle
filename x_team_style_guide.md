# X-Team 60 Style Guide

Team 60's coding style guidelines will be mostly standard Java style conventions

## Naming conventions

Our group will be using standard camelCase naming conventions (i.e. inOrder, toString, sortHelper)

### Examples
* interfaces
```
interface Printable {
  void print();
}
```
* classes
```
public class Test {
    public static void main (String[] args) {
    }
}
```
* exception types
```
public class DuplicateKeyException extends RuntimeException {
  public DuplicateKeyException(){
      super(s);
  }
}
```
* fields
```
private int height;
private boolean visited;
```
* methods
```
private int getHeight() {
    return height;
}
```
* parameters
```
public void insert(K key) {
}

public void sort(List list) {
}
```
* local variables
```
int height = 0;
boolean balanced = false;
```
* instance constants
```
private final String EXAMPLE_NAME = "example";
```
* class constants
```
public static final String MY_CONSTANT = "hello world";
```

## Commenting style for public and private members of a class or interface:

Most commenting styles will follow standard commenting guidelines.

### Examples

* classes

* fields
* constructors
* methods
```
/**
* This method invokes toString() on any object passed through it.
*
* @param Object o - an object the user wants to passed through it
* @throws IllegalArgumentException
* @return - the Object o applied to toString()
*/
public String toString(Object o) throws IllegalArgumentException {
  return o.toString();
}
```
* coding style (brackets, horizontal, and vertical spacing) for:
  * if statements
  * switch statement
  * while loops
  * for loops
  * enhanced for loops
