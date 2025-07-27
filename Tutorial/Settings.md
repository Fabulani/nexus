# Settings

In the `Settings` folder, we control all the system stuff, like templates, classes, and fields.
## Fields

Each notes contains a list of values for the field. This is used by the `Metadata Menu` plugin so it knows what values to show for selector fields in the edit metadata side panel.
## Classes

The `Classes` folder contains file classes used by the Metadata Menu plugin. They define the expected front matter for notes with that file class, i.e., the properties. A note's file class is defined by its `class` property.
## Templates

Contains note templates. These should always start with the front matter containing the `tags` property, along with all the fields from its class.
## Tags

Each class is associated with a tag of the same name. E.g., `Quest` has the tag `#quest`.