# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
 ```
import pandas as pd

import numpy as np

import seaborn as sns

import matplotlib.pyplot as plt
```
<img width="505" height="252" alt="image" src="https://github.com/user-attachments/assets/a0593ee1-4512-479a-9664-f9005ba555f5" />
### Line Plot
```
marks=[90,45,63,78]

student=['Raghul', 'Ram', 'Kishore', 'sam']

plt.plot(marks, student)

plt.xlabel('Marks')

plt.ylabel('Student name')

plt.show()


student=['Raghul', 'Ram', 'Kishore', 'Sam']

attendence=[90,85,73,88]

plt.plot(attendence, student)

plt.xlabel('Attendence')

plt.ylabel('Student name')

plt.show()
```
<img width="681" height="592" alt="image" src="https://github.com/user-attachments/assets/bc7d9125-f5b3-48ed-953e-accf33073d54" />
<img width="765" height="546" alt="image" src="https://github.com/user-attachments/assets/50860ba5-55cb-4744-9637-94bbf78db1b2" />
<img width="743" height="561" alt="image" src="https://github.com/user-attachments/assets/2b4cd72b-efe4-4ae1-950e-74363cca3c16" />

### Scatter Plot
```
x=[10,20,30,40,50]
y=[20,40,60,80,100]
plt.scatter(x,y,color='green',marker="*",s=30)
plt.show()
```
<img width="776" height="652" alt="image" src="https://github.com/user-attachments/assets/ff57759d-ed31-4ecf-a268-315bb1dd9098" />
```
x=np.arange(0,30)

y=np.arange(0,30)

x

y

plt.scatter(x,y,c='r')

plt.xlabel('X axis')

plt.ylabel('y axis')

plt.title('Scatter plot')

plt.show()
```
<img width="497" height="248" alt="image" src="https://github.com/user-attachments/assets/fd74f746-60af-41c9-a069-3b5fbe3f5cde" />
<img width="783" height="596" alt="image" src="https://github.com/user-attachments/assets/55769f0e-30b5-4ecb-8ab7-f6308fb45175" />
### Pie chart
```
act=["sleep","eat","work","play"]
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()

feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
<img width="1313" height="337" alt="image" src="https://github.com/user-attachments/assets/a313d73a-9bde-4dd7-b3f5-5fc01483a890" />
<img width="623" height="531" alt="image" src="https://github.com/user-attachments/assets/3bf4452d-fcad-4183-a1c7-5c77016a4364" />
<img width="552" height="532" alt="image" src="https://github.com/user-attachments/assets/1daed0f7-8b83-40c2-ac73-2aabbcc20bd8" />
### Area Chart
```
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```
<img width="697" height="536" alt="image" src="https://github.com/user-attachments/assets/dd4479ac-dcd2-445c-9f5d-3e27089068a1" />
### Bar Chart
```
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green']
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c2)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```
<img width="576" height="237" alt="image" src="https://github.com/user-attachments/assets/61f266c0-37d6-4e9a-bd1a-8ed8c41f8aed" />
<img width="722" height="582" alt="image" src="https://github.com/user-attachments/assets/06a299ef-d49e-48a4-b220-748f6a96f803" />

### Histogram
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.3)
plt.show()

```
<img width="748" height="648" alt="image" src="https://github.com/user-attachments/assets/1d49c21b-d926-42dd-a99b-6448765dd993" />
### Box Plot
```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data

plt.boxplot(data)
plt.xlabel("Data")
plt.ylabel("Values")
plt.title("Boxplot")
plt.show()
```
<img width="756" height="735" alt="image" src="https://github.com/user-attachments/assets/9d281107-fa52-44df-b07d-59f813285251" />

# Result:
Thus, all the data visualization techniques of matplotlib has been implemented.
