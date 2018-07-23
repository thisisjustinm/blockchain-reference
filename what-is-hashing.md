#What is Hashing?


Hashing, in cryptography is the process of mapping a given arbitrary amount of data to a fixed length digest. Since it is deterministic
in nature, the same input given will produce the same output value every time. It is a mathematical algorithm that maps the input 
to a fixed length value and is designed to be a one-way (non-invertible) function.
For e.g. consider the following hash function h, that returns the ASCII value and next two characters in series, for the first character
of the given input: 

* h (a)  =>  97bc
* h (cat)  => 99de
* h (ant)  => 97bc


 But this cannot be considered as a “good” hash function, because we can see that collisions occur for words starting with the same
letter of the alphabet. A perfect hash function maps every key to a different value. 
The ideal cryptographic hash function has the following properties:
•	should be deterministic
•	should be non-invertible
•	a small change to the message should change the hash extensively so that the old and new value appear completely unrelated.
•	No two strings must have the same hash value i.e. h(x1) ≠h(x2) for x1 and x2



A non-perfect but a good example of hashing algorithm is the SHA-3.
Several variants like SHA3-256 and SHA3-512 exists. Several other hashing algorithms exist like SHA-1 and MD5 which are obsolete now.
