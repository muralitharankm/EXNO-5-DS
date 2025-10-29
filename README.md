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

# LINE PLOT:

```
marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()


student=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()
```

<img width="748" height="546" alt="image" src="https://github.com/user-attachments/assets/c0486868-43c5-4511-8086-cadd2eeabe8d" />


<img width="747" height="566" alt="image" src="https://github.com/user-attachments/assets/72275385-93db-4765-a171-66b3b8d0e3db" />



# Scatter Plot:
```
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()
x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()
```
<img width="772" height="524" alt="image" src="https://github.com/user-attachments/assets/bb8305be-61a2-41cd-9052-fa3bef2cf51f" />



<img width="760" height="585" alt="image" src="https://github.com/user-attachments/assets/f08762ff-9e0b-4567-a338-fb07ede20084" />


# Pie Chart:
```
act=['eat','sleep','work','play']
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

<img width="722" height="515" alt="image" src="https://github.com/user-attachments/assets/21e4719f-2baa-4bed-8e40-02f510ede3c6" />


<img width="716" height="515" alt="image" src="https://github.com/user-attachments/assets/825f5765-c953-4e04-9870-1c409659e33d" />


# Area Chart:
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

<img width="735" height="542" alt="image" src="https://github.com/user-attachments/assets/fed513c8-b009-4a75-8621-2ec173a2d42b" />


# Bar Chart:
```
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```

<img width="728" height="567" alt="image" src="https://github.com/user-attachments/assets/b8e8aa21-3fce-4622-9320-6eb57a3d079a" />


# Histogram:
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```

<img width="701" height="537" alt="image" src="https://github.com/user-attachments/assets/ea0597ff-055e-4296-ae31-716dea8830f4" />


# Box Plot:
```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```

<img width="727" height="437" alt="image" src="https://github.com/user-attachments/assets/dcf0a740-0736-402e-a72e-26edf2084361" />



```
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

<img width="735" height="617" alt="image" src="https://github.com/user-attachments/assets/b232bf7b-9574-4881-b3d9-b9281bae72d9" />



# Result:
  Thus, all the data visualization techniques of matplotlib has been implemented.
