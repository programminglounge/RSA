# RSA

In this repository I implement the RSA cryptosystem using javascript and plain HTML to practice working on other languages aside from c++ and python. 
In this project I am using the / symbol as a delimiter of texts. the HTML file consists of a few functions (like gcd, finding a decryption value, finding an encryption value, finding a prime and etc.) which each are needed to implement the RSA cryptosystem. <br><br>
In the RSA cryptosystem we need to find two prime numbers p and q such that p and q are not equal to eachother <br>
We then multiply p and q together to form the number n. <br>
We calculate the phi(n) function which is (p-1)*(q-1) <br>
We choose a value e, such that 1<e<phi(n) where e and phi(n) are coprime.<br>
We find a d value such that (d*e) % phi(n) = 1 <br>
The public key is the pair (e, n) and the private key is the pair (d, n)

Example: p = 11, q = 13 -> n = 143 <br>
phi (n) = 10*12 = 120 <br>
lets choose e = 7, one choice for d = 41 <br>
lets choose the message m = 5 <br>
then the cipher text = 5<sup>7</sup> % 143 = 47 <br>
the original plaintext = 47<sup>41</sup> % 143 = 5 <br>

In my example I used the ascii code for each character as the message m and used the RSA cryptosystem where p and q are random prime numbers to encrypt and decrypt the message  
