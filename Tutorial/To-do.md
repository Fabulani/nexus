# Project to-dos:

Status dashboards:
- [ ] Status table showing last modified files
- [ ] Query for all items in a room using dataviewjs. I.e., traverse hierarchy of rooms and containers to reach items.
- [ ] Checkout [SnipeIt App](https://snipeitapp.com/product) for dashboard ideas.

Tutorial:
- [ ] Improve documentation formatting
- [ ] Write the README
- [ ] Customization tutorial
- [ ] Quick-start tutorial
- [ ] Implementation tutorial (how the different plugins and ideas are connected, how they affect eachother, more technical)

Automation: 
- [ ] The macro for new templates applies templater formula (e.g., inserts current date instead of the formula). Any way to fix?
- [ ]  Use a single macro for creating notes with classes.
	- [ ] One macro per class is useful for Commander custom buttons. Will this be useful if the user interacts primarily with the buttons?

Misc:
- [ ] Implement a JDex in the current framework. I.e., implement the JDex entry...
	- [ ] class
	- [ ] fields
	- [ ] template
	- [ ] tutorial entry
	- [ ] status dashboard

# Script drafts

Traverse room and containers to find all items:
```js
let currentRoom = dv.current().file.link;

// Step 1: Find containers in this room
let containers = dv.pages('"Containers"') // or any folder where containers are
  .where(c => c.location && c.location.path == currentRoom.path);

// Step 2: Get all items in those containers
let containerLinks = containers.map(c => c.file.link);
let items = dv.pages('"Items"') // or wherever items are
  .where(i => i.container && containerLinks.includes(i.container));

// Step 3: Display the items
dv.table(["Item", "Type", "Container"], 
  items.map(i => [i.file.link, i.type, i.container])
);

```
