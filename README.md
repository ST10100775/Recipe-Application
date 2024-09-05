#RECIPE APP DOCUMENTATION

##NOTE: FOR THE APP TO WORK:

INSTALL NEWTOWNSOFT.JSON - VISUAL STUDIO.

##GO TO PROJECT > MANAGE NUGET PACKAGES>BROWSE (SEARCH & INSTALL)

 	NEWTOWNSOFT.JSON
  NEWTOWNSOFT.JSON. BSON

##PAGE NAVIGATION

Open the app > Home menu page. There are features like a:  Close application  Home page - Home takes you back to the Home page  Add new recipe  Recipe List CLICK ADD RECIPE TO GET STARTED!

##ADD RECIPE PAGE

Home page > Add new recipe > A page that has a textbox for the Recipe Title. (Enter Recipe Name)  Structured so that you can add or remove any data/ingredients or steps to record the recipe. There are food groups, units, and calories that are optional to input. Type in the of one of your ingredients > Food Group > Amount of ingredient > ingredients unit of measurement > number of Calories.  There are two buttons on the side. The “+” button adds a copy of the ingredient/steps whilst the “–“button removes a single copy at a time.

The are two buttons. “SAVE” and “RESET”  The save button saves all the data on the present page to a JSON file.

 The reset button resets all the GUI elements and the text boxes so that the user can create a brand-new Recipe. PLEASE NOTE THAT A MENU WILL NOTIFY YOU IF YOUR RECIPE’S CALORIES EXCEED 300

##RECIPE LIST PAGE

 Displays a data grid with a search bar that displays all the files we created in our add Recipe page.

 It arranges our data from Recipe Name, Calories, Food Group, Creation Date, and Modified Date.

 Our search bar allows us to filter the data to show use a recipe by its name, food group or calorie.

 Double clicking a Recipe will display a message box that will show the contents of the recipe for the user’s own use.

At the bottom are two buttons. “EDIT” and “DELETE”.  The Edit Button edits the contents of the recipe the user selects.  The delete button removes the JSON file of the selected recipe from the folder.

Structure of the Application: The usage of a delegate improves the implementation of the 300-calorie notice. The notification technique was formerly incorporated directly in the code logic. However, a delegation strategy was employed to improve modularity and responsibility separation. This change entails creating a new delegate object to handle the notification feature. Isolating the notification functionality makes the code more orderly and maintainable. It also allows for expansion by enabling for the creation of new notification techniques simply by switching out the delegate object. Overall, using the delegate pattern improves the application's structure and fosters code reusability.

To confirm the accuracy and reliability of the calorie calculation feature, a dedicated unit test was added to the code. The purpose of this test is to confirm that when given a set of specified inputs, the calorie calculating algorithm produces the desired results. The unit test examines multiple scenarios, including border cases and edge cases, to determine the accuracy of the calculation logic. It compares the accuracy of the output to known values to ensure that any future changes to the code do not introduce unforeseen defects or errors. By implementing this unit test, the code increases resilience and quality because it is extensively tested to match the provided criteria.
