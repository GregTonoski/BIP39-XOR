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

## Screenshots
![image](https://github.com/GregTonoski/BIP39-XOR/assets/111286121/d9ed7f32-59a0-42ae-b5c2-32f47938fdb0)

![image](https://github.com/GregTonoski/BIP39-XOR/assets/111286121/a5e417b2-3c76-4650-b5e0-f50b09a703cc)

## Launch on Windows
In order to download and run the program on Windows, open PowerShell application and copy-paste this line:
```
Invoke-WebRequest -URI "https://github.com/GregTonoski/BIP39-XOR/releases/download/v4.1.0/busybox.exe" -OutFile "$HOME\busybox.exe" ; Invoke-WebRequest -URI "https://raw.githubusercontent.com/GregTonoski/BIP39-XOR/main/BIP39-XOR.sh" -OutFile "$HOME\BIP39-XOR.sh" ; Start-Process "$HOME\busybox.exe" "bash BIP39-XOR.sh"
```
The next time BIP39-XOR.sh the shorter command (without downloading) will start the program: `cd $HOME; .\busybox.exe bash BIP39-XOR.sh`.

The BIP39-XOR.sh will start by double-clicking the file icon if [Git for Windows](https://git-scm.com/downloads) is installed (with the default file association settings).

Alternatively, [Windows Subsytem for Linux](https://learn.microsoft.com/en-us/windows/wsl/install), [MSYS2](https://www.msys2.org/) or [Cygwin](https://www.cygwin.com/) must be installed in order to launch BIP39-XOR.sh on Windows.
## Launch on Linux, Unix, BSD, ChromeOS and MacOS
Download and run from a terminal: 
```
curl -fsSL "https://raw.githubusercontent.com/GregTonoski/BIP39-XOR/main/BIP39-XOR.sh" > BIP39-XOR.sh && bash ./BIP39-XOR.sh
```
Optionally make the file executable ( `$ chmod +x BIP39-XOR.sh` ) to run it in by the shorter `./BIP39-XOR.sh` command subsequently.
## Launch on Android
Open the BIP39-XOR.sh file from a terminal app, e.g. [Termux](https://play.google.com/store/apps/details?id=com.termux) or SSH.
## Launch on iOS
Open the BIP39-XOR.sh file from a terminal app, e.g.  [iSH Shell](https://apps.apple.com/us/app/ish-shell/id1436902243) or SSH.
## Launch on embedded and other systems
The program is compatible with Portable Operating System Interface (POSIX) shells so should run on various electronic devices. The launch methods should be similar to the ones described for other systems altough may differ in details and depend on a device.
