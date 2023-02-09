# Python Tips

## Read a CSV file

See https://earthly.dev/blog/csv-python/ for more on reading CSV files

```python

import csv

with open("./filename.csv", 'r') as file:
  csvreader = csv.reader(file)
  for row in csvreader:
    print(row)
```
