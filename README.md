

class ListManipulator:
    def __init__(self):
        self._internal_list = []

    def add_elements(self, elements):
        """
        Appends the given elements to the internal list.
        """
        self._internal_list.extend(elements)

    def remove_duplicates(self):
        
        Removes duplicate elements from the internal list.
        
        self._internal_list = list(set(self._internal_list))

    def reverse_list(self):
        
        Reverses the order of elements in the internal list.
      
        self._internal_list.reverse()

    def sort_list(self):
        
        Sorts the elements in the internal list in ascending order.
        
        self._internal_list.sort()

    def get_unique_elements(self):
        
        Returns a new list containing only the unique elements from the internal list.
        
        return list(set(self._internal_list))

    def remove_element(self, element):
        
        Removes the first occurrence of the specified element from the internal list.
        
        if element in self._internal_list:
            self._internal_list.remove(element)

    def get_list(self):
        
        Returns the current state of the internal list.
        
        return self._internal_list

# Example usage:
# manipulator = ListManipulator()
# manipulator.add_elements([1, 2, 3, 2, 3, 4])
# print(manipulator.get_list())  # Output: [1, 2, 3, 2, 3, 4]
# manipulator.remove_duplicates()
# print(manipulator.get_list())  # Output: [1, 2, 3, 4]
# manipulator.reverse_list()
# print(manipulator.get_list())  # Output: [4, 3, 2, 1]
# manipulator.sort_list()
# print(manipulator.get_list())  # Output: [1, 2, 3, 4]
# print(manipulator.get_unique_elements())  # Output: [1, 2, 3, 4]
# manipulator.remove_element(2)
# print(manipulator.get_list())  # Output: [1, 3, 4]
 
