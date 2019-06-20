# Merging csv files

Merge multiple csv files using pandas

### Merging two files:

```py
import pandas as pd

input1 = input("File name (including path) 1: ")
csv_input = pd.read_csv(input1)
df = pd.DataFrame(csv_input)
input2 = input("File name (including path) 2: ")
csv_input2 = pd.read_csv(input2)
df2 = pd.DataFrame(csv_input2)
column = input("Column to match: ")
combined = pd.merge(csv_input, csv_input2, on=column)
output = input("Output name: ")
combined.to_csv(output, index=False)
```

### Merging more:

```py
import pandas as pd

input1 = input("File name (including path) 1: ")
csv_input = pd.read_csv(input1)
df = pd.DataFrame(csv_input)
input2 = input("File name (including path) 2: ")
csv_input2 = pd.read_csv(input2)
df2 = pd.DataFrame(csv_input2)
input3 = input("File name (including path) 3: ")
csv_input3 = pd.read_csv(input3)
df3 = pd.DataFrame(csv_input3)
column = input("Column to match: ")
combined = pd.merge(csv_input, csv_input2, csv_input3, on=column)
output = input("Output name: ")
combined.to_csv(output, index=False)
```

etc...
