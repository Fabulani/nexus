# Usage

Always use the colored buttons in the ribbon (left-side bar). There is a button for each task:
- New Quest
- New Item
- New Template
- and so on...

![Buttons in the ribbon](./Images/Buttons-in-ribbon.png)

For Quests and Inventory, set fields in the front matter as you like. You can also add additional content in the note body.

Creating new templates involves also creating a new class. See below.

## Creating new classes

Metadata Menu, QuickAdd, and Templater are used for the class system:
1. Create a note for each selector field with all possible values in `Settings/Fields`
2. Create a file class in `Settings/Classes`. This represents a new type of class and defines the fields for the template.
3. Use the `New Template` button to create a new template file. Wait until it prompts for adding properties, and click on the `Add this field at the end of the front matter` button on the top right of the modal.
4. Create a new QuickAdd template choice for creating the note.

## Updating a note's front matter with new fields

Easiest method is to click on the class icon button in the note and select `Insert missing fields in the front matter`. It's at the bottom of the front matter.

Another method is to use the command `Metadata Menu: Bulk insert missing fields` and click on the last button, `Insert at the end of the front matter`.
