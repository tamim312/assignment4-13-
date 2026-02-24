1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?
Ans.: getElementById("id") returns only one element it is unique by id,  getElementsByClassName("class") returns all matching classes
, querySelector("selector") return the first match element and querySelectorAll("selector") return all match elements as nodelist.
2.How do you create and insert a new element into the DOM?
Ans.: A new element is created with document.createElement("tag").
parent.appendChild(newElement) or parent.insertBefore(newElement, referenceNode)
3.What is Event Bubbling? And how does it work?
Ans.:Event Bubbling is an event propagation method in JavaScript where an event occurs on a child element, and it gradually moves up to its parent element.
For example, clicking on a button will first handle the button's event, then the event will gradually propagate to its parent div, then the body, and finally the document.
This is the default behavior and often allows the parent element to handle events for multiple child elements at once.
4.What is Event Delegation in JavaScript? Why is it useful?
Ans.:Event Delegation is a JavaScript technique where a single event listener is placed on the parent element, and any event that occurs on the child element is handled through the parent listener.
This can be done without having to set up separate listeners for different child elements.
This is very useful for memory-efficient and dynamic content, because the listener will work even if new elements are added to the DOM in the future.
5.What is the difference between preventDefault() and stopPropagation() methods?
Ans.: The preventDefault() method is used to stop the browser's default behavior, such as page reload or form submit on link click.
The stopPropagation() method is used to prevent event bubbling or capturing, i.e. the event will not reach the parent element.
preventDefault() changes the behavior, but keeps event propagation on.
stopPropagation() stops propagation, but keeps the default browser behavior.
In general, preventDefault = disable default action, stopPropagation = disable event propagation.