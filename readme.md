# 1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?
All this is used to target an element by using different css selector. "getElementById" targets using ID selector, "getElementByClass" targets using class selector. "querySelector" and "querySelectorAll" targets using any valid CSS selector. The main difference between them is "querySelectorAll" targets all the occurance and "querySelector" targets the first occurance.

<br>
<br>

# 2. How do you create and insert a new element into the DOM?
1. Create a element using document.CreateElement('element_tag');
2. Add content, attribute or html using element.textContent, element.innerHTML, element.setAttribute(), classList.add() 
3. Add the element to the DOM using parentElement.appendChild(element)

<br>
<br>

# 3. What is Event Bubbling? And how does it work?
Event bubbling is a JS mechanism that triggers a event on parent element that get triggered in child element. <br>
At first the JS created the complete DOM. After that if any event gets triggered, js goes to that element, triggers that element, than traverse back to root of the DOM from that child element and while travesing if there is any event in parent element, that one also gets triggered

<br>
<br>

# 4. What is Event Delegation in JavaScript? Why is it useful?
Event delagation means adding a single event to a parent element instead of using multiple event to the child element. So, if event gets triggered in child element, that one gets triggered by JS Event bubble mechanism.
It's help improve performance, clean code and reduce memory leaks.

<br>
<br>

# 5. What is the difference between preventDefault() and stopPropagation() methods?
"preventDefault()" stops the default behaviour of a browser when gets triggered by a event, while on the other hand "stopPropagation()" stops event bubbling.
