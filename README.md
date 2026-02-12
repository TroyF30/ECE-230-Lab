# Lab 04 - SOP/POS and KMaps

Troy Fowers & Peter Krahn

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

What we learned in this lab is creating truth tables, through K-Maps, in multiple files through the naive, minterm and maxterm files allow us to check our work and make sure that 
what we have written down is correct, by comparing the wave forms of the truth tables. This allowed us to use the Basys3 board to check our table using the LED lights, that were 
then tested by the insructors. We also learned of the importance of setting up the different .v files correctly, otherwise it won't simulate properly.

## Lab Questions

### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?

Because there is only a change of a single bit when going around, and similarly to what we were shown in the lecture, you can think of a K-Map as a cylinder, which helps when 
creating the function of the truth table. 

### Why are the names Sum of Products and Products of Sums?

The names are what they are, because the OR (|) function is similar to a sum, while the AND (&) is similar to a product. This means that when we combine the different minterms 
and maxterms through OR and AND, we get sums or products, and then we combine the different ways that the K-Maps are made up through the operator that we didn't use, causing the
minterm to be the Sum of Products, meaning a bunch of AND statements combined through OR's, and the maxterm to be the Product of Sums, meaning a bunch of OR terms combinded through 
AND's.

### Open the test.v file – how are we able to check that the signals match using XOR?

Through the test.v file we are able to use the XOR (^) to check the signals to see if they have the same output. If the output of the XOR was 0, is meant that the outputs of the tested
truth tables were the same, and if the output of the XOR was 1, it meant that the truth tables did not have the same output.

