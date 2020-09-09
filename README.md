# ToDoList
A Todo list app

This app was with the intent to excersize some of the Android development concepts that I have been studying.
The app uses 3 fragments.
1. A "display" or "home" fragment (Where all of the ToDo items are listed)
2. An "add" fragment (Where the user creates a new todo list item)
3. An "update" fragment (Where the user can update details on an item or just delete it)

The app displays the todo list items on the "display" fragment via recycler view with each item inside a card view.
Each item has 3 elements, a title, description, and a "priority" or "importance" level. The priority level can be
high priority (which displays as a red dot on the card view), medium priority (yellow dot), or low priority (green dot).
These priority levels also serve as a way to sort the list of todo list items via custom SQL queries using a Room database.
You can sort the todo list items on the home fragment by clicking on the 3 dots in the top right corner of the screen.
Furthermore, you can also search the list via the search icon which is also in the top left of the screen. You can also
update an item by simply clicking on it, which will take you to the update fragment. The update fragment has the same
UI as the add fragment with the exception of the menu and save icons in the top left. The menu icon only gives one option
which is to delete the fragment. When the user selects the save button, live data observers on the home fragments view
model class notice the change, and update the home fragment accordingly. 

This app is available on the Google Play store via this link: https://play.google.com/store/apps/details?id=my.first.todoapp
