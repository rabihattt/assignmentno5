1. Difference between selectors

getElementById("id") → Selects one element by its id.

getElementsByClassName("class") → Selects all elements with a given class → returns an HTMLCollection (live list).

querySelector("cssSelector") → Selects the first element that matches a CSS selector.

querySelectorAll("cssSelector") → Selects all matching elements → returns a NodeList


2. Create and insert a new element
let newDiv = document.createElement("div");
newDiv.textContent = "Hello!";
document.body.appendChild(newDiv); // inserts into DOM


3. Event Bubbling

When an event occurs, it starts from the target element and then bubbles up through its parent elements until it reaches document.

4. Event Delegation

Attaching one event listener to a parent element instead of many children, and using event bubbling to detect which child was clicked.
 Useful for better performance and handling dynamic elements.

5. preventDefault() vs stopPropagation()

preventDefault() → Stops the default action (e.g., stopping form submission, stopping a link from opening).

stopPropagation() → Stops the event from bubbling up to parent elements.