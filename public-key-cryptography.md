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

An example of Alice's private and public keys can be see here.
```
-----BEGIN PGP PRIVATE KEY BLOCK-----
Version: 

lQOsBFtfJzoBCADBZ6/nIATLbudrX8PtNZQu6FsEDNz65gD7FQgpwRFkZV/ENrKL
zHmKDU7CZib7NxEEp+fXJ1bIZlbMhgqa/7/R1X78tGpT5+umXBuAEJuyoL05BOgO
1b0q+zjexewJuevGyjuI7hCTUd2ERKfOFhihS1gO+XwJUgWYd15iAunWDKwLFnQB
up/IDwnleFOLUBpqdTcCiTJ/y+PF6WsuiS7/MR7Lv9kBX8H5R8IK+U4EowKxw0SV
ZNb3lSmB+plbKKrHGz/BVpVmfG/UgJNutTp2wN9LTPj4dl04djLeHtT4w2Nt/wri
SL3strAjcw5AtQUqIwnmP4kRDEIdapgmVp+1ABEBAAH/AwMCAOra8vndqQ9gnKpd
rhigzWB91UKsx7bDVKysfMmGRh6kseagBgsZJZQ3AzSkXNkVg32Eq/S/zx11QVI4
JfZlipVitmDy9vVTyytar3mUAeB9fU6XKNFdacQb6i2NAbNdGJUBZjhSWpXVipPt
UvYHvgHu3bIo9hhZZmZbJZ7XeZ/2L6I9CeF1vJOsxo4tv33aFn0XkMtUFClD2ry
Olun/IOIgiSpa8V0klrAHdcp6sJH13ZrSKIztiyr+EnAiT61aMvnbMfP
1EzF11iSlgklNwwkhyt4Ipm2KmAqcJheA1KjMPvrCBxxQgMH76KM2s8HWj5tGiWW
93EaoO0lAVQgNveLrlQdlayBaGb25X5ZBunDgGBwT1zUmYZNet+iGCfVI6I9zVBD
ORLpiKMlTusy5LvhpI0wV4FV52LLl8MsEGcKIQuBWxHOtuAU4IGEVLhxAfLW+0kdE9zzL4ZSX
x/fDYEqVIXVZmphhZZmZbJZ7XeZ/2L6I9CeF1vJOsxo4tv33aFn0XkMtUFClD2ry
Olun/IOIgiSpa8V0klrAHdcp6sJH13ZrSKIztiyr+EnAiT61aMvnbMfP
1EzF11iSlgklNwwkhyt4Ipm2KmAqcJheA1KjMPvrCBxxQgMH76KM2s8HWj5tGiWW
93EaoO0lAVQgNveLrlQdlayBaGb25X5ZBunDgGBwT1zUmYZNet+iGCfVI6I9zVBD
ORLpiKMlTusy5LvhpI0wV4TJ/ON/h85KMONcOs1gdwR9ZgPf/foSXEs0397T+o7t
J4MSra8etsNvsurk77euIdZwzqd4n9Ft1s/Piw7AorQAiQEcBBABAgAGBQJbXyc6
AAoJEEY9Grfgd3/m/EUIAKgQCJoKcxC6DDNlf1u4AXj5rcGKCPc/TFVDivXNufZJ
lJcBbc6+LsNIEIlfraaFRpTOYhKzB8aPlLnHkb/kJMelRCbKG1xAVrYJnV34hRxa
N6GkiWhzwahCD6vmMXI6fi+OVXMBrwYoTEZimo+jUeK5FX+uRxz9eJhSCqAtQCXX
gVuVtk+0xKu+d/+YqA0Gsz0Jo1EKuL+AbhbPyDPkqD0ZM87qgogj8gE+aL/SV/5w
g5dTZn0FBJPD00p8X9S5qpNh3YtLZl3VpQbB2bqNNvEoUR4nLrzBrPf1bAJpxs9y
M9CmO+mOfnxuqq3nPDCprfXp79HugltGOZVN1QWyNCg=
=nPDk
-----END PGP PRIVATE KEY BLOCK-----
```

```
-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: 

mQENBFtfJzoBCADBZ6/nIATLbudrX8PtNZQu6FsEDNz65gD7FQgpwRFkZV/ENrKL
zHmKDU7CZib7NxEEp+fXJ1bIZlbMhgqa/7/R1X78tGpT5+umXBuAEJuyoL05BOgO
1b0q+zjexewJuevGyjuI7hCTUd2ERKfOFhihS1gO+XwJUgWYd15iAunWDKwLFnQB
up/IDwnleFOLUBpKExGYfXJ1bIZlbMhgqa/7/R1X78tGpT5+umXBuAEJuyoL05BOgO
1b0q+zjexewJuevGyjuI7hCTUd2ERKfOFhihS1gO+XwJUgWYd15iAunWDKwLFnQB
up/IDwnleFOLUBpKExGYpqPo1HiuRV/rkcc/XiYUgqgLUAl
14FblbZPtMSrvnf/mKgNBrM9CaNRCri/gG4Wz8gz5Kg9GTPO6oKII/IBPmi/0lf+
cIOXU2Z9BQSTw9NKfF/UuaqTYd2LS2ZdpqPo1HiuRV/rkcc/XiYUgqgLUAl
14FblbZPtMSrvnf/mKgNBrM9CaNRCri/gG4Wz8gz5Kg9GTPO6oKII/IBPmi/0lf+
cIOXU2Z9BQSTw9NKfF/UuaqTYd2LS2Zd1aUGwdm6jTbxKFEeJy68waz39WwCacbP
cjPQpjvpjn58bqqt5zwwqa316e/R7oJbRjmVTdUFsjQo
=Pl2l
-----END PGP PUBLIC KEY BLOCK-----
```
