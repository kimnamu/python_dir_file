## 1. os library
import os

### 1.1 Return the curruent path
```python
os.getcwd()
# /Users/task/
```

### 1.2 Return the list of fils
```python
os.listdir(<PATH>)
# ['file1.txt', 'file2.txt', 'file3.txt']
```
### 1.3 Change the current working directory to path
```python
work_dir = '/Users/task1'
os.chdir(work_dir)
os.getcwd()
# /Users/task1
```

### 1.4 Join one or more path compoenets
```python
path1 = '/Users/task1'
path2 = 'chocolate'
path = os.path.join(path1, path2)
path
# /users/task1/chocolate
```

### 1.5 Create a directory named path with numeric mode
```python
os.mkdir(<PATH>)
```

### 1.6 Return True if path is an existing directory
```python
os.path.isdir(<PATH>)
# True or False
```

### 1.7 Rename the file or directory src to dst
```python
os.rename(<PATH>, <NEW_PATH>)
# NEW_PATH
```

### 1.8 Creat the dir
```python
os.mkdir(<PATH>)
```

### 1.9 Remove the directory (when directory is empty) and file
```python
os.rmdir(<PATH>)
os.remove(<FILE>)
```



## 2. shutil
```python
import shutil
```

### 2.1 Copy and paste
```python
shutil.copyfile(<SRC_PATH>, <DST_PATH>)
```

### 2.2 Remove the directory(whether directory is empty or not) and file
```python
shutil.rmtree('/User/task/subtask1')
```

## 3. glob
```python
import glob
```

### 3.1 Get all files or specific files
```python
# All files
glob.glob(os.path.join(<PATH>,'*'))
# ['b.txt', 'a.txt', 'd.jpg', 'c.jpg', 'e.jpg']

# Specific files
glob.glob(os.path.join(<PATH>, "*.jpg"))
# ['c.jpg', 'e.jpg', 'd.jpg']
```

## Reference
[1] https://docs.python.org/3/library/os.html <br/>
[2] https://docs.python.org/3/library/shutil.html  <br/>
[3] https://docs.python.org/3/library/glob.html <br/>
