# What I've Learned

## Capture
- When you throw an event to an element, the browser capture the element that you throwed the event. But wont launch the event just yet.
## Bubble
- After captured where the event occurred, the event will be triggered for all of those elements above them (starts from bottom to up). This is called bubbling.
## `capture: true`
- This is a option to the `addEventListener` that says to the browser to trigger the event in capture-down order. As the elements are being captured, the events will be triggered. `capture: false` is the default.
## Propagation
- The event bubble up to the child elements.
- To stop this, do `e.stopPropagation()`, so the event will only be triggered on the actual element that you want.
## `once:true`
- Same as `element.removeEventListener`
- The event will be run only one time, than it is removed.