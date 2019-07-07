# JavaScript_DoublyLinkedList
A doubly linked list built in JavaScript along with test cases.

Test Cases:

var doublyLinkedList = new DoublyLinkedList();
doublyLinkedList.print(); 
// => ''
doublyLinkedList.add(1);
doublyLinkedList.add(2);
doublyLinkedList.add(3);
doublyLinkedList.add(4);
doublyLinkedList.print(); 
// => 1 2 3 4
console.log('length is 4:', doublyLinkedList.length()); 
// => 4
doublyLinkedList.remove(3); 
// remove value
doublyLinkedList.print(); 
// => 1 2 4
doublyLinkedList.remove(9); 
// remove non existing value
doublyLinkedList.print(); 
// => 1 2 4
doublyLinkedList.remove(1); 
// remove head
doublyLinkedList.print(); 
// => 2 4
doublyLinkedList.remove(4); 
// remove tail
doublyLinkedList.print(); 
// => 2
console.log('length is 1:', doublyLinkedList.length()); 
// => 1
doublyLinkedList.remove(2); 
// remove tail, the list should be empty
doublyLinkedList.print(); 
// => ''
console.log('length is 0:', doublyLinkedList.length()); 
// => 0
doublyLinkedList.add(2);
doublyLinkedList.add(6);
doublyLinkedList.print(); 
// => 2 6
doublyLinkedList.insertAfter(3, 2);
doublyLinkedList.print(); 
// => 2 3 6
doublyLinkedList.traverseReverse(function(node) { console.log(node.data); });
doublyLinkedList.insertAfter(4, 3);
doublyLinkedList.print(); 
// => 2 3 4 6
doublyLinkedList.insertAfter(5, 9); 
// insertAfter a non existing node
doublyLinkedList.print(); 
// => 2 3 4 6
doublyLinkedList.insertAfter(5, 4);
doublyLinkedList.insertAfter(7, 6); 
// insertAfter the tail
doublyLinkedList.print(); 
// => 2 3 4 5 6 7
doublyLinkedList.add(8); 
// add node with normal method
doublyLinkedList.print(); 
// => 2 3 4 5 6 7 8
console.log('length is 7:', doublyLinkedList.length()); 
// => 7
doublyLinkedList.traverse(function(node) { node.data = node.data + 10; });
doublyLinkedList.print(); 
// => 12 13 14 15 16 17 18
doublyLinkedList.traverse(function(node) { console.log(node.data); }); 
// => 12 13 14 15 16 17 18
console.log('length is 7:', doublyLinkedList.length()); 
// => 7
doublyLinkedList.traverseReverse(function(node) { console.log(node.data); }); 
// => 18 17 16 15 14 13 12
doublyLinkedList.print(); 
// => 12 13 14 15 16 17 18
console.log('length is 7:', doublyLinkedList.length()); 
// => 7
