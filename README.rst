============
Python Koans
============

This is an adapted and simplified version of the Python Koans repo you can find at:

https://github.com/gregmalcolm/python_koans

Python Koans is an interactive tutorial for learning the Python programming
language by making tests pass.

Most tests are *fixed* by filling the missing parts of assert functions. Eg:

    self.assertEqual(__, 1+2)

which can be fixed by replacing the __ part with the appropriate code:

    self.assertEqual(3, 1+2)

Occasionally you will encounter some failing tests that are already filled out.
In these cases you will need to finish implementing some code to progress. For
example, there is an exercise for writing some code that will tell you if a
triangle is equilateral, isosceles or scalene.

As well as being a great way to learn some Python, it is also a good way to get
a taste of Test Driven Development (TDD).

Getting Started
---------------

To test your koans just run::

    python3 contemplate_koans.py

or run the script provided::

    ./run.sh

The first run you will see apparently a test failed::

    AssertionError: False is not True

It also tells you exactly where the problem is, it's an assert on line 12
of .\\koans\\about_asserts.py. This one is easy, just change False to True to
make the test pass.

Sooner or later you will likely encounter tests where you are not sure what the
expected value should be. For example::

    class Dog:
        pass

    def test_objects_are_objects(self):
        fido = self.Dog()
        self.assertEqual(__, isinstance(fido, object))

This is where the Python Command Line can come in handy. In this case I can
fire up the command line, recreate the scenario and run queries:

.. image:: https://user-images.githubusercontent.com/2614930/28401750-f9dcb296-6cd0-11e7-98eb-c20318eada33.png

Getting the Most From the Koans
-------------------------------

Quoting the Ruby Koans instructions::

	"In test-driven development the mantra has always been, red, green,
	refactor. Write a failing test and run it (red), make the test pass
	(green), then refactor it (that is look at the code and see if you
	can make it any better). In this case you will need to run the koan
	and see it fail (red), make the test pass (green), then take a
	moment and reflect upon the test to see what it is teaching you
	and improve the code to better communicate its intent (refactor)."
