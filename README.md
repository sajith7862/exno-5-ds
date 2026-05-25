# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Name : Mohamed Hameem Sajith J
# Reg : 212223240090

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
import numpy as np
import pandas as pd
```
```python
x1=[1,2,3]
y1=[2,4,1]

x2=[1,2,3]
y2=[4,1,3]

plt.plot(x1,y1,label='line1')
plt.plot(x2,y2,label='line2')

plt.xlabel('x-axis')
plt.ylabel('y-axis')

plt.title('Two lines on same graph')
plt.legend()

plt.show()
```
<img width="567" height="455" alt="image" src="https://github.com/user-attachments/assets/c79b5d33-8e97-4ff1-b86d-bc2e7f90708e" />

```python
x=[1,2,3,4,5,6]
y=[2,4,3,5,2,7]

plt.plot(x,y,
         color='blue',
         linestyle='dashed',
         linewidth=3,
         marker='s',
         markerfacecolor='yellow',
         markersize=7)

plt.xlabel('x-axis')
plt.ylabel('y-axis')

plt.title('Some cool customizations')
plt.show()
```
<img width="554" height="455" alt="image" src="https://github.com/user-attachments/assets/3051d639-5cd4-40f7-8438-940a66a7214d" />

```python
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]

plt.plot(years,yield_apples)

plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')

plt.show()
```
<img width="584" height="432" alt="image" src="https://github.com/user-attachments/assets/79c3aaa6-fb31-4384-8518-50c6ba0f1620" />

```python
years=range(2000,2012)

apples=[0.895,0.91,0.919,0.926,0.929,0.931,
        0.934,0.936,0.937,0.9375,0.9372,0.939]

oranges=[0.962,0.941,0.93,0.923,0.918,0.908,
         0.907,0.904,0.901,0.898,0.9,0.896]

plt.plot(years,apples)
plt.plot(years,oranges)

plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')

plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges'])

plt.show()
```
<img width="576" height="455" alt="image" src="https://github.com/user-attachments/assets/ca3a5245-c755-4753-9f11-5bb2b4193b9e" />

```python
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]

plt.scatter(x_values,y_values,
            s=30,
            color='green')

plt.show()
```
<img width="543" height="413" alt="image" src="https://github.com/user-attachments/assets/38559bd7-49f5-4135-90b0-967148497bbe" />

```python
x=np.arange(0,10)
y=np.arange(11,21)

plt.scatter(x,y,c='r')

plt.xlabel('x-axis')
plt.ylabel('y-axis')

plt.title('Graph in 2D')

plt.show()
```
<img width="563" height="455" alt="image" src="https://github.com/user-attachments/assets/6185fcb7-0547-4298-80b8-227a3f2fe084" />

```python
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)

plt.title('Sine wave form')

plt.plot(x,y)

plt.show()
```
<img width="568" height="435" alt="image" src="https://github.com/user-attachments/assets/774e463b-4e9f-4891-af8e-5e877fe561d1" />

```python
x=[1,2,3,4,5]

y1=[10,12,14,16,18]
y2=[5,7,9,11,13]

plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')

plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')

plt.legend(['y1','y2'])

plt.show()
```
<img width="556" height="413" alt="image" src="https://github.com/user-attachments/assets/f8a8784d-9c54-4386-b60c-8225363cff93" />

```python
height=[10,24,36,40,5]

names=['one','two','three','four','five']

c1=['b','g']

plt.bar(names,height,color=c1,width=0.5)

plt.xlabel('x-axis')
plt.ylabel('y-axis')

plt.title('My bar chart')

plt.show()
```
<img width="562" height="455" alt="image" src="https://github.com/user-attachments/assets/9112c814-45e2-45aa-8a66-8e852f2892b5" />

```python
ages=[5,7,9,40,30,45,50,45,43,40,44,
      60,7,13,57,18,90,77,32,21,20,40]

bins=[0,10,20,30,40,50,60,70,80,90,100]

plt.hist(ages,
         bins,
         range=(0,100),
         color='blue',
         histtype='bar',
         rwidth=0.7)

plt.xlabel('age')
plt.ylabel('No of people')

plt.title('My Histogram')

plt.show()
```
<img width="554" height="455" alt="image" src="https://github.com/user-attachments/assets/89b2ca62-269f-4af0-9cb6-13eacb2622cc" />

```python
np.random.seed(0)

data=np.random.normal(loc=0,
                      scale=1,
                      size=100)

fig,ax=plt.subplots()

ax.boxplot(data)

ax.set_xlabel('Data')
ax.set_ylabel('Values')

ax.set_title('Box plot')

plt.show()
```
<img width="565" height="455" alt="image" src="https://github.com/user-attachments/assets/377ccc92-1f72-42a6-89be-00a0d10f41e0" />

```python
labels=['Python','C++','Ruby','Java']

sizes=[215,130,245,210]

colors=['gold','lightcoral','lightskyblue','yellowgreen']

explode=(0,0.1,0,0)

plt.pie(sizes,
        explode=explode,
        labels=labels,
        colors=colors,
        autopct='%1.1f%%',
        shadow=True)

plt.axis('equal')

plt.show()
```
<img width="515" height="389" alt="image" src="https://github.com/user-attachments/assets/5f204772-8966-4936-896b-899fcc03e48d" />


# Result:

Thus the program to perform Data Visualization using matplotlib python library for the given data is implemented successfully.
