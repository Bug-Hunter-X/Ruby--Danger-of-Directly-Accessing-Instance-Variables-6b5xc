# Ruby: The Pitfalls of Directly Accessing Instance Variables

This repository demonstrates a common, yet subtle, error in Ruby: directly accessing and modifying an object's instance variables from outside the class definition.  This practice undermines encapsulation and can introduce hard-to-debug issues.

## The Problem

The `bug.rb` file showcases how directly manipulating instance variables (`@value`) using `instance_variable_set` bypasses the class's intended interface. This weakens encapsulation and can lead to unpredictable results, particularly in larger, more complex applications.

## The Solution

The `bugSolution.rb` file illustrates a better approach. Instead of directly accessing instance variables, we use accessor methods (`value=` and `value`). This provides a controlled way to modify the object's state, making the code more maintainable, robust, and easier to reason about.

## How to Run

1.  Clone this repository.
2.  Run the Ruby scripts using `ruby bug.rb` and `ruby bugSolution.rb` to observe the different behaviors.

This example highlights the importance of adhering to proper object-oriented programming principles in Ruby to build reliable and maintainable applications.