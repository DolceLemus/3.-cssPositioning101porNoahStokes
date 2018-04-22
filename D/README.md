# instrucciones

_basado en el documento alist_

Creating a coordinate system for child elements is another one of the relative positioning property’s super powers. A coordinate system is a reference point for offset properties. Recall in example C, our blue block (#box_2) is not sitting inside of any other elements, so the coordinate system it’s using to offset itself 200 pixels from the left is the document itself. If we place the #box_2 element inside of #box_1, we’ll get a different result, as #box_2 will position itself relative to the coordinate system from #box_1. For the next example, we won’t change any CSS, we’ll adjust our HTML to move #box_2 inside of #box_1:

<div id="box_1">
	<div id="box_2"></div>
</div>
Example D shows our new markup. Because of the new coordinate system, the blue block measures its offset 200 pixels from the left of the red block (#box_1) instead of the document. This practice is more common with elements set to position: absolute—the way you wish you could have built towers when you were younger.
