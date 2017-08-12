%title: Numbers & Bits
%author: hellerve
%date: 2017-10-08

-> Guess what this piece of code does <-

---

-> IEEE 754 Floating Point addition! <-

---

-> I fiddle with numbers all the time <-

-> I have no idea how they work <-

---

-> IEEE, how do I do rounding? <-

---

- If the last bit shifted out was zero, just truncate
- If the last bit shifted out was 1 and there was at
  least one more 1 in all of the other bits that were
  shifted out, add 1 to mantissa
- Otherwise round mantissa up by one if the manissa’s
  lowest bit contains a one

---

-> 💩 <-

---

-> Lemma 1: All of our computational systems are 💩 <-

---

-> Lemma 1: All of our computational systems are 💩 <-

-> Lemma 2: numbers in computation are abstract computational systems <-

---

-> Lemma 1: All of our computational systems are 💩 <-

-> Lemma 2: numbers in computation are abstract computational systems <-

-> Corollary 1: numbers in computation == 💩 <-

---

-> What did I want to talk about again? <-

---

-> Binary Coded Decimals <-

https://github.com/hellerve/nibbles

---

- decimal digits stand on their own
- we need to represent numbers from 0 to 9
- a little more than 3 bits of information

---

- packed:
  - pack into a nibble[1]
  - throw away ~0.5 bit of information
- unpacked:
  - pack into a byte
  - throw away ~4.5 bit of information

1: fun fact: nibble is an actual technical term

---

-> Why would you want that? <-

---

-> Main reason: because you’re lazy and it’s easy <-

- Infinite precision numbers
- Decimal computers
- Financial & bureaucratic systems
- [...]

---

-> Lemma 3: It’s just a silly hack around how awful our numbers are <-

---

-> Fixed Point Numbers <-

https://github.com/hellerve/silly

---

- Fixed width for fractional and integral part
- Cool if you know that your values are restricted
- Terrible in many other ways

---

- You can store number as integer and do integer
  arithmetic on it
- Actually works!

---

- ... as long as you don’t mind integer precision in
  division

---

- ... as long as you don’t mind constant brutal overflows
  in multiplication

---

-> Lemma 4: 💩 <-

---

-> Floating Point Numbers <-

https://github.com/hellerve/silleee

---

- IEEE 754: great specs

---

- You have _to pay to see the specs_ ($100)
- wtf.

---

- I p̶i̶r̶a̶t̶e̶d̶ bought the specs
- 70 pages of unreadable legalese

---

-> Confession: I never got past addition and subtraction <-

---

-> Lemma 5: I give up. <-
