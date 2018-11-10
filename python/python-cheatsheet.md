# Python 2.7 Cheatsheet

## Run terminal commands

Example for run the `ls` command.

```python
import os

os.system('ls')
os.system('ls -a')
```



### Read the output

Example for reading the output of a command

```python
import commands

output = commands.getoutput('ls -a')
```

## Class

```python
class class_name:
    def __init__(self):
        ...
    
    def another_function(self):
        ...
```



# Comment

```python
'''
A function
'''
def function():
    return 0
```



# Print multiple line

```python
print(```
Multiple
line
​```)
```



# for

```python
array = []
for index in range(len(array)):
    print(array[i])
```



# try catch

```python
try:
    input = raw_input("Give an input")
except ValueError:
    print('Error')
```

