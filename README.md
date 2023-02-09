# Python Tips

### Read a CSV file

See https://earthly.dev/blog/csv-python/ for more on reading CSV files

```python

import csv

with open("filename.csv", 'r') as file:
  csvreader = csv.reader(file)
  for row in csvreader:
    print(row)
```

### Filter rows

with open("filename.csv", 'r') as file:
  csvreader = csv.reader(file)
  for row in csvreader:
    if row.column == "some value":
      print(row)

### Filter and write to a file

with open("./filename.csv", 'r') as file:
  csvreader = csv.reader(inputfile)
  csvwriter = csv.writer(outputfile)
  for row in csvreader:
    if row.column == "some value":
      print(row)
