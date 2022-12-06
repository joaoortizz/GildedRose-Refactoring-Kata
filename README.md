# Gilded Rose Refactoring Kata

This is the solution for the [Gilded Rose Refactoring Kata](https://github.com/emilybache/GildedRose-Refactoring-Kata).
The **original** folder contains the cloned files from the original repository.
The **refactoring** folder contains the solution.


## Development
Obeying the instructions of the proposed problem, the **Item** class was not changed. The **GildedRose** class was refactored and the **Updater** class was also added.

In order to remove all the nested if clauses, the **GildedRose** class now has an **item.name** check in a single `if` clause, with some `elif` options and also the `else` (more performant and also more readable, i.e., easier to maintain).


## Maintenance
For each item type, a function will be instantiated.
If new item types need to be implemented, just add it as a new `elif` and create the function that will handle **sell in** and **quality** accordingly.


## Tests
The **texttest_fixture.py** file has been kept identical to the original and can be run to verify the results.
In addition, the **unit_tests.py** file contains step-by-step tests, in order to guarantee all possibilities of updates for different types of items.