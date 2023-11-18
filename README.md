# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
pos = [[1,30],[2,40],[3,90]]
robot = getRobot()
robot.driveJoints (0,0,0,0,0,0)
delay(5)
for i in pos:
robot.Controller.moveJoint (i[0],i[1])
delay (5)






```
## Output
### 1. Generic Articulated Robot
![image](https://github.com/gifty003/Movement-of-Robot-Joints/assets/145822352/26d04883-0721-425c-9bc8-5cba46ffda4d)


### 2. robot.driveJoints(0,0,0,0,0,0)
![image](https://github.com/gifty003/Movement-of-Robot-Joints/assets/145822352/e6ecc3c8-259d-4347-8d83-297ea751eca9)


### 3. Movement of Joint1
![image](https://github.com/gifty003/Movement-of-Robot-Joints/assets/145822352/b91b1088-9b73-49ef-8a97-44666618885d)


### 3. Movement of Joint2
![image](https://github.com/gifty003/Movement-of-Robot-Joints/assets/145822352/b55aabe8-85fd-4a20-92dc-b1d3f64de8c1)


### 3. Movement of Joint3
![image](https://github.com/gifty003/Movement-of-Robot-Joints/assets/145822352/35ebf90b-775d-44ee-9fc3-3d3d2ff8ff7a)


## Result 
Thus the different robots joints are moved with the help of python list.


