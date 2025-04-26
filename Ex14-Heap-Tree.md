# Ex.No.(3D). Heap Tree
## DATE:17-03-25
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm
1. Start
2. Find the index of the element num in the array.
3. Swap the element to be deleted with the last element in the array.
4. Decrease the array size (size) by 1.
5. Start heapifying from the last non-leaf node (index size/2 - 1).
6. Call heapify() to restore the heap property for each node.
7. End
## Program:
```
/*
Program to delete an element in a Heap Tree
Developed by:MUKITHA V M 
RegisterNumber:212223040119 
*/
```
```
void deleteRoot(int array[], int num)
{
int i;
for(i=0;i<size;i++)
{
if(num==array[i])
{
break;
}
}
swap(&array[i],&array[size-1]);
size-=1;
for(i=size/2-1;i>=0;i--)
{
heapify(array,size,i);
}
}
```

## Output:
![Screenshot 2025-04-26 162521](https://github.com/user-attachments/assets/c5dd0fa3-b5f9-4f2e-ba14-87a424c87b86)

## Result:
Thus, the function to delete an element in a Heap Tree is implemented successfully.
