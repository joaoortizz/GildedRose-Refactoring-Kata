# Gilded Rose Refactoring Kata

This is the solution for the [Gilded Rose Refactoring Kata](https://github.com/emilybache/GildedRose-Refactoring-Kata). The **original** folder contains the cloned files from the original repository. The **refactoring** folder contains the solution. This solution is implemented in Python 3.

## Development
Obeying the instructions of the proposed problem, the **Item** class was not changed. The **GildedRose** class was refactored, and the **Updater** class was also added.

In order to remove all the nested if clauses, the **GildedRose** class now has an **item.name** check in a single `if` clause, with some `elif` options, and an `else` statement (which is more performant and also more readable, i.e., easier to maintain).

## Maintenance
For each item type, a function will be instantiated. If new item types need to be implemented, simply add them as new `elif` conditions and create the function that will handle **sell in** and **quality** accordingly.

## Tests
The **texttest_fixture.py** file has been kept identical to the original and can be run to verify the results. In addition, the **unit_tests.py** file contains step-by-step tests to ensure all possibilities of updates for different types of items.
