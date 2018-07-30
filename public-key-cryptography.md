##	Public Key Cryptography

It refers to any system that uses key pairs and, is also called asymmetric key cryptography.
There are two keys involved: 
* public key, known to every one and  
* private key only known to the owner.  

Both keys have a one-to-one relation with each other i.e. there is a single private key for each public key. Also, documents can be digitally signed, using the private key, which can be verified using the public key, hence giving a proof of ownership/identity and proof of intent. In this system, any person can encrypt a message using the receiver’s public key, 
but the message can be decrypted only by the receiver’s private key.
Due to the complex nature of asymmetric encryption, it is usually used only to transfer small bytes of data, 
like a symmetric encryption key. This key may then be used to encrypt the rest of the message.

Public key cryptography is a main component of security, in various applications and protocols. 
Various internet standards such as TLS and PGP use Public key cryptography. 

#### Example:
![pkc1.jpg](/assets/pkc2.JPG) ![pkc2.jpg](/assets/pkc1.JPG)

Alice generates a public-private key pair using a key generator algorithm.
The public key maybe made available on keyservers and can be shared by Alice. Bob encrypts the message he wishes to send using her public key, and Alice decrypts it using her private key.An example of Alice's private and public keys, as well as the message can be see here.
```
-----BEGIN PGP PRIVATE KEY BLOCK-----
Version: BCPG C# v1.6.1.0

lQOsBFtfKWoBCACgkqqmsqfOws9ekPJNMoorpQVHIz5YNbiqzf4gAh1JpmY2Bdw1
soTfDayOjNRCOqpHW85vw14JNGjsWlSmy+FoCWmP+oEDdo8q8EabnwSS8oIhjC9X
6l3m0zaC1GXw0ZP/5lvWvPYscSA+7OlFq9Sc8Y3kfdfNbubYZRam3WuMNFk28aTY
zQGOvUlOb5cPlEnsnvwME7OaAjEC8NLAa958wNfi30fD6W2nvkf5X0OKKfRoL18J
1p58TnQtoR4jL7AvU3alx/8rPKyOVbMiPYdc2nC/kGR29t0Gba1r/x6SYDOkGrlF
HpM8TcT5VDK2TzFxnH0CIYVQuAJz7lXHEI8HABEBAAH/AwMCyHT3cv46zopgsQUz
ZOPP8oBZkB8QuNSTrv0iMm1MlJI8ypPuMr575jtJkViw2uy3FskX/un/xAm+tXe4
y4E9kf94OwCLSh6WceXZSujwucj9zJpQp/NF0lADYnmNHEPphJhP04JyvB7Qgh5E
ukjj1I3nbz+eHZu/7d237J0pjZ5IZZRlg2F1STsK05zXGFNu0d2KTVV24y6sQGjW
BhfWhlPfyIZErSXW2VpRd4jSEVkF4+z5aMZFU42VG8FxfG27rcBoBskszfkzR//B
B09kvTXz8NZ8F2NR661UtTzbkvoN46lELnNYtV0I53KKzNSvPvRioTsXE5hIvE11
S/vMsCGs2PlF3YnYZUcYaAbOKIGD0JJOmbPGZ9l8XZi7LiG+oCu2Bmt5zwg2AEd/
u+SMGLw4gzO64JGKv/m0RSrtmhehymPzFG3GLArSJpCyj9871dW8jzX5TXhpd1Ge
Qbs92GSs3CX+v8P5gXf7ooJE3lc2vWPA0p7x33/3zaHQpK8EVY2xfB0yV7zIWUPp
wBitaRhoyLQlAI/MwIIVnMXNmWq5wxGuzIp4ADdH4f62paO2QXU82/+oLOotsuLd
HS2E8mGzPVf4VMB6J+9u1jV4EBR+/ejC25PGreD/lyipRxn2Xz7B1woW0DOdozY7
DHPxJYJK2cf+AzRUCy4cyxHlMX/bTM1tcncZ/xN32Ttbvm/4UqWTMTYDQV7IsNku
uTKayuvB2NmSIJCu1+U/jW51zKZFXwGusKa9gXme+mp2CW1SOXp4DA/IeJiZOdiW
plETg8MHoiocrI0cMwHjXiLdL06k/mPi+RR3EVIedSzHbIit9eyM6UuK17082zZn
wZRD2zr9nUgmU23gBk+GZSsbVuLR60/nqg8rSy5r/rQAiQEcBBABAgAGBQJbXylq
AAoJEEdO99lHU7E2NJ0H/ikDttfEmCtsF708Z9taE2Vt/F0rStdVHJyRTOsbHoHr
MJzi0OpDtcq93tJ0Fm+tzHjmITgDZZImRPU4jnS0jSEbQOQAw7ZzdoltH1L51mvh
1Wkf6dqRMX03o4nbTsB2fJC7YhfS9BccAGLETeRUFYKqjBD5zB2E45GIuEtC7vEl
WA19qSxSMS0GbdkErDdy4zN64El09X6WPcxr7qNB37h1Kh4S6Q9RV4+kSgSmsAjs
5FNtDcYj5vJBJXDHRrLljjz+7FQ/KWLXBK3j7Oh7ZOVJzvkboXDdd1JmMvgQ5HiV
19hPPMKi1zx7Q3xJmtSj6nQ6jeOmKXVBP0JVfZ3NvdM=
=HyZr
-----END PGP PRIVATE KEY BLOCK-----

```

```
-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: BCPG C# v1.6.1.0

mQENBFtfKWoBCACgkqqmsqfOws9ekPJNMoorpQVHIz5YNbiqzf4gAh1JpmY2Bdw1
soTfDayOjNRCOqpHW85vw14JNGjsWlSmy+FoCWmP+oEDdo8q8EabnwSS8oIhjC9X
6l3m0zaC1GXw0ZP/5lvWvPYscSA+7OlFq9Sc8Y3kfdfNbubYZRam3WuMNFk28aTY
zQGOvUlOb5cPlEnsnvwME7OaAjEC8NLAa958wNfi30fD6W2nvkf5X0OKKfRoL18J
1p58TnQtoR4jL7AvU3alx/8rPKyOVbMiPYdc2nC/kGR29t0Gba1r/x6SYDOkGrlF
HpM8TcT5VDK2TzFxnH0CIYVQuAJz7lXHEI8HABEBAAG0AIkBHAQQAQIABgUCW18p
agAKCRBHTvfZR1OxNjSdB/4pA7bXxJgrbBe9PGfbWhNlbfxdK0rXVRyckUzrGx6B
6zCc4tDqQ7XKvd7SdBZvrcx45iE4A2WSJkT1OI50tI0hG0DkAMO2c3aJbR9S+dZr
4dVpH+nakTF9N6OJ207AdnyQu2IX0vQXHABixE3kVBWCqowQ+cwdhOORiLhLQu7x
JVgNfaksUjEtBm3ZBKw3cuMzeuBJdPV+lj3Ma+6jQd+4dSoeEukPUVePpEoEprAI
7ORTbQ3GI+byQSVwx0ay5Y48/uxUPyli1wSt4+zoe2TlSc75G6Fw3XdSZjL4EOR4
ldfYTzzCotc8e0N8SZrUo+p0Oo3jpil1QT9CVX2dzb3T
=q5t3
-----END PGP PUBLIC KEY BLOCK-----

```

```
-----BEGIN PGP MESSAGE-----
Version: BCPG C# v1.6.1.0

hQEMA0dO99lHU7E2AQgAhltsAxHHqbWjNDnr2Wvk5Ovy6TWvw48Q69BlHYqO6aTv
WXOLH8fW9oNyMU8q+pVDuYN7URDwz4yyLBQyst+7okM74hto753namCozu/tOOF5
TM7LFBxvnphkTot34kI9NVpw4lBZl/sp8ALiEEchlPXcNOzlwsmXM7Hegb0NzgfE
xTX+ArbWndZKKzpfc2jeoYalFc6W9Ird23oXn7AbylCLfuqeKtMPrI2nE8Wau58L
T5WzEZsboHkhTPBOjZ0FVOHDC4ENB8fj1zJC4r6ADCRLqMX/MgwlfkkMByxvt9sw
+ELG0ZyRwaCtheOf7SWKCQ8jQydMSasVZ0THbUEYG8kryVBfEz6R8dJjcoa90j6/
aAV/5cqsW5F4eao2jANv2KjIJ0OEpero5janjQ==
=BDlJ
-----END PGP MESSAGE-----
```

Keys and message generated [here](http://www.igolder.com/pgp/).
