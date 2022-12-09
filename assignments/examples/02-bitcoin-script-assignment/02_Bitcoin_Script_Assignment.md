# Assignment 02 - Bitcoin Script

Name    : Yuhao Zhang  
Email   : yuhaozhang@utexas.edu  
Discord : yz4236  Description goes here

## Program Inputs

The inputs of this script can be any pair of integers. But here we use 1 and 2 as an example. 

```python
## First Input
<1>

## Second Input
<2>
```

## Program Script

The script goes through the following operations:

```python
OP_2DUP   # Duplicate both inputs.
OP_SWAP   # The top two items on the stack are swapped
OP_ADD    # Pop the top two items of the stack, add them, and push the result on top
OP_ROT    # The 3rd item down the stack is moved to the top
OP_ROT    # The 3rd item down the stack is moved to the top
OP_ADD    # Pop the top two items of the stack, add them, and push the result on top 
OP_EQUAL  # Check that both elements are equal 
```

## Result

This script is demonstrating the simple law that a + b = b + a. It first caculates the result of a + b and then calculates the result of b + a, and lastly verifies that the results are the same. 

## Resources

**Script Wiz IDE**  
https://ide.scriptwiz.app