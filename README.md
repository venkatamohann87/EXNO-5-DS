# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

## DEVELOPED BY : venkata mohan n
## REGISTOR NO : 24900969
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
import matplotlib.pyplot as plt

x_values = [0, 1, 2, 3, 4, 5]
y_values = [0, 1, 4, 9, 16, 25]

plt.plot(x_values, y_values)
plt.show()

![image](https://github.com/user-attachments/assets/627204bb-fcba-4a0b-a5d5-acd54f5eff68)

# Simple line
```
import matplotlib.pyplot as plt

x = [1, 2, 3]
y = [2, 4, 1]

plt.plot(x, y)
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.title("My first graph!")
plt.show()
```
![image](https://github.com/user-attachments/assets/b5c032ff-adbc-4910-95cc-880c761a015a)

# Simple 2 lines
import matplotlib.pyplot as plt

x1 = [1, 2, 3]
y1 = [2, 4, 1]
plt.plot(x1, y1, label='line 1')

x2 = [1, 2, 3]
y2 = [4, 1, 3]
plt.plot(x2, y2, label='line 2')

plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.title("Two lines on same graph!")
plt.legend()
plt.show()
``
![image](https://github.com/user-attachments/assets/1a008f0f-5b52-4982-9716-ea180b744425)


# Customixation of plots
```
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5, 6]
y = [2, 4, 1, 5, 2, 6]

plt.plot(x,y, color='red', linewidth=3, linestyle='--', marker = 'o', markerfacecolor='blue', markersize=10)
plt.ylim(1, 8)
plt.xlim(1, 8)
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.title("Some cool customization")
plt.show()
```
![image](https://github.com/user-attachments/assets/11f7e71f-79c6-46c5-9504-768a76107d66)


# Scatter Plots
```
import matplotlib.pyplot as plt

x_values = [0, 1, 2, 3, 4, 5]
y_values = [0, 1, 4, 9, 16, 25]

plt.scatter(x_values, y_values, s=30, color="teal")
plt.show()
```
![image](https://github.com/user-attachments/assets/35aa4282-9d64-4198-a38a-d5b7182d14a0)


# Customized Scatter Plot
```
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
y = [2, 4, 5, 6, 7, 8, 9, 11, 12, 12]

plt.scatter(x, y, label="stars", color="blue", marker="*", s=30)
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.title("My Scatter Plot")
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/60d52369-d4bb-4d08-931f-e62d96099fcd)


# Graph in 2D
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

x=np.arange(0, 10)
y=np.arange(11,21)

x
y

plt.scatter(x,y,c='r')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![image](https://github.com/user-attachments/assets/d8453e35-9d1e-4f09-969d-ed94e3593396)


# 2D Diagram
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

x=np.arange(0, 10)
y=np.arange(11,21)

y=x*x
y

plt.plot(x,y,'g*',linestyle='--', linewidth=2,markersize=10)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('2D Diagram')
```
![image](https://github.com/user-attachments/assets/681f6bf4-1b78-489b-9786-cba0d55de7e7)

```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(y,x,'g*--')
plt.subplot(2,2,3)
plt.plot(x,x,'bo--')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
![image](https://github.com/user-attachments/assets/4f764829-37df-4f94-9b4f-fd4e9b63abb7)


# Sine wave form
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

np.pi

x=np.arange(0,3*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
![image](https://github.com/user-attachments/assets/d747e798-efef-49dd-8f01-1aee086c7cb5)


# Area Chart
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]

plt.fill_between(x,y1,color="green")
plt.legend(['y1'])
plt.show()
```
![image](https://github.com/user-attachments/assets/12af0922-7730-415f-a581-a8192fc2508d)


# Stacked Area Chart
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]

plt.fill_between(x,y1,color="red")
plt.fill_between(x,y2,color="blue")
plt.fill_between(x,y3,color="green")
plt.plot(x,y1,color="white")
plt.plot(x,y2,color="beige")
plt.plot(x,y3,color="pink")
plt.legend(['y1','y2','y3'])
plt.show()
```
![image](https://github.com/user-attachments/assets/8ea463f7-ba6d-40ff-a1f9-23fcefcc3271)


# Spline chart
```
import matplotlib.pyplot as plt
import numpy as np
from scipy.interpolate import make_interp_spline

x=np.array([1,2,3,4,5,6,7,8,9,10])
y=np.array([2,4,5,7,8,8,9,10,11,12])

spl = make_interp_spline(x,y)

x_smooth = np.linspace(x.min(),x.max(),100)
y_smooth = spl(x_smooth)

plt.plot(x,y,'o',label='data')
plt.plot(x_smooth,y_smooth,label='spline')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/80223d95-4d77-4525-8024-49452fd01611)


# Bar graph
```
import matplotlib.pyplot as plt
values = [5,6,3,7,2]
names = ["A", "B", "C", "D", "E"]
plt.bar(names, values, color="pink")
plt.show()
```
![image](https://github.com/user-attachments/assets/6e3cbf40-9556-4d10-89be-14f7df33c83c)


# Customized Bar Plot
```
import matplotlib.pyplot as plt

height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1 = ['red','green']
c2 = ['b','g']
plt.bar(names , height, color=c1)

plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart')

plt.show()
```
![image](https://github.com/user-attachments/assets/d84e5268-c960-42e3-85d6-97d1bf3cc8bd)


# Bar plot for 2 features
```
import matplotlib.pyplot as plt

x = [2, 8, 10]
y = [11, 16, 9]
x2 = [3, 9, 11]
y2 = [6, 15, 7]

plt.bar(x,y,color="r")
plt.bar(x2,y2,color="g")
plt.title("Bar graph")
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![image](https://github.com/user-attachments/assets/548c0b93-c696-4734-879b-68d9b962e2ce)


# Histogram
```
import matplotlib.pyplot as plt

ages = [2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,401]
range=(0,100)
bins=10

plt.hist(ages,bins,range,color="blue",histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```
![image](https://github.com/user-attachments/assets/b9c5c6e3-e464-4469-bcb6-8c0b5b3dd38a)

```
import matplotlib.pyplot as plt
import numpy as np

np.random.seed(0)
data = np.random.normal(loc=0, scale=1,size=100)
data
```
![image](https://github.com/user-attachments/assets/8253da01-3b75-46e3-98da-4595203e0627)

```
fig, ax = plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![image](https://github.com/user-attachments/assets/5ed49625-2537-4702-b62d-714906f51e58)


# Pie Chart
```
import matplotlib.pyplot as plt

activities = ['eat', 'sleep', 'work', 'play']
#Pie Chart

import matplotlib.pyplot as plt

activities = ['eat', 'sleep', 'work', 'play']
slices = [3, 7, 8, 6]
colors = ['r', 'y', 'g', 'b']
plt.pie(slices, labels = activities, colors=colors, startangle=90, shadow = True, explode = (0, 0, 0.1, 0), radius = 1.2, autopct = '%1.1f%%')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/1379f23f-7773-48b2-becc-797078b7a8b1)
 
 # Result:
 Thus the data visualization using matplot python library for the given datas are performed
