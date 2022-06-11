# Python-Nympy


# NumPy (Numeric Python) is a Python package used for building multi dimensional arrays and performing various operations

#For Installation: pip3 install numpy

import numpy as np

# arrange() is a function to arrange the numbers in a perticular dimension
MyArray = np.arange(20)
print(MyArray)            # [ 0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19]

# range of array from 10 to 20
MyArray = np.arange(10, 20) 
print(MyArray)            # [10 11 12 13 14 15 16 17 18 19]

# range of array from 10 to 20 with 2 step gap
MyArray = np.arange(10, 20, 2)
print(MyArray)            # [10 12 14 16 18]


#RESHAPE: It helps to reshapethe array. syntax: reshape(number_of_rows, number_of_columns)
MyArray = np.arange(20)
MyArray = MyArray.reshape(5, 4)
print(MyArray)

# [[ 0  1  2  3 ]
#  [ 4  5  6  7 ]
#  [ 8  9  10 11]
#  [12  13  14  15]
#  [16  17  18  19]]

MyArray = MyArray.reshape(10, 2)
print(MyArray)

# [[ 0  1]
#  [ 2  3]
#  [ 4  5]
#  [ 6  7]
#  [ 8  9]
#  [10 11]
#  [12 13]
#  [14 15]
#  [16 17]
#  [18 19]]

# ones creates array with all entry as 1
myArray = np.ones((3, 4))
print(myArray)

# [[ 1.  1.  1.  1.]
#  [ 1.  1.  1.  1.]
#  [ 1.  1.  1.  1.]]


# zeros creates array with all entry as 0
myArray = np.zeros((4, 4))
print(myArray)

# [[ 0.  0.  0.  0.]
#  [ 0.  0.  0.  0.]
#  [ 0.  0.  0.  0.]
#  [ 0.  0.  0.  0.]]



# shape returns the shape of the array.
print(MyArray.shape)        # (10, 2)

# ndim returns the dimension of the array
print(MyArray.ndim)         # 2

# size returns the total number of elements in an array
print(MyArray.size)         # 20

# to check the data we have dtype.
print(MyArray.dtype)      


# Randome module is use to initialize numbers in randome form in the given range
myArray = np.random.rand(3, 4)
print(myArray)

# [[ 0.25485438  0.74754555  0.27846822  0.36496946]
#  [ 0.96748535  0.68376208  0.79337973  0.48643819]
#  [ 0.48654677  0.05732675  0.15997665  0.57316947]]

