# Cryptography

## The Numbers - 50 Points

The numbers given to us are the values of letters within in the alphabet. 

We can use [this website](https://www.dcode.fr/letter-number-cipher) to quickly decode to the numbers.

16 9 3 15 3 20 6 { 20 8 5 14 21 13 2 5 18 19 13 1 19 15 14 }

<img src="images/The Numbers1.png">

The flag for this challenge is `PICOCTF{THENUMBERSMASON}`

## caesar - 100 Points

In this challenge, we are given ciphertext with a caesar cipher encoded string. 

<img src="images/caesar1.png">

Take the contents within the curly braces, and put it into [this website](https://www.dcode.fr/caesar-cipher) to decode the string. Brute force the shift until the text becomes legible (the shift should be 22).

<img src="images/caesar2.png">

The flag for this challenge is `picoCTF{crossingtherubiconvfhsjkou}`

## Easy1 - 100 Points

In this challenge, we are told to decrypt a one time pad cipher encoded string.

We are given: the ciphertext `UFJKXQZQUNB`, the key `SOLVECRYPTO`, and the table.  

You can either solve this simply by putting these elements into [this website](https://www.boxentriq.com/code-breaking/one-time-pad), or do it the more *fun* way, which is to manually decode it. 

In order to decrypt the message, we have to work backwards. To derive a cleartext value from a ciphertext letter, you need to choose the row that corresponds with the first letter of the key. Then within that row, find the letter of the ciphertext. Once found, highlight the column and see which letter it corresponds to; that letter should be the first letter of the cleartext. Keep repeating these steps with every letter in the ciphertext, in relation with every letter in the key.  

<img src="images/Easy11.png">

The flag for this challenge is `picoCTF{CRYPTOISFUN}`
