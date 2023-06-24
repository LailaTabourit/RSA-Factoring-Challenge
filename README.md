
![RSA Image](https://cdn.hashnode.com/res/hashnode/image/unsplash/FnA5pAzqhMM/upload/v1664867430622/yP5GJxzOL.jpeg?w=1600&h=840&fit=crop&crop=entropy&auto=compress,format&format=webp)
 <h2 align="center">RSA Factoring Challenge</h2>

RSA-Factoring-Challenge is a repository dedicated to exploring the fascinating world of RSA encryption and decryption. RSA (Rivest-Shamir-Adleman) is the most widely used public-key cryptography algorithm globally, renowned for its robust security and versatility.

## Introduction

RSA is not just an encryption algorithm; it also serves as a foundation for digital signatures and key exchange. Developed in the 1970s by Ron Rivest, Adi Shamir, and Len Adleman, RSA revolutionized the field of cryptography by leveraging the difficulty of factoring large numbers.

## How RSA Works

RSA utilizes a public-key cryptosystem, employing two keys: a public key and a private key. The public key, known to everyone, is used for encryption, while the private key, held only by the owner, enables decryption. The asymmetric nature of RSA means that the encryption and decryption keys are distinct.

To generate RSA keys, two large prime numbers (p and q) are selected. The modulus (n) is calculated as the product of p and q. Additionally, the totient of n (φ(n)) is computed as (p-1)(q-1).

An integer e is chosen, satisfying the conditions 1 < e < φ(n) and gcd(e, φ(n)) = 1, where gcd(a, b) denotes the greatest common divisor of a and b. This e is referred to as the public exponent and is used for encryption.

The final step is determining d such that ed = 1 mod φ(n). d, known as the private exponent, is used for decryption.

## Encryption and Decryption

With the RSA keys established, the message can be encrypted and decrypted. Encryption involves the computation of the ciphertext (c) using the following formula:

<code>c = m^e mod n</code>

Here, c represents the ciphertext, m denotes the message to be encrypted, and e is the public exponent.

To decrypt the ciphertext, the following formula is used:

<code> m = c^d mod n </code>

Here, m signifies the decrypted message, c represents the ciphertext, and d is the private exponent.
<body>
  <h1>Tasks:</h1>
  <p>This repository contains a program for factorizing numbers into a product of two smaller numbers. The challenge includes two tasks: factorizing arbitrary numbers and the RSA Factoring Challenge. The program can run without any dependencies and has a time limit of 5 seconds.</p>

  <h2>Task 0: Factorize all the things!</h2>
  <p>The task is to factorize as many numbers as possible into a product of two smaller numbers. The program takes a file containing natural numbers to factor, with one number per line. The numbers in the file are assumed to be valid natural numbers greater than 1, and there will be no empty lines or spaces before/after the valid number. The output format for each factorization is <code>n = p * q</code> (where n is the input number and p, q are the factors).</p>

  <h3>Usage</h3>
  <p>To run the program for Task 0, use the following command:</p>
  <pre><code>factors &lt;file&gt;</code></pre>
  <p>Replace <code>&lt;file&gt;</code> with the path to the file containing the numbers to factor.</p>

  <h3>Example</h3>
  <p>Input file (<code>numbers.txt</code>):</p>
  <pre><code>15
21
35</code></pre>
  <p>Output:</p>
  <pre><code>15 = 3 * 5
21 = 3 * 7
35 = 5 * 7</code></pre>

  <h2>Task 1: RSA Factoring Challenge</h2>
  <p>RSA Laboratories states that for each RSA number n, there exist prime numbers p and q such that n = p × q. The challenge is to find these two primes given only n. This task is similar to Task 0, but with the following differences:</p>
  <ul>
    <li>p and q are always prime numbers.</li>
    <li>There is only one number in the input file.</li>
  </ul>
  <p>The goal is to factorize the given number in less than 5 seconds.</p>
<h2>Repository Contents</h2>
  <p>This repository contains the following files:</p>
  <ol>
    <li><code>factors</code>: The executable program for both Task 0 and Task 1.</li>
    <li><code>README.md</code>: This readme file providing an overview of the repository and its contents.</li>
  </ol>
  <p>Feel free to explore the code and use it to participate in the RSA Factoring Challenge or factorize other numbers as required.</p>


## Conclusion

RSA remains the most widely adopted public-key algorithm due to its robust security and versatility. While it relies on the difficulty of factoring large numbers, the algorithm is not without weaknesses. Safeguarding the private key and employing a reliable random number generator are crucial to ensuring its strength.

Discover the power of RSA encryption and decryption, and unlock the realm of secure communication and data protection.

## Resources

To delve deeper into the realm of RSA, consider exploring the following resources:

- [Wikipedia: RSA (cryptosystem)](https://en.wikipedia.org/wiki/RSA_(cryptosystem))
- [Khan Academy: RSA Encryption](https://www.khanacademy.org/computing/computer-science/cryptography/modern-crypt/v/intro-to-rsa-encryption)
- [GeeksforGeeks: RSA Algorithm in Cryptography](https://www.geeksforgeeks.org/rsa-algorithm-cryptography/)
- [Coursera: Cryptography and Information Theory](https://www.coursera.org/learn/crypto) (Online course)
  <p> 
  <h2 id="license">License</h2>
  <p>&copy; 2023 Laila Tabourit</p>
    This repository is licensed under the MIT License. See the <a href="LICENSE">LICENSE</a> file for more information.
  </p>  
**Note:** This repository is intended for educational purposes and should not be used for production systems without proper security considerations.

