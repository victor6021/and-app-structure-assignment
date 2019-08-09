# Android Code Organization

In this project we'll begin to explore keeping code well-organized into logical packages.


## Objectives

- [ ] organize code between activities and models / classes
- [ ] explain the importance of packages for code organization
- [ ] learn how to keep code DRY

## Instructions

### Part 1 - Starter Code

Start with the assignment project in the current repo.

### Part 2 - Add the appropriate packages

Add packages called:

1. `application`
2. `model`
3. `ui`
4. `util`

Move the existing app code to the appropriate packages.

### Part 3 - Add the util methods

Open `TextUtils` and complete the util methods, as specified in the comments. You'll have to look at the documentation and examples for the `NumberFormat`
class to complete this step.

### Part 4 - Define a model class for a Product in the appropriate package

This model will represent a product we're selling and will include the normal characteristics of a product. Fields defined in this model should include:

1. `productName` - the product's name
2. `productDescription` - the product's description
3. `productPrice` - the product's price
4. `productTax` - the dollar-amount of tax for this item
5. `productDiscount` - the percent discount for this item

  (Hint: You should use a Kotlin data class for the model.)

### Part 5 - Open MainActivity and wire up the UI

You'll need to complete the `displayProductDetails` method in MainActivity.

1. Instantiate the model from Part 4. You can give your product any kind of name, description and other characteristics that you want.
2. Open the `activity_main.xml` layout and examine the pre-created `TextView` fields. Take note of their names.
3. In the `displayProductDetails` method you'll want to set the fields from your model into the appropriate `TextViews` in the layout.
4. Use the `TextUtils` you defined from Part 3
5. Display today's date in the `orderDate` `TextView`. Use the appropriate `DateUtils` method for formatting.
6. Search the code for any remaining `TODO` items, and fix any bugs.

### Part 6 - Bonus Challenge

How would you make your model available to every screen in your `Application`? What are the pros and cons to doing this?
