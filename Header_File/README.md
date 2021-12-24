# Set library for performing set operations with ease in C language

**Please Note that this header file only works in the case of integer arrays and not for strings**

### This repo contains a header file which has all the source code for performing set operations, description of all the pre-defined functions present in the header file are given below,

## 1. Creating sets by passing an array and address of its  size to the pre-defined function in the header file-

    set(array, &size_of_the_array)
    
    This function will return an array which has all properties of sets i.e., without any duplicates.

    Note: The size of the array which is returned by the function is stored in the same variable which is passed to the function i.e., 'size_of_the_array' in this case.

## 2.  To evalute the Union of two sets, just pass two arrays and addresses of their sizes to the pre-defined function-

    set_union(set1, &size_of_set1, set2, &size_of_set2)

    This function will return an array which is a Union set of the two sets passed to the fuction

    Note1: You are also allowed to pass arrays without the properties of sets i.e., with duplicate elements, the function takes care of removing the duplicates i.e., creating sets out of it and will give you the required answer.

    Note2: The size of the array which is returned by the function is stored in the first size variable which is passed to the function i.e., 'size_of_set1' in this case.

## 3. To evalute the Intersection of two sets, just pass two arrays and addresses of their sizes to the pre-defined function-

    set_intersection(set1, &size_of_set1, set2, &size_of_set2)

    This function will return an array which is an Intersection set of the two sets passed to the fuction.

    Note1: You are also allowed to pass arrays without the properties of sets i.e., with duplicate elements, the function takes care of removing the duplicates i.e., creating sets out of it and will give you the required answer.

    Note2: The size of the array which is returned by the function is stored in the first size variable which is passed to the function i.e., 'size_of_set1' in this case.

## 4. To evalute the Difference of two sets, just pass two arrays and addresses of their sizes to the pre-defined function-

    set_difference(set1, &size_of_set1, set2, &size_of_set2)

    This function will return an array which is the Difference set of the two sets passed to the fuction.

    Note1: Please take care of the order while passing the arrays/sets to this function, as it is for the evauation of difference i.e., if you first pass 'set1' and then 'set2' it'll evaluate 'set1 - set2', similarly if you first pass 'set2' and then 'set1' it'll evaluate 'set2 - set1'.
    
    Note2: You are also allowed to pass arrays without the properties of sets i.e., with duplicate elements, the function takes care of removing the duplicates i.e., creating sets out of it and will give you the required answer.

    Note3: The size of the array which is returned by the function is stored in the first size variable which is passed to the function i.e., 'size_of_set1' in this case.

## 5. To sort the set, just pass the set along with the address of its size, and integer '1' for ascending order or '0' for descending order, to the pre-defined function-

    set_sort(set, &size_of_the_set, 1 (or) 0)

    This function will return a sorted version of the set which is passed to the function.

    Note: The size of the set which is returned by the function is same as the size which is passed as during sorting the size remains the same.

## 6. To find the maximum element present in a set, just pass the set along with the address of its size to the pre-defined function-

    maxof(set, &size_of_the_set)

    This function will just return the maximum element/biggest element found in the given set.

## 7. To find the minimum element present in a set, just pass the set along with the address of its size to the pre-defined function-

    minof(set, &size_of_the_set)

    This function will just return the minimum element/smallest element found in the given set.

## 8. To find the sum of all the elements in a set, just pass the set along with the address of its size to the pre-defined function-

    sumall(set, &size_of_the_set)

    This function will just return the sum of all the elements present in a set.