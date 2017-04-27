# iOS-Unit-Testing-and-UI-Testing

This tutorial will focus how to write **Unit and UI** tests for your code in Xcode.

This iOS Unit Testing and UI Testing tutorial shows how to use Xcode’s test navigator to test an app’s model and asynchronous methods, how to fake interactions with library or system objects by using stubs and mocks, how to test UI and performance, and how to use the code coverage tool.

## First Things FIRST: Best Practices for Testing
The acronym **FIRST** describes a concise set of criteria for effective unit tests. 
Those criteria are:

* **Fast**: Tests should run quickly, so people won’t mind running them.
Independent/Isolated: Tests should not do setup or teardown for one another.

* **Repeatable**: You should obtain the same results every time you run a test. External data providers and concurrency issues could cause intermittent failures.

* **Self-validating**: Tests should be fully automated; the output should be either “pass” or “fail”, rather than a programmer’s interpretation of a log file.

* **Timely**: Ideally, tests should be written just before you write the production code they test.

## Getting Started

Inspect the Starter Project **BullsEye** and **HalfTunes**.

Let’s start testing!

## Unit Testing in Xcode
### Creating a Unit Test Target
Open the BullsEye project and hit Command-5 to open its test navigator.

Click the + button in the lower-left corner, then select New Unit Test Target… from the menu:

![](https://github.com/virtualforce/iOS-Unit-Testing-and-UI-Testing/blob/master/images/1.png?raw=true)

Accept the default name **BullsEyeTests**. When the test bundle appears in the test navigator, click it to open it in the editor.

![](https://github.com/virtualforce/iOS-Unit-Testing-and-UI-Testing/blob/master/images/2.png?raw=true)

The template imports **XCTest** and defines a BullsEyeTests subclass of **XCTestCase**, with **setup(), tearDown()** and example test methods.

There are three ways to run the test class:

* **Product\Test** or **Command-U**. This actually runs all test classes.

* Click the arrow button in the test navigator.

* Click the diamond button in the gutter.

