##	Public Key Cryptography

It refers to any system that uses key pairs and, is also called asymmetric key cryptography.
There are two keys involved: 
* public key, known to every one and  
* private key only known to the owner.  

In this system, any person can encrypt a message using the receiver’s public key, 
but the message can be decrypted only by the receiver’s private key.
Due to the complex nature of asymmetric encryption, it is usually used only to transfer small bytes of data, 
like a symmetric encryption key. This key may then be used to encrypt the rest of the message.

Public key cryptography is a main component of security, in various applications and protocols. 
Various internet standards such as TLS and PGP use Public key cryptography. 

An example in case of PGP is,

![pkc1.jpg](/assets/pkc2.JPG)

A key generation algorithm is used to generate Alice's keys

![pkc2.jpg](/assets/pkc1.JPG)

Bob encrypts the message _HELLO_ using Alice's public key and sends it to her. Alice decrypts it using her private key.

The following is an example of a PGP public key:
```
-----BEGIN PGP PUBLIC KEY BLOCK-----
Comment:
Version:

vn586vy94Nkafgbgaaioief84toew0403n6v1yuI7kXp8NjFmb/x37KeqUHujegAMX09Y
vrEUeyzSrO2FwKgBisIy/0gyw0ucJNd6xSreE
UZGZA46G+fblqQYRf4PeLmR9EsFdgv3orufUjBC+LYZ+bd9mR9EsFdgv3orufUjBC+yZO/0p7JYGrlzbbI0BS+PCj2/4gyw0ucJNd6xSreE
UZGZA46G+fblqQYRf4PeLmR9EsFdgv3orufUjBC+yZO/0p7JYRjyN+K8cl5HzkVDOvkCb0G+1nP
3fNz1xCfwiK5Tghe/iZMxPZVJHgwyIYI+vnGrlzbbI0BS+PCj2/4gyw0ucJNd6xSreE
UZGZA46G+fblqQYRf4PeLmR9EsFdgv3orufUjBC+LYZ+bd9mR9EsFdgv3orufUjBC+yZO/0p7JYRjyN+K8cl5HzkVDOvkCb0G+1nP
3fNz1xCfwiK5Tghe/iZMxPZVJHgwyIfnBkyOt6F4Zvxb64itvn3784ft5f936

-----END PGP PUBLIC KEY BLOCK-----
```
