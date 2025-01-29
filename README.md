# Ada Shallow Array Copy Pitfall

This example demonstrates a common pitfall in Ada: the shallow copy nature of array assignment.  When you assign one array to another, you're not creating a completely independent copy. Instead, both arrays point to the same underlying data. Modifying one array affects the other.

This behavior can lead to hard-to-find bugs if not understood.

The solution demonstrates the use of `My_Array'Copy` to create a deep copy, which avoids this issue.