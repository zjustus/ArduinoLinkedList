# ArduinoLinkedList
A full featured and ultra light linked list data structure for the Arduino framework

This is coded under the JustusDevTools namespace

#Functions
LinkedList() - inits the list
~LinkedList() - deletes the linked list
unt8_t length() - returns size of the list
void add(T data) - adds a node to the last of the list
void remove() - removes the current node and preserves the list
T get_data() - gets the current data
T get_next() - gets the current data then increments forward
T get_back() - gets the current data then increments back
void goto_first() - goes to the first node
void goto_last() - goes to the last node
void move_forward() - moves 1 forward
void move_back() - moves 1 back
T *to_array() - converts the linked list to an array of the given type

#Example
#include <LinkedList.h>
LinkedList<unit8_t> x;
x.add('a');
x.add('b');
x.add('c');
x.add('d');

const char* y = x.to_array();
