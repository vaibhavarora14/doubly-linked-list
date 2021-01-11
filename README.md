## Doubly Linked List in EcmaScript(JavaScript) [⚒ Under progress]

🚀🚀 Production ready implementation of [doubly linked list](https://en.wikipedia.org/wiki/Doubly_linked_list) in EcmaScript

## Example

```js
import DoublyLinkedList from "doubly-linked-list";

const list = new DoublyLinkedList();
list.insert(1);
list.insert(2);

list.contains(2); // true
list.remove(2);
list.contains(2); // false
```

## API

---

### Insertion

- #### insert(element)

  add element to end of the list

  ```js
  const list = new DoublyLinkedList();
  list.add(2);
  list.add(1);
  list.add(3);

  // list - [2 -> 1 -> 3]
  ```

- #### prepend(element)

  add element to start of the list

  ```js
  const list = new LinkedList();
  list.add(2);
  list.add(1);
  list.prepend(3);
  list.add(4);
  // list - [3 -> 2 -> 1 -> 4];
  ```

### Deletion

- #### remove()

  removes element from the list

  ```js
  const list = new DoublyLinkedList();
  list.add(2);
  list.add(1);
  list.add(3);
  // list - [2 -> 1 -> 3]

  list.remove(1);
  // list - [2 -> 3]
  ```

### Search

- #### contains()

  check if element is present in the list or not

  ```js
  const list = new DoublyLinkedList();
  list.add(2);
  list.add(1);
  list.add(3);
  // list - [2 -> 1 -> 3]

  list.contains(4); //false
  list.contains(2); //true
  ```

### Traverse

- #### traverse()

  iterate on list from start to end

  ```js
  const list = new DoublyLinkedList();
  list.add(2);
  list.add(1);
  list.add(3);
  // list - [2 -> 1 -> 3]

  const generator = list.traverse();
  for (const value of generator) {
    console.log(value);
  }
  // console - 2, 1, 3
  ```

- #### reverseTraversal()

  iterate on list from end to start

  ```js
  const list = new DoublyLinkedList();
  list.add(2);
  list.add(1);
  list.add(3);
  // list - [2 -> 1 -> 3]

  const generator = list.reverseTraversal();
  for (const value of generator) {
    console.log(value);
  }
  // console - 3, 1, 2
  ```
