# LinkedList-Data-Storage

## Vocabulary List Data Structure

This project implements a vocabulary list management system using doubly linked lists and singly linked lists in Java. The main components of the structure are depicted in the diagram, showing the relationships and organization of the data.

![Graph](GraphRepresentation.png)

### Main Components

#### Doubly Linked List (`DoublyLinkedList`)

- **Head**: Points to the first `DNode`.
- **Tail**: Points to the last `DNode`.
- **Size**: Keeps track of the number of nodes in the list.
- Contains nodes (`DNode`), each representing a vocabulary category.

#### Doubly Linked Node (`DNode`)

- **Next**: Points to the next `DNode` in the list.
- **Prev**: Points to the previous `DNode` in the list.
- **Vocab**: Holds a `Vocab` object that includes the topic and a list of words.

#### Vocabulary (`Vocab`)

- **Topic**: A string representing the category/topic of the vocabulary (e.g., "Sports", "Animals").
- **Words**: A singly linked list containing the words associated with the topic.

#### Singly Linked List (`SinglyLinkedList`)

- **Head**: Points to the first `SNode`.
- **Tail**: Points to the last `SNode`.
- **Size**: Keeps track of the number of nodes in the list.
- Contains nodes (`SNode`), each representing a word.

#### Singly Linked Node (`SNode`)

- **Word**: A string representing the word.
- **Next**: Points to the next `SNode` in the list.

### Example Structure

- The `DoublyLinkedList` contains 4 `DNode` elements representing the topics: "Sports", "Animals", "Fruits", and "Drinks".
- Each `DNode` links to a `Vocab` object, which contains a `SinglyLinkedList` of words.
  - "Sports" has words: "Tennis", "Squash", "Hockey".
  - "Animals" has the word: "Cow".
  - "Fruits" has words: "Apple", "Orange".
  - "Drinks" has words: "Water", "Sodas", "Beer", "Wine".

### Usage

The implementation allows for efficient management and categorization of vocabulary words. It supports operations such as adding new topics, adding words to existing topics, and navigating through the lists both forwards and backwards due to the doubly linked nature of the main list.

### Features

- **Dynamic Data Structure**: Easily expandable to accommodate more topics and words.
- **Efficient Navigation**: Doubly linked list enables traversal in both directions, making it easy to insert and delete nodes.
- **Category Management**: Each vocabulary topic is managed independently with its own singly linked list of words.

### Diagram Representation

The provided diagram visually represents the structure, illustrating how the doubly linked list (`DoublyLinkedList`) connects multiple topics (`DNode`), each with its own list of words (`SinglyLinkedList`).

---

Feel free to adjust the description as needed for your specific use case or to add any additional details that are relevant to your project.
