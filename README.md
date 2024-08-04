# List-Set-Tuple-and-Dictionary-in-Python
## Python Data Structures README
## Welcome to the guide on basic Python data structures! This document provides an overview of lists, sets, tuples, and dictionaries in Python, along with examples and key methods.

## Table of Contents
1. Lists
2. Sets
3. Tuples
4. Dictionaries
5. Lists
## Overview
A list in Python is an ordered collection of items that can be of any type. Lists are mutable, meaning you can change their content after creation.

Creating Lists
``` python 
  Copy code 
  my_list = [1, 2, 3, 4, 5]
  mixed_list = [1, "two", 3.0, [4, 5]] 

## Key Methods
append(item): Adds an item to the end of the list.
extend(iterable): Extends the list by appending elements from an iterable.
insert(index, item): Inserts an item at a specified index.
remove(item): Removes the first occurrence of an item.
pop([index]): Removes and returns the item at the specified index. If no index is specified, it removes and returns the last item.
sort(key=None, reverse=False): Sorts the items of the list in place.
reverse(): Reverses the elements of the list in place.

## Example
python
Copy code
numbers = [1, 2, 3]
numbers.append(4)       # [1, 2, 3, 4]
numbers.remove(2)       # [1, 3, 4] 

## Sets
## Overview
A set is an unordered collection of unique items. Sets are mutable and are often used for membership testing and eliminating duplicate entries.

## Creating Sets
python
Copy code
my_set = {1, 2, 3}
empty_set = set()

## Key Methods
add(item): Adds an item to the set.
remove(item): Removes an item from the set. Raises a KeyError if the item is not present.
discard(item): Removes an item from the set if it exists. Does not raise an error if the item is not present.
pop(): Removes and returns an arbitrary item from the set.
clear(): Removes all items from the set.
union(other_set): Returns a set that contains all items from both sets.
intersection(other_set): Returns a set that contains only items present in both sets.
difference(other_set): Returns a set that contains items present in the set but not in the other set.

## Example
## Overview
A tuple is an ordered collection of items, similar to lists, but unlike lists, tuples are immutable. Once created, their contents cannot be changed.

## Creating Tuples
python
Copy code
my_tuple = (1, 2, 3)
single_item_tuple = (1,)

## Key Methods
## Example
python
Copy code
coordinates = (10, 20)
coordinates.count(10)    # 1

## Dictionaries
## Overview
A dictionary in Python is an unordered collection of key-value pairs. Keys must be unique and immutable, while values can be of any type.

## Creating Dictionaries
python
Copy code
my_dict = {'name': 'Alice', 'age': 25}

## Key Methods
get(key, default=None): Returns the value for the specified key. Returns default if the key is not found.
keys(): Returns a view object that displays a list of all the keys.
values(): Returns a view object that displays a list of all the values.
items(): Returns a view object that displays a list of all key-value pairs.
update(other_dict): Updates the dictionary with key-value pairs from another dictionary.
pop(key, default=None): Removes the item with the specified key and returns its value. If the key is not found, returns default.
popitem(): Removes and returns a random (key, value) pair from the dictionary.
clear(): Removes all items from the dictionary.

## Example
python
Copy code
person = {'name': 'Alice', 'age': 25}
person['age'] = 26              # {'name': 'Alice', 'age': 26}
person.get('name')             # 'Alice'
