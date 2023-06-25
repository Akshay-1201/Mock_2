# Mock test 2
## Q 1 
Implement a stack using an array in JavaScript. Include the necessary methods such as push, pop, and isEmpty.
## Answer
```js
class Stack {
  constructor() {
    this.stack = [];
  }

  push(element) {
    this.stack.push(element);
  }

  pop() {
    if (this.isEmpty()) {
      return "Stack is empty";
    }
    return this.stack.pop();
  }

  isEmpty() {
    return this.stack.length === 0;
  }
}

const stack = new Stack();

stack.push(10);
stack.push(20);
stack.push(30);

console.log(stack.pop()); 
console.log(stack.pop()); 
console.log(stack.isEmpty());
console.log(stack.pop()); 
console.log(stack.isEmpty());
console.log(stack.pop()); 
```
#
## Q 2
 mplement a queue using an array in JavaScript. Include the necessary methods such as enqueue, dequeue, and isEmpty.
## Answer 
```js
 class Queue {
  constructor() {
    this.queue = [];
  }

  enqueue(element) {
    this.queue.push(element);
  }

  dequeue() {
    if (this.isEmpty()) {
      return "Queue is empty";
    }
    return this.queue.shift();
  }

  isEmpty() {
    return this.queue.length === 0;
  }
}

const queue = new Queue();

queue.enqueue(10);
queue.enqueue(20);
queue.enqueue(30);

console.log(queue.dequeue()); 
console.log(queue.dequeue()); 
console.log(queue.isEmpty()); 
console.log(queue.dequeue());
console.log(queue.isEmpty()); 
console.log(queue.dequeue()); 
```