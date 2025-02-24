Download link :https://programming.engineering/product/homework-02-gone-fishing/


# Homework-02-Gone-Fishing
Homework 02 – Gone Fishing
Topics: Javadocs, inheritance, constructor chaining, copy constructor, static variables, wrapper classes, good class design

Problem Description

The first wave of midterms has passed, and it’s time to relax a little. You decide it’s time to go fishing, and you return with an impressive haul! You decide to apply your object-oriented programming skills to record information about your new fish friends.

Solution Description

You will complete and turn in 4 classes: Fish, Catfish, StripedBass, and FlyingFish. Each of these classes have constructors, methods, and variables that are described below. A lot of the code will be reused through inheritance, so make sure you pay attention to the hints given below!

Notes:

All variables should be inaccessible from other classes and require an instance to be accessed through, unless specified otherwise.

All methods should be accessible from everywhere and must require an instance to be accessed through, unless specified otherwise.

Use constructor and method chaining whenever possible! Ensure that your constructor chaining helps you minimize code repetition and maximize code reuse!

Helper methods with appropriate visibility are optional.

Make sure to add Javadoc comments to your methods and classes!

Fish.java

This class defines a Fish object.

Variables:

String name – the name of this fish

This field should be visible to any descendant classes.

An invalid value should default this field to “Nemo”.

A value is invalid if it is an empty String, blank String, or null.

This value cannot be changed once set.

Double length –the end-to-end length of this fish in inches

This field should be visible to any descendant classes.

An invalid value should default this field to 8.0.

A value is invalid if it is not a number, infinite, nonpositive, or null.

Hint: Reference the Double API to help implement this logic.

Double weight –the weight of this fish in ounces

This field should be visible to any descendant classes.

An invalid value should default this field to 2.0.

A value is invalid if it is not a number, infinite, nonpositive, or null.

int totalFish – a value tracking the number of fish that have been introduced to your

aquarium

o This variable should only be subject to modification in the body of Fish constructors. o Hint: Consider what keyword enables a value to be tracked at the class, rather than

instance level.

Constructors:

A constructor that takes in name, length, and weight.

Note: Constructor parameters should be written in the listed order.

A constructor that takes in no parameters and sets name to “Nemo”, length to 5.0, and weight to 12.0.

A copy constructor that deep copies all necessary instance fields.

You may assume that the input will not be null.

Methods:

formatLength

Returns the end-to-end length of this fish as a String, formatted precisely as follows (without the angle brackets and quotation marks):

“<feet> ft <inches> in”

feet should be displayed as an integer, and inches should be displayed to 2 decimal places with rounding.

• e.g., A 25.015 inch long fish should yield: “2 ft 1.02 in”

Note: There are 12 inches in 1 foot.

Hint: Check the String API. It has a method that should remind you of printf.

formatWeight

Returns the weight of this fish as a String, formatted precisely as follows (without the angle brackets and quotation marks):

“<pounds> lbs <ounces> oz”

If the weight of this fish includes only one pound, the unit should instead be

“lb”.

pounds should be displayed as an integer, and ounces should be displayed to

2 decimal places with rounding.

▪ e.g., A 16.015 ounce fish would yield: “1 lb 0.02 oz”

Note: There are 16 ounces in 1 pound.

toString

Overrides the corresponding method in its super class, such that a String with the following format is returned (without angle brackets, quotation marks, and trailing or leading whitespace):

“I’m a talking fish named <name>. My length is <feet> ft <inches> in and my weight is <pounds> lbs <ounces> oz.”

Floating-point values should be displayed to two decimal places with rounding.

No getters or setters should be written.
