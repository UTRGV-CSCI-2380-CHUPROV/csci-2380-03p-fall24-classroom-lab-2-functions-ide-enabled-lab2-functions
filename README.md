# Lab 2: Functions with Arrays in C++

## Instructions

Complete the required function definitions in `FunctionsLab.cpp`.

You will be working with functions that search, modify, print, and calculate values from integer arrays.

The required functions are:

- `locateSmallest`
- `replaceVariable`
- `printArray`
- `sumOdds`

Some of the function declarations in the starter code are **incomplete and are missing their required parameters**.

You are responsible for reading the comments above each function and determining which parameters the function needs. You must then update the function declaration correctly before implementing the function.

For example, the comments may tell you that a function needs:

- an integer array
- the size of an array
- a starting index
- an ending index
- a target value

Your function declaration must match the requirements described in the comments.

If the parameters are missing or incorrect, the automated tests may **fail to compile**, and commands such as:

```bash
make test
```

and:

```bash
make test try="functionName"
```

may not work correctly.

Do **not** write a `main()` function inside `FunctionsLab.cpp`. The testing framework already provides the `main()` function needed to run the automated tests.

## Running the Tests

Open the terminal in Codespaces and run:

```bash
make test
```

This command compiles your code and runs all provided test cases.

If your code does not compile, first check that:

- Each required function has the correct name.
- You added all required parameters described in the comments.
- The parameter types are correct.
- Your function's return type is correct.
- You did not add a `main()` function to `FunctionsLab.cpp`.

### Running an Individual Test

To run the tests for only one function, use:

```bash
make test try="functionName"
```

Replace `functionName` with the name of the function you are trying to test.

For example:

```bash
make test try="locateSmallest"
```

or:

```bash
make test try="sumOdds"
```

You can also test the other functions individually:

```bash
make test try="replaceVariable"
```

```bash
make test try="printArray"
```

Remember that the test commands expect your function declarations to be written correctly. If a function is missing parameters or uses the wrong parameters, its tests may not compile.

## Using `demo.cpp`

You may use `demo.cpp` to manually test your functions, print values, create arrays, or experiment with your code.

Write your `main()` function inside `demo.cpp`, not `FunctionsLab.cpp`. Include `FunctionsLab.cpp` so that you can call its functions.

Example:

```cpp
#include <iostream>
#include "FunctionsLab.cpp"

using namespace std;

int main() {
    int values[] = {8, 3, 5, 1, 9};

    cout << locateSmallest(values, 0, 4) << endl;

    return 0;
}
```

To compile and run the code inside `demo.cpp`, enter:

```bash
make demo
```

This command runs whatever code you placed inside the `main()` function in `demo.cpp`.

## Important Notes

- Complete and submit your function definitions in `FunctionsLab.cpp`.
- **Read the comments above each function carefully.**
- **Some functions are missing parameters in the starter code. You must determine and add the correct parameters yourself.**
- Do not add a `main()` function to `FunctionsLab.cpp`.
- Do not change the required function names.
- Make sure your function parameters match the requirements described in the starter code comments.
- Use `make demo` to run your own code from `demo.cpp`.
- Use `make test` to run all automated tests.
- Use `make test try="functionName"` to run an individual function's tests.
- Make sure all tests appear green before submitting.

## Cleaning Compiled Files

If you experience unexpected compilation or testing problems, remove the existing compiled files by running:

```bash
make clean
```

Then run the tests again:

```bash
make test
```

---

# Before You Submit

Your final step should be running all of the tests again:

```bash
make test
```

Do not submit the assignment until all tests pass, the test results appear green, and there are no compilation errors or failed test cases.

Before submitting, make sure you have also checked that every required function has the correct parameters based on the instructions and comments in `FunctionsLab.cpp`.