# Homework_4.1



def move_zeros_to_end(lst):
    non_zeros = [x for x in lst if x != 0]
    zeros = [x for x in lst if x == 0]
    return non_zeros + zeros

assert move_zeros_to_end([0, 1, 0, 12, 3]) == [1, 12, 3, 0, 0], 'Test1'
assert move_zeros_to_end([0]) == [0], 'Test2'
assert move_zeros_to_end([1, 0, 13, 0, 0, 0, 5]) == [1, 13, 5, 0, 0, 0, 0], 'Test3'
assert move_zeros_to_end([9, 0, 7, 31, 0, 45, 0, 45, 96, 0, 0]) == [9, 7, 31, 45, 45, 96, 0, 0, 0, 0], 'Test4'

print("Все тесты пройдены!")
