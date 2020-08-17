# Addition

Scenario: Add two numbers

Given I have a calculator that's turned on.

When I enter "number1"
And I press "+" button
And I enter "number2"
And I press "=" button

Then I see the "added sum" as the result

Scenario: Add more numbers

Given I have a calculator that's turned on

when I enter "number1"
And I press "+" button
And I enter  "number2"
And I press "+" button
And so on.
And I press "=" button.

Then I see the "added sum" of more numbers as a result.

Scenario: Result is too large to display (or overrunning the limits)

Given I have a calculator that's turned on

When the result is too large to display

Then I Truncate the overrunning limits.


Scenario: Numbers can be negative

Given I have a calculator that's turned on

When I enter "negative number1"
And I press "+" button
And I enter  "negative number2"
And I press "+" button.
And I press "=" button.

Then I see the "added sum" of the negative numbers as a result.

Scenario: Numbers can be fraction

Given I have a calculator that's turned on

When I enter "fractional number1"
And I press "+" button
And I enter  "fractional number2"
And I press "+" button.
And I press "=" button.

Then I see the "added sum" of the fractional numbers as a result.

Scenario: Number can be irrational

Scenario: Length of each number

Scenario: If number1 or number2 is not entered

Scenario: If the number is real/complex

Scenario: If we are inbetween some operation
