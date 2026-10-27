# ClinicQueue


def reverse_list(items):
    reversed_items = []     

    aladi = len(items) -1
    while aladi >= 0:
        reversed_items = reversed_items + [items[aladi]]    
        aladi -= 1

    return reversed_items

target_number = [1, 2, 3, 4]
target_alphabet = ["a", "b", "c", "d"]

print(reverse_list(target_number))
print(reverse_list(target_alphabet))



def count_occurances(number, target):
    count = 0
    for number in number:
        if number == target:
            count += 1
            
    return count   
print(count_occurances([2, 5, 2, 8, 2], target= 5))     
        
def find_number(numbers, target):
    if not numbers:
        return -1

    for i in range(len(numbers)):
        if numbers[i] == target:
            return i 
 
print(find_number([10, 25, 30, 45], target = 45))       
