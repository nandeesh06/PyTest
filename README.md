# PyTest
PyTest Framework

What is Pytest?
Pytest is a python based testing framework, which is used to write and execute test codes

Advantages of Pytest
 1. Pytest can run multiple tests in parallel, which reduces the execution time of the test suite.
 2. Pytest has its own way to detect the test file and test functions automatically, if not mentioned explicitly.
 3. Pytest allows us to skip a subset of the tests during execution.
 4. Pytest allows us to run a subset of the entire test suite.
 5. Pytest has a feature called Fixtures which allows us setup and teardown methods.

How Pytest Framework Indentifies test files and test functions?
 1. Name of test case should start from "test_"
 2. Name of file shauld start with "test_" or ends with "_test"
 3. If we use class, Name should start with "Test"

How to Identify and Run multiple test in a suit?
 Pytest provides two ways to run the subset of the test suite.
  1. Select tests to run based on substring matching of test names.
     pytest -k <substring> -v
     -k <substring> represents the substring to search for in the test names.
     Ex: pytest -k great -v
     This will execute all the test names having the word "great" in its name. In this case,they are test_greater() and test_greater_equal(). See the result below
     
  2. Select tests groups to run based on the markers applied.
     - Pytest allows us to use markers on test functions. Markers are used to set various features/attributes to test functions.
     - Pytest provides many inbuilt markers such as xfail, skip and parametrize.
     - Apart from that, we can create our own marker names
     - To use markers, we have to import "pytest module" in the test file

Commands used to run tests:
  1. pytest
  2. pyetst -v : -v increases the verbosity.
  3. pytest <filename> -v: to run specific testfile

How to mark the testcases?
syntax: pytest.mark.<markname> : to mark testcases
        pytest -m <markname> : to run the marked testcase


       


