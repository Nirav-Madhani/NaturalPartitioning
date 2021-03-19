
# NaturalPartitioning
Simple project to implement Natural Partitioning using on 3-4-5 Rule. You can also generate the final tree using this notebook.

## Features

1. Apply Natural Partitioning to discrete data.
2. Both methods support user defined depth.
3. 2 Variants -  Simple Printing and Recursive Dictionary that stores all information about partitioning, and can be plotted as tree.

Sample Input:
```
32, 38, 48, 91, 46, 37, 22, 69, 78, 82, 33, 49, 55, 66, 84, 86, 67, 80, 79, 44
```

Sample Output:

```
8 Distinct MSD
 4 Partition
 22.0 to 39.25
 [32, 38, 37, 22, 33]
	 2 Distinct MSD
	 4 Partition
	 22.0 to 26.0
	 [22]
	 26.0 to 30.0
	 []
	 30.0 to 34.0
	 [32, 33]
	 34.0 to 38.0
	 [37]
 39.25 to 56.5
 [48, 46, 49, 55, 44]
	 2 Distinct MSD
	 4 Partition
	 44.0 to 46.75
	 [46, 44]
	 46.75 to 49.5
	 [48, 49]
	 49.5 to 52.25
	 []
	 52.25 to 55.0
	 []
 56.5 to 73.75
 [69, 66, 67]
	 1 Distinct MSD
	 5 Partition
	 66.0 to 66.6
	 [66]
	 66.6 to 67.2
	 [67]
	 67.2 to 67.8
	 []
	 67.8 to 68.4
	 []
	 68.4 to 69.0
	 []
 73.75 to 91.0
 [78, 82, 84, 86, 80, 79]
	 2 Distinct MSD
	 4 Partition
	 78.0 to 80.0
	 [78, 79]
	 80.0 to 82.0
	 [80]
	 82.0 to 84.0
	 [82]
	 84.0 to 86.0
	 [84]
   ```


## Applying on Star.csv 

This time, rather than just printing, I'm using dictionary to store partition range as well as points in each partition

```
1939.0 - 9551.2
	 1939.0 - 4420.333333333334
	 4420.333333333334 - 6901.666666666667
	 6901.666666666667 - 9383.0
 9551.2 - 17163.4
	 9675.0 - 11541.25
	 11541.25 - 13407.5
	 13407.5 - 15273.75
	 15273.75 - 17140.0
 17163.4 - 24775.6
	 17200.0 - 19057.5
	 19057.5 - 20915.0
	 20915.0 - 22772.5
	 22772.5 - 24630.0
 24775.6 - 32387.8
	 25000.0 - 26459.75
	 26459.75 - 27919.5
	 27919.5 - 29379.25
	 29379.25 - 30839.0
 32387.8 - 40000.0
	 32460.0 - 33768.0
	 33768.0 - 35076.0
	 35076.0 - 36384.0
	 37692.0 - 39000.0
   ```
   
   Sample Tree:
   
   
