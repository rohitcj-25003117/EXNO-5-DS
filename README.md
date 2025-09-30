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
import matplotlib.pyplot as plt  
import numpy as np 
import pandas as pd


x=[2018,2019,2020,2021,2022]
y=[15000, 20000, 25000, 30000, 35000]
plt.plot(x,y,'g*', linestyle="dashed", linewidth=2,markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('2D Diagram')
plt.show()
```
<img width="1386" height="753" alt="image" src="https://github.com/user-attachments/assets/c92d4cc9-24e6-48be-bb22-dda31df99692" />


```
 x=[2018,2019,2020,2021,2022]
 y=[15000, 20000, 25000, 30000, 35000]
plt.subplot(2,2,1)
plt.plot(x,y)
plt.subplot(2,2,2)
plt.plot(x,y,'g')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'ga')
plt.show()
```

<img width="906" height="617" alt="image" src="https://github.com/user-attachments/assets/db9c814c-af46-4f80-9338-2aee098634d3" />

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine waveform")
plt.plot(x,y)
plt.show()
```

<img width="1045" height="687" alt="image" src="https://github.com/user-attachments/assets/ed5fd530-cacf-4597-9699-3b48f6a353c6" />

```
x=[2,8,10]
y=[11,16,9]
x1=[3,9,11]
y1=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x1,y1,color='g')
plt.title("Bar graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
<img width="1027" height="733" alt="image" src="https://github.com/user-attachments/assets/f8fd00b4-a0aa-4a59-a45e-514de1ba4fc0" />

```
x=[1,2,3]
y=[7,3,9]
plt.plot(x,y,color='g')
plt.title("line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
<img width="1062" height="756" alt="image" src="https://github.com/user-attachments/assets/53606398-f509-4e40-a7e5-e3cfb1b2914f" />

```
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1, label='line1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2, label='line2')
plt.title("multiline graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="943" height="802" alt="image" src="https://github.com/user-attachments/assets/ffdb389b-3891-4e9b-9c9f-031a612114c5" />

```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color="green", linestyle="dashed", linewidth=3, marker='o', markerfacecolor="red", markersize=12, label='spices')
plt.ylim(1,8)
plt.xlim(1,8)
plt.title("line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="993" height="691" alt="image" src="https://github.com/user-attachments/assets/538ae9f2-f753-467b-b365-e0335c8be0e2" />

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples, linestyle="dashed", linewidth=3, marker='s', markersize=12,color='g')
plt.show()
```
<img width="1383" height="614" alt="image" src="https://github.com/user-attachments/assets/96c7dc12-3ab7-423b-9b74-49af5ceba809" />

```
oranges=[2,4,6,7,8,12,45]
apples=[2,4,5,6,8,23,37]
years=[2019,2020,2021,2022, 2023, 2024, 2025]
plt.plot(years, apples, marker='o', label='apples')
plt.plot(years, oranges, marker='o', label='oranges')
plt.title("crop yields in kanto")
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.legend()
plt.show()
```
<img width="1080" height="679" alt="image" src="https://github.com/user-attachments/assets/e9e5fa1e-4fb5-48ce-91d6-99a41e0926f0" />

```
oranges=[2,4,6,7,8,12]
apples=[2,4,5,6,8,23]
years=[2019,2020,2021,2022, 2023, 2024]
plt.bar(oranges, apples)
plt.plot(years, apples, label='apples', marker='s')
plt.plot(years, oranges, label='oranges', marker='o')
plt.title("Fruit sales")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="1001" height="612" alt="image" src="https://github.com/user-attachments/assets/023475f8-ed1e-4113-941a-1c9aa44a4700" />

```
years=[2019,2020,2021,2022, 2023, 2024]
oranges=[2,4,6,7,8,12]
plt.figure(figsize=(12,6))
plt.plot(years, oranges, marker='o', label='oranges')
plt.title("Yield of oranges (tons per hectare)")
plt.legend()
plt.show()
```
<img width="1379" height="754" alt="image" src="https://github.com/user-attachments/assets/221b1c0f-d37d-4049-b158-87e1c0f7a39b" />

```
print("scatter plot is:")
x=[1,2,3,4,5,6,7,8,9,10]
y=[2,4,5,7,6,8,9,11,12,12]
plt.scatter(x,y, label='star', color='green', marker='*', s=30)
plt.title("my scatterplot")
plt.xlabel("x-axis")
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="955" height="648" alt="image" src="https://github.com/user-attachments/assets/5171c8e4-8075-4f53-a70e-c2c996dd90b2" />

```
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1, color='green', label='y1')
plt.fill_between(x,y2, color='blue', label='y2')
plt.fill_between(x,y3, color='red', label='y3')
plt.title("fill between is")
plt.legend()
plt.show()
```
<img width="967" height="657" alt="image" src="https://github.com/user-attachments/assets/6e37d00d-6d63-4142-848c-165b4fb74529" />

```
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.stackplot(x,y1, y2,y3, labels=['line1', 'line2', 'line3'])
plt.legend(loc='upper left')
plt.title("Stacked line chart")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
<img width="894" height="650" alt="image" src="https://github.com/user-attachments/assets/2f8abda7-7c43-4c26-8dad-afb44d2dc4aa" />

```
from scipy.interpolate import make_interp_spline
x=np.array([1,2,3,4,5,6,7,8,9,10])
y=np.array([2,4,5,7,8,9,10,11,12,13])
spl=make_interp_spline(x,y)
x_smooth=np.linspace(x.min(),x.max(),100)
y_smooth=spl(x_smooth)
plt.plot(x,y,'o', label='data')
plt.plot(x_smooth,y_smooth, label="spline")
plt.legend()
plt.show()
```
<img width="873" height="654" alt="image" src="https://github.com/user-attachments/assets/d4e9f910-6b62-4411-b4d2-db8f08172776" />

```
values=[5,6,7,3,2]
names=['A', 'B', 'C', 'D', 'E']
plt.bar(names, values, color='green')
plt.show()
```
<img width="1043" height="648" alt="image" src="https://github.com/user-attachments/assets/32427f78-e60c-4e48-9600-38793bf31af5" />

```
ages=[2,5,70,40,45,50,43,40,44,60,7,13,57,18,90, 77, 32,21,20,40]
range1=(0,100)
bins=10
plt.hist(ages, bins, range1, color='green', histtype='bar', rwidth=0.8)
plt.xlabel('ages')
plt.ylabel('no. of people')
plt.title('my histogram')
plt.show()
```
<img width="903" height="750" alt="image" src="https://github.com/user-attachments/assets/4dfbb553-945f-478a-87b8-c6c5b6af16b6" />

```
x=[2,1,6,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10, color='green', alpha=0.5)
plt.show()
```
<img width="921" height="627" alt="image" src="https://github.com/user-attachments/assets/dd91e969-e93a-42a7-bc86-2eea5ae58913" />

```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('x-axis')
ax.set_ylabel('y-axis')
ax.set_title('box plot')
ax.text(0.5, 1.6, 'box plot')
plt.show()
```
<img width="904" height="737" alt="image" src="https://github.com/user-attachments/assets/b777d864-6f9c-47b5-89c1-87aa04b77a9d" />

```
activities=['eat', 'sleep', 'work', 'play']
slices=[3,8,8,6]
colors=['r', 'y', 'g', 'b']
plt.pie(slices, labels=activities, colors=colors, startangle=90, shadow=True, explode=(0,0,0,0), radius=1.2, autopct='%1.1f%%')
plt.legend()
plt.show()
```

<img width="875" height="589" alt="image" src="https://github.com/user-attachments/assets/8cdb51e0-eb7f-4433-ae2f-f50b72d2f017" />

```
labels=['python', 'c++', 'ruby', 'java']
sizes=[215, 130, 245, 210]
colors=['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode=(0.1,0,0.1,0)
plt.pie(sizes, explode=explode, colors=colors, labels=labels, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show()
```
<img width="1381" height="749" alt="image" src="https://github.com/user-attachments/assets/6944670c-1a67-4de0-b98a-d13588151c98" />



# Result:


Thus the data visualization was peformed using matplot python library for the given datas successfully.
