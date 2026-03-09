# EX.NO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# Explanation:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
# Line Graph

```py
import matplotlib.pyplot as plt
x= [0,1,2,3,4,5]
y=[0,1,4,9,16,25]
plt.plot(x,y)
plt.show()
```

 ![image](https://github.com/SamyukthaSreenivasan/EXNO-5-DS/assets/119475703/714c39f4-c504-451e-ba95-54704ab98ca1)

```py
import matplotlib.pyplot as plt
x1 = [1,2,3]
y1 = [2,4,1]
plt.plot(x1, y1, label="line 1")

x2 = [1,2,3]
y2 = [4,1,3]
plt.plot(x2, y2, label="line 2")

plt.xlabel('x - axis')
plt.ylabel('y - axis')

plt.title('Two lines on same graph!')

plt.legend()
plt.show()
```
<img width="713" height="575" alt="image" src="https://github.com/user-attachments/assets/bfb780f5-4399-4063-8bde-471f7a8b286e" />

```py
import matplotlib.pyplot as plt

x = [1,2,3,4,5,6]
y = [2,4,1,5,2,6]

plt.plot(x, y, color='red', linestyle='dashed', linewidth = 5, marker='o', markerfacecolor='blue', markersize=14)

plt.ylim(1,8)
plt.xlim(1,8)

plt.xlabel('x - axis')
plt.ylabel('y - axis')

plt.title('Line customization!')

plt.show()
```
<img width="695" height="566" alt="image" src="https://github.com/user-attachments/assets/d8a861c8-8ed2-4046-a225-9f3c460143ec" />

# Scatter Plot

```py
import numpy as np
x = np.arange(0,10)
y = np.arange(11,21)
x
y
```
<img width="372" height="51" alt="image" src="https://github.com/user-attachments/assets/268e77b7-849c-47a4-b15d-9e07037f0a30" />
<img width="479" height="56" alt="image" src="https://github.com/user-attachments/assets/9d0e995a-996e-42e1-abdf-2e31ad0ebf8d" />

```py
y=x*x
y
```
<img width="473" height="44" alt="image" src="https://github.com/user-attachments/assets/81a0566f-6927-4213-a765-f527e91181dc" />

```py
plt.plot(x, y, 'g*', linestyle='dashed', linewidth = 2, markersize = 14)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('2d Diagram')
```
<img width="707" height="599" alt="image" src="https://github.com/user-attachments/assets/7581d292-65b8-420b-82d5-825c22ff07dc" />

```py
np.pi
```
<img width="195" height="40" alt="image" src="https://github.com/user-attachments/assets/77f8c7cd-c214-43c2-a044-77a3642bdbd4" />

```py
x = np.arange(0, 2*np.pi, 0.1)
y = np.sin(x)
plt.title("sine wave form")

plt.plot(x,y, 'go', markersize=8, color="pink")
plt.show()
```
<img width="725" height="596" alt="image" src="https://github.com/user-attachments/assets/0e4ff3b8-c87f-4028-992f-27cf6b672e91" />

# Area Chart

```py
import matplotlib.pyplot as plt
import numpy as np
x = [1,2,3,4,5]
y1 = [10,12,14,16,18]
y2 = [5,7,9,11,13]
y3 = [2,4,6,8,10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```
<img width="697" height="517" alt="image" src="https://github.com/user-attachments/assets/441946d7-12a6-41bd-b5bb-75784a8f36aa" />

# Bar Chart
```py
import matplotlib.pyplot as plt
val=[5,6,3,7,2]
n=["A", "B", "C", "D", "E"]
plt.bar(n,val,color="green")
plt.show()
```
![image](https://github.com/SamyukthaSreenivasan/EXNO-5-DS/assets/119475703/c0033a63-164f-4cc4-996f-95201893ecd0)


```py
import matplotlib.pyplot as plt 
val=[5,6,3,7,2] 
n=["A", "B", "C", "D", "E"] 
plt.barh(n,val,color="green")
plt.show()
```
<img width="674" height="519" alt="image" src="https://github.com/user-attachments/assets/d4ef3611-c357-4b02-beef-0f98f2057d0a" />

```py
import matplotlib.pyplot as plt
height=[10,20,30,40,50]
names=["one", "two", "three", "four", "five"]
c1=["red", "green"]
c2=["b","g"]
plt.bar(names,height, width=0.8,color=c1)
plt.xlabel('x axis')
plt.ylabel('y axis')
plt.title("Bar Chart")
plt.show()
```
![image](https://github.com/SamyukthaSreenivasan/EXNO-5-DS/assets/119475703/555b339d-2f21-4348-9feb-b631839a5e36)

# Histogram

```py
import matplotlib.pyplot as plt
age=[2,5,70,30,45,50,45,43,40,44,60,7,13,57,18,90, 77, 32, 21, 20,40]
range=(0,100)
bins=10
plt.hist(age,bins, range, color="green", histtype='bar', rwidth=0.8)
plt.xlabel('Age')
plt.ylabel('No of People')
plt.title("Histogram")
plt.show()
```

![image](https://github.com/SamyukthaSreenivasan/EXNO-5-DS/assets/119475703/3a7dab5f-b3ec-419e-96c0-8807e20cf43a)

```py
import matplotlib.pyplot as plt
x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1] 
plt.hist(x,bins=10,color='blue', alpha=0.5)
plt.show()
```
<img width="666" height="522" alt="image" src="https://github.com/user-attachments/assets/cc3385c8-756e-4338-bb4d-4f0754502f93" />

# Box Plot

```py
import matplotlib.pyplot as plt 
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
<img width="702" height="441" alt="image" src="https://github.com/user-attachments/assets/51b4354d-4fc0-4677-b16a-e4c41a32c84f" />

```py
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
<img width="704" height="600" alt="image" src="https://github.com/user-attachments/assets/80b774d1-3ca9-49f3-91d4-9e0b96e72eb2" />

# Pie Chart

```py
import matplotlib.pyplot as plt
activities=["eat", "sleep", "work", "play"]
slices=[3,7,8,6]
colors=['r','y','g', 'b']
plt.pie(slices, labels=activities, colors=colors, startangle=90, shadow=True, explode=(0,0,0.1, 0), radius=1.2, autopct='%1.1f%%')
plt.legend()
plt.show()
```
<img width="544" height="498" alt="image" src="https://github.com/user-attachments/assets/efd91c19-2493-4741-bdba-4f5e578c50fc" />

# Result:
Thus the program to Perform Data Visualization using matplot python library for the given datas is been implemented.
