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
Replace this line with the rule that decides this case.

## P10
Replace this line with the rule that decides this case.

## P11
Replace this line with the rule that decides this case.

## P12
Replace this line with the rule that decides this case.

## P13
Replace this line with the rule that decides this case.

## P14
Replace this line with the rule that decides this case.

## P15
Replace this line with the rule that decides this case.

## P16
Replace this line with the rule that decides this case.
