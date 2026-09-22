# Lab 04 - SOP/POS and KMaps

In this lab, you’ve learned how to apply KMaps, Sum Of Products and Products of
sums to simplify digital logic equations. Then, you’ve proven out that they work
using an implemented design on your Basys3 boards.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Summary

I learned about implementing K-Map SOP and POS in Vivado/Verilog and got to see them in action, and I learned more about Vivado tools to see automatically generated schematics/truth tables.

## Lab Questions

### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?
Because across the edges it is still the case that only one variable is changing to create the OR compliment and eliminate variables.  K-Maps neighbors are "circular" in this way.

### Why are the names Sum of Products and Products of Sums?
The sum of products is named as such because first you make a bunch of products and then you sum them together, and likewise the product of sums is named as such because first you make a bunch of products and then you sum them together.

### Open the test.v file – how are we able to check that the signals match using XOR?
Because XOR(^) only goes to 1 if the two inputs are different, we can always check if the outputs are XOR'ed is not 0 to see see if there is a disagreement.
