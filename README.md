# Python Tips

## Read a CSV file

https://earthly.dev/blog/csv-python/

import csv

with open("./filename.csv", 'r') as file:
  csvreader = csv.reader(file)
  for row in csvreader:
    print(row)

