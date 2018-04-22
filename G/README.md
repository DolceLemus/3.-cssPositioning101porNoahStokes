# instrucciones

_basado en el documento alist_

Not to be outdone by other position property values, the absolute value offers some really cool functionality using the offset property. Use two or all four offset properties, and you can stretch an element without defining any width or height—it’s bound only by its parent element or the document itself. Let’s see it in action. Consider the following code:

#box_a {
	position: absolute;
	top: 10px;
	right: 10px;
	bottom: 10px;
	left: 10px;
	background: red;
}
#box_b {
	position: absolute;
	top: 20px;
	right: 20px;
	bottom: 20px;
	left: 20px;
	background: white;
}
In example G we’ve created a border offset 10 pixels by the document, and it’s entirely fluid as the document resize—all with absolute positioning and offsets. 
