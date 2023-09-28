# BIP39-XOR
Encrypt or decrypt 12, 15, 18, 21 or 24 BIP39 codewords array (so-called "seed phrase") using exclusive OR (XOR)/Vernam cipher (a.k.a. One Time Pad). If not input by a user, an encryption key is automatically generated at random. Encryption with such a key preserves integrity of BIP-39 checksums of all keys (that's distinct while also compatible with SeedXOR implementation).

```
Usage: BIP39-XOR.bash [codewords...] [XOR] [codewords...]
       BIP39-XOR.bash [--auto-input]
```

EXAMPLES:

`$ bash BIP39-XOR.bash time until select then return void float true false case catch depart`

Encrypt into and output two complementary encryption keys encoded in BIP39 codewords.

`$ bash BIP39-XOR.bash time until select then return void float true false case catch depart XOR age age age age age age age age age age age used`

Use input keys to decrypt and output a key. Or, equivalently, encrypt an input key with another one and output two complementary encryption keys in BIP39 format.

`$ bash BIP39-XOR.bash --auto-input`

Generate input BIP-39 twelve codewords randomly and output two complementary encryption keys encoded in BIP39 codewords.
