# HabBit
This application is capable of modifying  Habbo's game client to allow it to run anywhere, from anywhere, with custom RSA keys.

[Latest Release(s)](https://github.com/ArachisH/HabBit/releases)  
*This application will take a maximum of 5 seconds without compressing(+10 with compression), and updating headers(+4) to finish.*

## Requirements
* .NET Framework 4.5
* (Source Only)IDE with C# 6 support.

## Capabilties
* Bypass local/remote host checks.
* Dump Outgoing/Incoming message data(header, hash, ctor, parser).
* Update Outgoing/Incoming header files from a previous client revision.
* Public RSA key replacement, with the option to generate new 1024-bit keys.

## Commands/Arguments
* `-compress` - Will compress the file once it has been assembled.
* `-rsa modulus exponent` - The custom RSA public key pair to use when replacing the client's RSA keys.
* `-dumph` - Will create a text file containing the Outgoing/Incoming message data(header, hash, ctor, parser).
* `-updateh previous.swf outFile.* inFile.*` - Updates the Outgoing/Incoming headers files(Relative to client) of a previous client, to the current one.

Default RSA Keys
```
E:3

N:86851dd364d5c5cece3c883171cc6ddc5760779b992482bd1e20dd296888df91b33b936a7b93f06d29e8870f703a216257dec7c81de0058fea4cc5116f75e6efc4e9113513e45357dc3fd43d4efab5963ef178b78bd61e81a14c603b24c8bcce0a12230b320045498edc29282ff0603bc7b7dae8fc1b05b52b2f301a9dc783b7

D:59ae13e243392e89ded305764bdd9e92e4eafa67bb6dac7e1415e8c645b0950bccd26246fd0d4af37145af5fa026c0ec3a94853013eaae5ff1888360f4f9449ee023762ec195dff3f30ca0b08b8c947e3859877b5d7dced5c8715c58b53740b84e11fbc71349a27c31745fcefeeea57cff291099205e230e0c7c27e8e1c0512b
```

## Console Interface
![HabBit](http://i.imgur.com/C3vcnFO.png)
