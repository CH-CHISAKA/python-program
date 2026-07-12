# Introduction 

This lesson, one will learn how to organize code using functions.

A **Function** is a block of code designed to perform a specific task.

## Intro to Functions: 
<!-- A Simple Example -->

The `add_three()` function below accepts any number, adds to it, and then returns the result

``` bash
<!-- Define the function -->

def add_three(input_var):
    output_var = input_var + 3
    return output_var
```

Every function is composed of two pieces: a **header** and **body** 

![alt text](<image-1.png>)


### Header
The function **header** defines the name of the function and its argument(s).

* Every function header begins with `def`, which tells Python that we are about to define a function.

* In the example, the function name is `add_three`.

* In the example, the **argument** is `input_var`. The **argument**is the name of the variable that will be used as input to the function.
    - It is always enclosed in parentheses that appear immediately after the name of the function. 
 note: A function can also have no arguments, ot it can have multiple arguments.

* For every function, the parentheses enclosing the function argument(s) must be followed by a colon : .

### Body
The function **body** specifies the work that the function does.

* Every line of ode in the function body must be indented exactly four spaces. One can do this by `pushing the space bar exactly four times` or by hitting the `Tab button on the keyboard, exactly once`.

* The function does its work by running all of the indented lines from top to bottom.
    - It takes the argument as input, which in the example is `input_var`
    - The function creates a new variable `output_var` with the calculation `output_var = input_var + 3`.
    - Then, the final line of code, called the `return statement`, just returns the value in `output_var` as the function's output.

The code cell above just defines the function, but does not run it. The details of the function body will make more sense in the next cell.

## How to run (or "call") a function
When we run a function, it can also be referred to as `calling` the function.

In the code cell below, we run the function with `10` as the input value. We define a new variable `new_number` which is set to the output of the function.

```bash
# Run the function with 10 as input
 new_number = add_three(10)

 # Check that the value is 13, as expected
 print(new_number)
```
![alt text](<image-2.png>)


<!-- The complete code will look like this -->

```bash 

def add_three(input_var):
    output_var = input_var + 3
    return output_var
    
# Run the function with 10 as input
new_number = add_three(10)

# Check that the value is 13, as expected
print(new_number)

```
![alt text](<image-3.png>)

A simplified version of the code would be

```bash 

# Define the function
def add_three(input_var):
    output_var = input_var + 3
    return output_var
    
# Run the function with 10 as input
# Call it with parentheses and an argument:
# Check that the value is 13, as expected
print(add_three(10))
```

![alt text](<image-4.png>)

**Note**: When we casually refer to the add_three() function in this tutorial, we use empty closing parentheses after the function name. This is consistent with how people generally write explanations of Python code, and the empty parentheses just make it clear that we are referring to a function, as opposed to a variable or another Python object. These parentheses should always be empty, even if the function has arguments

## Naming Functions
When naming your own functions, one should 
* Only use `lowercase letters`
* Words separated by `underscores` instead of spaces.







