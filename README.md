# Unit 4 Review - Pursuit Farms


## App Description
Remember our unit 1 assessment? Where you made a checkout app in the command line? Turn that into an iOS shopping cart app!

Here is the app:

![pursuit farms](./Images/command_line_app.gif)


## App Architecture

Create your app without a storyboard. Add all views, actions, and gestures programmatically.

### Main View Controller

You should have a main view controller that has a collection view of all the items in your shopping cart. These items should load from the document directory, so that they are available between launches of the app. Each collection cell should have a name, price, and picture of the cart item.

Add a long press gesture recognizer to each cell that brings up an action sheet. The action sheet should give the option to delete that item. See if you can animate the deletion of the cell. You can add other options too!

In the top right of your main view controller should be an "add" button that brings you to a "create new item" view controller. In the top left should be a "person" button that brings up an alert that takes an input (those exist!). This alert should prompt the user to enter a name, which will be persisted to User Defaults and shown as "\(name)'s shopping list" in the navigation bar.

### Create View Controller

In the create view controller, the user should be able to enter an item's name, select the price from a picker, and add a picture. When the user hits a save button, the item should be added to their documents directory. Make each field required.
