# NewStackFromJSON
Example of how to use JSON Data to create a new stack complete with card's UI

This stack has a field containing JSON data of a LiveCode stack and card objects that is used to recreate the new Stack and UI of the cards.

It is possible to export a JSON file which represents everything need to recrreate the satck from only the JSON file data. It's also a way to do version control using Git of a stack's binary elements not found in script files or script only sracks.

Clicking on the button "Create New Stack from JSON below" will create a new stack from the JSON data found in the field below the button.

The "Click to Create JSON Data of All Objects and Scripts in this Stack" button will create a JSON data in the field below it of all stack properties, all card(s) properties and all objects founs on all cards in the stack.

This allow you to edit this data to include or exclude cards or controls with their properties including thier scripts.

Warning: If you copy and paste the data from a currently loaded stack without modifying the "ID" properties the LiveCode engine will try to duplicate the open stack in memory since the engine assigns the "ids" when creating or changing objects which can crash LiveCode. Changing the Stack and Card "ids" will fix this problem or leaving the values empty will also work since the engine will just assign new ones.
