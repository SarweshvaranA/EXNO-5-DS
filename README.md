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
 
 ```python
 import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line1")
 ```
 ![alt text](<Screenshot 2024-10-23 102033.png>)
  ```python
  x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line2")
 ```
 ![alt text](<Screenshot 2024-10-23 102050.png>)
  ```python
  x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line1")
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line2")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two line graph')
plt.legend()
plt.show()
 ```
 ![alt text](<Screenshot 2024-10-23 102106.png>)
  ```python
  x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='--',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customization')
plt.show()
 ```
 ![alt text](<Screenshot 2024-10-23 102122.png>)
  ```python
  years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896]
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)')
 ```
 ![alt text](<Screenshot 2024-10-23 102140.png>)
  ```python
  import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=30,color="blue")
plt.show()
 ```
 ![alt text](<Screenshot 2024-10-23 102156.png>)
  ```python
  import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
 ```
 ![alt text](<Screenshot 2024-10-23 102207.png>)
  ```python
  y
 ```
 ![alt text](<Screenshot 2024-10-23 102315.png>)
  ```python
  plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
 ```
 ![alt text](<Screenshot 2024-10-23 102333.png>)
  ```python
  np.pi
 ```
 ![alt text](<Screenshot 2024-10-23 102345.png>)
  ```python
  x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("Sine wave form")
plt.plot(x,y)
plt.show()
 ```
 ![alt text](<Screenshot 2024-10-23 102357.png>)
  ```python
  import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
plt.fill_between(x,y3,color='red')
plt.legend(['y1','y2','y3'])
plt.show()
 ```
 ![alt text](<Screenshot 2024-10-23 102408.png>)
  ```python
  import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
 ```
 ![alt text](<Screenshot 2024-10-23 102422.png>)
  ```python
  x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='red')
plt.bar(x2,y2,color='green')
plt.title('bar graph')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
 ```
 ![alt text](<Screenshot 2024-10-23 102437.png>)
  ```python
  import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No of people')
plt.title('Histogram')
plt.show()
 ```
 ![alt text](<Screenshot 2024-10-23 102459.png>)
  ```python
  import matplotlib.pyplot as plt
x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='blue',alpha=0.5)
plt.show()
 ```
  ![alt text](<Screenshot 2024-10-23 102512.png>)
  ```python
  import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
 ```
 ![alt text](<Screenshot 2024-10-23 102528.png>)
  ```python
  fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Boxplot')
 ```
 ![alt text](<Screenshot 2024-10-23 102632.png>)
  ```python
  import matplotlib.pyplot as plt
# defining labels
activities = ['eat', 'sleep', 'work', 'play']
# portion covered by each label
slices = [3, 7, 8, 6]
# color for each label
colors = ['r', 'y', 'g', 'b']
# plotting the pie chart
plt.pie(slices, labels = activities, colors=colors, startangle=90, shadow = True, explode = (0, 0, 0.1, 0), radius = 1.2, autopct = '81.1f88')
# plotting legend
plt.legend()
# showing the plot
plt.show()
 ```
 ![alt text](<Screenshot 2024-10-23 102645.png>)
  ```python
  # Data to plot
labels = 'Python', 'C++', 'Ruby', 'Java'
sizes = [215, 130, 245, 210]
colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0, 0.4, 0, 0.5)
# Plot
plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show()
 ```
 ![alt text](<Screenshot 2024-10-23 102659.png>)

 
 

# Result:
Hence, Data Visualization using matplot python library for the given datas is performed.
