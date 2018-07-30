## What is Hashing?


Hashing, in cryptography is the process of mapping a given arbitrary amount of data to a fixed length digest. Since it is deterministic
in nature, the same input given will produce the same output value every time. It is a mathematical algorithm that maps the input 
to a fixed length value and is designed to be a one-way (non-invertible) function.

For e.g. consider the following hash function h, that returns the ASCII value and next two characters in series, for the first character
of the given input: 

* h (a)  =>  97bc
* h (cat)  => 99de
* h (ant)  => 97bc


 But this cannot be considered as a “good” hash function, because we can see that we get similar hashes for words starting with the same
letter of the alphabet. A perfect hash function maps every key to a different value. 

The ideal cryptographic hash function has the following properties:
*	should be deterministic
*	should be non-invertible
*	a small change to the message should change the hash extensively so that the old and new value appear completely unrelated.
*	No two strings must have the same hash value i.e. h(x1) ≠h(x2) for x1 and x2

Since the input length is unbounded (i.e. it can be any length) and the output is bounded by a fixed length, there will always be cases where two different inputs generate the same output. This is called a collision. It is not possible for a hash function to be collision-free. However, cryptographic hash functions can be resistant to collision, i.e. it is very difficult to find two inputs that generate the same output.A non-perfect but a good example of hashing algorithm is the SHA-3.
Several variants like SHA3-256 and SHA3-512 exists. Several other hashing algorithms exist like SHA-1 and MD5 which are obsolete now.


The following table shows a collision resistant set of hashes.

```String``` | ```SHA-256 Hash```
------------ | -------------
```Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua``` | ```29c03d361dde0dbff070f8efad6da05fcb72e0cc825c301ab8f0596224bc23c7```
```lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua``` | ```c1f947fd7d47254945c9131be3254609634c84f709b60bb37c6a8f3377300392```
```Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.```| ```973153f86ec2da1748e63f0cf85b89835b42f8ee8018c549868a1308a19f6ca3```

