# target
problem solving
array = [3,5,3]
target = 6
arr = []
final = []
final_array = []
for i in range(len(array)):
    com = target - array[i]
    if com in arr:
        final.append(array[i])
        final.append(com)
        break 
    arr.append(array[i])
for i in range(len(array)):
    if final[0] == array[i]:
        final_array.append(i)
        array[i] = '.'
        break
for i in range(len(array)):
    if final[1] == array[i]:
        final_array.append(i)
        array[i] = '.'
        break
print(final_array)
    
