# instrucciones

_basado en el documento alist_
In another example, we can create a two-column layout that fills the entire height of the document. Here is the CSS:

An element with position: fixed shares all the rules of an absolutely positioned element, except that the viewport (browser/device window) positions the fixed element, as opposed to any parent element. Additionally, a fixed element does not scroll with the document. It stays, well…fixed. Let’s look at an example:

#box_2 {
	position: fixed;
	bottom: 0;
	left: 0;
	right: 0;
}
Example I shows a footer with some copyright text in it as a fixed element. As you scroll, notice that it doesn’t move. Notice that the left and right offset properties are set to zero. Since the fixed value behaves similar to the absolute value, we can stretch the width of the element to fit the viewport while fixing the element to the bottom using bottom: 0;. Use caution with the fixed value: Support in older browsers is spotty at best. For example, older versions of Internet Explorer render fixed elements as static elements. And, you now know that static elements don’t behave like fixed elements, right? If you do plan to use fixed elements in a layout, there are several solutions that can help make your element behave properly in browsers that don’t support the fixed value.
