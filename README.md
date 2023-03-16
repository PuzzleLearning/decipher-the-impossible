# Decipher the impossible

Nobody yet deciphered the message, including me. Can you?

## The puzzle

```
\/\/}{1(}{ 0|= +}{3 |=0|_|_0\/\/1/\/6 +3(}{/\/10_I_I3$ (4/\/ 83 I_I$3|) |=0|2 +}{3 |>I_I|2|>0$3 0|= |{3'/\/\/0|2|) /\/0|2/\/\4|_1%4+10/\/, +}{3 |>|20(3$$ 0|= (0/\/\/3|2+1/\/6 4 |{3'/\/\/0|2|) 1/\/+0 1+$ 84$3 |=0|2/\/\?
```

`1. |_3/\/\/\/\4+1%4+10/\/`

`2. |_3\/3/\/$}{+31/\/`

`3. $+3/\/\/\/\1/\/6`

`4. $0I_I/\/|)3><`

## Cracking it

### Automated approach 

I tried to use the `ciphey` tool (available here: [Ciphey](https://github.com/Ciphey/Ciphey)) for checking out-of-box all common cipher techniques with a single command. 

```bash
brew install ciphey
ciphey -t "the text from the puzzle..."
```

In the result, nothing usefull is returned at all. Program kind of freezes on the "thinking" stage, without yielding anything more for the whole 10 mintes. This framework doesn't seem to paralelize well on the MacOS system (only one cpu core is used).  

## Next steps to try

### Ciphey tuning

#### Lot of escape chars in the text

I have a suspicious some characters maybe be scrambled, possibly lot of slash/backslash sequences attack automated decyphers like cyphey

#### Using ciphey with a custom word list

Maybe it's not written in English language, so the ngram analysis fail. 

#### The encrypted entity is not actually a text, but a set of emojis. 

Self-explanatory, investigate

### Encrypted text is actually a computer code

Encrypted Python code? Isoteric programming language? 

### Brute-forcing my way in? 

Maybe we could check all possible combinations of association table within the alfanumerical alphabet (optionally with special characters), together with checking if the output is a real language (human or a programming code). 
