# paktoluss
#Tortoise is crawling on cartesian plane, it's path is described by array of integers [1, 3, 5, 2, 6, 2, …], after each segment tortoise turns on 90 degrees clockwise. 


# cyclically rotate clock array by one
#each segment tortoise turns on  clockwise

# Method for rotation
def rotate(arr, n):
	x = arr[n - 1]
	
	for i in range(n - 1, 0, -1):
		arr[i] = arr[i - 1];
		
	arr[0] = x;


# Driver function
arr= [1, 3, 5, 2, 6, 2]
n = len(arr)
print ("Given array is")
for i in range(0, n):
	print (arr[i], end = ' ')

rotate(arr, n)

print ("\nRotated array is")
for i in range(0, n):
	print (arr[i], end = ' ')


