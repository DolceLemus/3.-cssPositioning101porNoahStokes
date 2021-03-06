# instrucciones

_basado en el documento alist_

As I mentioned at the beginning of this article, there are five values available to the position property. The fifth value is inherit. It works as the name implies: The element inherits the value of its parent element. Typically, position property elements do not naturally inherit their parent’s values—the static value is assigned if no position value is given. Ultimately, you can type inherit or the parent element’s value and get the same result.

IN ACTION
All this talk and no action. Let’s take a look at a real-world example website that uses all the position values. Example J shows a typical website layout with a header, navigation, content, and footer. Let’s walk through each element, discuss its position property, and why we chose that property.

Let’s start with our #container element. This is simply the containing element that I’m using to center our content within the viewport. The #nav element is the first element within our #container element. No position property is assigned to the #nav element, so by default, it’s set to static. This is fine: We don’t need to do anything to offset this element, or create any new coordinate systems with it. We will need to do that with #content on our next element, so for that element, we’ve applied a position property of relative.

Since we’re not using any offsets here, the position value has no real influence on the #content element, but we placed it there to create a new coordinate system for the #callout element. Our #callout element is set to position: absolute, and since its parent element, #content is set to relative, the offset properties we’re using on #callout are based off the coordinates created by #content. The #callout element uses a negative 80px pixel offset on the right to pull the element outside of its containing parent element. Additionally, I’ve used one of the cooler features of the absolute value on our #callout element: by setting the top and bottom offsets to 100px, I’ve stretched the #callout element to the full height of the document minus the 100px offset on top and bottom.

Since the #callout element has an absolute value, it does not affect other elements. Therefore, we need to add some padding to the #content element to keep our paragraphs from disappearing beneath it. Setting the padding on the right of #content to 250px keeps our content in full view for our users. To bring up the rear, we’ve added a footer with a fixed position to keep it fixed to the bottom of the page. As we scroll, our footer stays in place. Just as we added padding to the #content to keep our paragraphs from disappearing under it, we need to do the same for the #footer element as it is a sibling of the absolute value. Adding 60px to the #content element’s bottom padding ensures that we can scroll the entire document and not miss any text that would normally be hidden under the #footer element.

Now we have a nice, simple layout with navigation, some content, a callout area, and a footer using static, relative, absolute, and fixed elements. Since we’re using the fixed value in this layout, we should apply some techniques to make sure that older browsers still respect our design. [Note: There used to be a link to sample techniques, but that site has since been taken over by malware. Apologies. —Ed.]


https://alistapart.com/d/css-positioning-101/example_j.html
