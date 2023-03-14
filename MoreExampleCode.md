# More Example Code

The purpose of this webpage is to provide you, the reader, with examples of the code that I have worked on during my time within the IT program.

Much of the following code was written for the purpose of completing assignments for IFOTC1000 and INFOTC1040

## Example Code
The following code listed below was used to determine the frequency of certain keys on a piano, the code works best with valid inputs such as: "440"
```
// 
import math #Use 440 for input

frequency = int(input())
r = math.pow(2,1/12)

my_value1 = (frequency * math.pow(r,0))
my_value2 = (frequency * math.pow(r,1))
my_value3 = (frequency * math.pow(r,2))
my_value4 = (frequency * math.pow(r,3))
my_value5 = (frequency * math.pow(r,4))
print(f'{my_value1:.2f} {my_value2:.2f} {my_value3:.2f} {my_value4:.2f} {my_value5:.2f}')
```
The following code listed below was used in INFOTC1000 to determine the radius of a cone

```
//
import math 
print("Please enter the radius of the cone: ")
radius = float(input())
print("Please enter the height of the cone: ")
height = float(input())

output_radius = math.pow(radius,2)
output_height = height / 3

output_final = math.pi * output_radius * height / 3
print("The volume of the cone is: ",output_final, "units")
```
This last piece of code was quite complicated, but essentailly it is used to swap lists within python with other lists and also appends them together.

```
//
def swap_items_inplace(l, i, j):
    temp = l[i]
    l[i] = l[j]
    l[j] = temp

def reverse_list_inplace(l):#This function takes the list "l" and reverses
                            #The items in the list by calling swap_items_inplace
    n = len(l)
    for i in range(n//2):
        swap_items_inplace(l, i, n-i-1)

def test_reverse_list(case_num, actual, expected): #This function takes the
                #Actual result and the expected result to test if they are equal
    print("Test " + str(case_num) + ": ", end="")
    if actual == expected:
        print("Passed")
    else:
        print("Failed")

if __name__ == "__main__":
    # Test 1
    test_1 = [1]
    reverse_list_inplace(test_1)
    test_reverse_list(1, test_1, [1])

    # Test 2
    test_2 = [1, 2]
    reverse_list_inplace(test_2)
    test_reverse_list(2, test_2, [2, 1])

    # Test 3
    test_3 = [1, 2, 3]
    reverse_list_inplace(test_3)
    test_reverse_list(3, test_3, [3, 2, 1])

    # Test 4
    test_4 = [1, 2, 3, 4]
    reverse_list_inplace(test_4)
    test_reverse_list(4, test_4, [4, 3, 2, 1])

    # Test 5
    test_5 = [1, 2, 3, 4, 5]
    reverse_list_inplace(test_5)
    test_reverse_list(5, test_5, [5, 4, 3, 2, 1])

    # Test 6
    test_6 = [1, 2, 3, 4, 5, 6]
    reverse_list_inplace(test_6)
    test_reverse_list(6, test_6, [6, 5, 4, 3, 2, 1])
```

## Thank you for taking the time to look at my code 

 
