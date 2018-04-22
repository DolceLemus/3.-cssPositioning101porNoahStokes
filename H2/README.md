# instrucciones

_basado en el documento alist_
In another example, we can create a two-column layout that fills the entire height of the document. Here is the CSS:

Using some creative thinking you can find several useful applications for position: absolute. Similar tricks use only a single offset value. For example:

#box_1 {
	width: 200px;
	height: 200px;
	background: #ee3e64;
}
#box_2 {
	position: absolute;
	left: 100px;
	width: 200px;
	height: 200px;
	background: #44accf;
}
In example H2, focus on the blue block (#box_2). Notice how I use only one offset, left: 100px;. This allows the #box_2 element to maintain its top edge and still shift 100 pixels to the left. 
