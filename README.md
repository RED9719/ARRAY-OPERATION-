# ARRAY-OPERATION-
import numpy as np
# CREATING AN ARRAY 
arr=np.array([1001,2001,3001,4001,5001])  
print("array\n",arr)

#Add a new element to an array 
arr_1=np.append(arr,8001)
print("the array after adding a new element 8001\n",arr_1)

#Add four elements to an array
arr_2=np.append(arr_1,[900,800,700,600])
print("array after adding  four element at a time\n",arr_2)

#Add an element at the fourth position 
arr_3=np.insert(arr_2,3,455)
print("array after adding element at fourth position\n",arr_3)

#Delete seventh element from the left of an array 
arr_4=np.delete(arr_3,6)
print("array after deleting element at seventh postion\n",arr_4)
#Remove last element and return it 
last_ele=arr_4[-1]
arr_5=np.delete(arr_4,-1)
print("array after removing the last elememt",arr_5)
print("element removed",last_ele)

#Create two arrays having three elements each and merge all three arrays. 
arr_a=np.array([30,20,10])
arr_b=np.array([60,50,40])
merged_array=np.concatenate((arr_a,arr_b))

#Display the array formed in question 
print("final merged array is",merged_array)

#Determine the length of the new array formed 
length=len(merged_array)
print("length of array is",length)


#Print the ninth element of the new array
if length>=9:
    print("ninth element of array is",merged_array[8])
else:
    print("the array does not have a ninth element ")
