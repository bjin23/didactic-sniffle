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
```
// this is a class
public class Dictionary{
	public Dictionary() {
	
	}
}
```
* fields
```
// counter variable for number of items in tree
int count = 0;

// constant for number of ASCII characters
private static final int ASCII_COUNT = 128;
```
* constructors
```
/**
* Constructs a DefinitionNode with the specified word and meaning.
* @param word The word associated with this definition
* @param meaning The meaning of that word
* @throws IllegalArgumentException when the word or meaning are either
*   references to an empty string or null references.
*/
public DefinitionNode(String word, String meaning) { 

this.word = word;
this.meaning = meaning;

}
```
* methods
```
/**
* This method invokes toString() on any object passed through it.
*
* @param Object o - an object the user wants to passed through it
* @throws IllegalArgumentException if null is passed to toString()
* @return - the Object o applied to toString()
*/
public String toString(Object o) throws IllegalArgumentException {
  return o.toString();
}
```
* coding style (brackets, horizontal, and vertical spacing) for:
  * if statements
  ```
  if (item == null) {
      throw IllegalArgumentException();
  }
  ```
  * switch statement
  ```
  switch (name) {
      case "Alice":
          message = "Congrats! You got 1st place!"
          break;
      case "Bob":
          message = "Nice! You got 2nd place!"
          break;
      case "Cecil":
          message = "You got 3rd place...out of 3 people."
          break;
      default:
          message = "You didn't participate."
  }
  ```
  * while loops
  ```
  while (!q.isEmpty()) {
  
  }
  ```
  * for loops
  ```
  for (int i = 0; i < n; i++) {
      
  }
  ```
  * enhanced for loops
  ```
  for (Integer i : list) {
  
  }
  ```
