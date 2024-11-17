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
```py
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.plot(x_values,y_values)
plt.show()
```
![image](https://github.com/user-attachments/assets/12a59060-4b0e-44b0-9925-422aaf800dac)

```py
import matplotlib.pyplot as plt
x=[1,2,3]
y=[2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel("y-axis")
plt.title('My first grpah!')
plt.show()
```
![image](https://github.com/user-attachments/assets/5f9dd9ce-f813-4637-bbfb-824ebbd0ca02)

```py
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line 1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line 2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("two lines on same grapg!")
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/7f4eb0ad-44bf-4737-89d3-72b32514360c)

```py
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
```
![image](https://github.com/user-attachments/assets/b051d844-fa4d-4067-9e8d-3bc3d149c1af)

```py
plt.stackplot(x,y1,y2,y3,labels=['line1','line2','line3'])
plt.legend(loc='upper left')
plt.title('stacked line chart')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
![image](https://github.com/user-attachments/assets/8924f9e0-9087-472e-b3e9-c4299540c12b)

```py
import numpy as np
import matplotlib.pyplot as plt
values=[5,6,3,7,2]
names=["A","B","C","D","E"]
plt.bar(names,values,color='green')
plt.show()
```
![image](https://github.com/user-attachments/assets/8aae9d13-966a-42bc-bf99-e50b4db717b2)

```py
import matplotlib.pyplot as plt
import numpy as np

ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range = (0, 100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no of people')
plt.title('histogram')
plt.show()
```
![image](https://github.com/user-attachments/assets/ae0a7e72-1e52-4242-9869-c4b9615086e3)

```py
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/user-attachments/assets/ccb784bc-1dcd-498d-acff-02779b94cdce)

```py
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel("data")
ax.set_ylabel("values")
ax.set_title("box plot")
```
![image](https://github.com/user-attachments/assets/b5b0c3a0-dbd8-41e8-85b3-9bca1a190b4d)

```py
import matplotlib.pyplot as plt
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels = slices,colors=colors,startangle=90,shadow = True,explode = (0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/52112cab-d72f-4a6a-8aca-6818439d1917)



# Result:
The Data Visualization using matplot python library is implemented successfully.
