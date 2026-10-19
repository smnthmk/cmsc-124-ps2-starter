# Reasoning Before Execution

Write the rule behind each case before you commit your predictions. Replace
every placeholder line below with one to three sentences that name the rule
producing that case's value, type, length, and dimensions. One rule is enough.
After you run and find a miss, add a short correction entry under that case in a
later commit.

## P01
According to the coercion rule, since the values have different types, R converts them to a common type based on the coercion ladder. Because 3.5 is a double, which has the highest level among the three, the other values are also converted to doubles.

## P02
According to the coercion rule, since "2" is of character type which ranks highest in the coercion ladder, R changes all the values into characters, resulting in ["1", "2", "TRUE"].

## P03
R uses the recycling rule when performing arithmetic on vectors of different lengths. The shorter vector repeats its values to match the longer one, so the operation becomes 10 + 1, 20 + 2, 30 + 1, and 40 + 2.

## P04
Positive indexing selects elements based on their position in the vector. Since R starts counting at 1 instead of 0, the indices 3 and 1 select third = 9 and first = 8, respectively.

## P05
Negative indexing in R removes the element at the specified position. Since -2L refers to the second element, 7 is excluded, leaving [4, 9].

## P06
R uses the logical OR operator (|) to select elements that satisfy at least one condition. Here, is.na(x) selects the missing value, while x > 10L selects 12. The type stays as integer since NA_integer_ represents an NA of integer type.

## P07
Factor in R groups values based on the categories specified by the levels argument. These categories are stored internally as integers based on their order, so low is encoded as 1 and high as 2.

## P08
Lists in R can store groups of values with different data types. The length counts the top-level components, so this list has a length of 2 because it contains scores and label.

## P09
A data frame is a list of equal-length columns with row and column dimensions.
Because of this, its type is list and its length equals its 2 columns, giving it dimensions of 2x2.

## P10
A matrix and an array are atomic vectors with a dim attribute.
A matrix is an underlying atomic vector with dimensions attached, which stores the 6 integers across 2 rows and 3 columns, giving dim = 2x3.

## P11
NA is a missing value. It has no explicit given type, and has a length of 1.

## P12
An atomic vector stores one basic type.
Since 9 is written without an L suffix, R stores it as a double with a length of 1.

## P13
According to the coercion rule, since 2.5 is a double which ranks highest in the vector, R converts all values into doubles, resulting in [1, 2.5, 3].

## P14
An atomic vector stores one basic type.
Since the numbers lack L suffixes, R defaults to storing every element as a double, resulting in a vector of length 4.

## P15
A matrix and an array are atomic vectors with a dim attribute.
An array is an underlying atomic vector with dimensions attached, which stores 8 integer values structured across 3 dimensions of length 2, giving dim = 2x2x2.

## P16
Index 0 selects nothing and returns a zero-length result of the same atomic type.
Since [] contains no elements, it returns a zero-length result while keeping its integer type.
