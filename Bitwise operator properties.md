# Bitwise operation properties #
--- 
Some necesary properties and equations of bitwise operations.
* a|b  = a⊕b + a&b
* a⊕(a&b)  = (a|b)⊕b
* b⊕(a&bb) = (a|b)⊕a

Addition:
* a+b = a|b + a&b
* a+b = a⊕b + 2(a&b)

Substraction
* a-b = a⊕(a&b) - b⊕(a&b)
* a-b = (a|b)⊕b - (a|b)⊕a
* a-b = a⊕(a&b) - (a|b)⊕a
* a-b = (a|b)⊕b - b⊕(a&b)
---
