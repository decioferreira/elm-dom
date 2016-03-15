Library for reading information off the DOM. Use this if you need to
discover geometry information (width, position, ...) of rendered elements.

Elm has two major hurdles to overcome when working with the DOM:

 1. Elm is pure, but the DOM mutates constantly. A function that,
 say, reads the height of a DOM element cannot be pure.
 2. If you use VirtualDom, you do not have direct access to the DOM
 anyway.

In event-handlers, we can overcome both these problems: the DOM does not
mutate while we are handling events, and events typically contain references
to DOM nodes.


