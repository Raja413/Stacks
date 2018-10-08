# Stacks
Stack in Swift

Stacks are like piling up plates, first in last out.

class Stack {
  
  var stackArray = [String]()
  
  func push(element: String) {
    self.stackArray.append(element)
  }
  
  func pop() -> String? {
    
    if self.stackArray.last != nil {
      let theLastString = stackArray.last
      stackArray.removeLast()
      return theLastString
    } else {
      return ""
    }
  }
}

let stack = Stack()
stack.push(element: "Raja")
stack.push(element: "Reddy")
stack.push(element: "Poreddy")

print(stack.pop()) // Prints Poreddy
