#### SSH - secure shell / Secure Shell Protocol

One of the ways to secure the communication across different devices (ex: your computer and computer of your friend; your computer and a remote server).
It's a more secure alternative to password authentication. It uses a cryptographic key pair instead of passwords.

To establish the secure communication you use an **SSH key-pair**
- 1st SSH-key is used to encode the message/data when sending. PUBLIC KEY - the one that you can give to anyone you want to securely communicate with.
- 2nd SSH-key is used to decode the message/date on the recieving device. PRIVATE KEY - never give this to anyone! Your way to ensure only you can encode the message.

Technically any length key with any algrorithm used for encoding can be decoded by hacker, but important question is: How long does it take?!
SSH-key is designed to be long enough to ensure that hacking takes that long to be irrelevant at the time it's been decoded (eg. 15 years).

Some applications automate the process of exchanging the keys, while others (eg. GitHub) need keys to be added manually.

Modern **SSH clients support multiple key algorithms**, including **Ed25519, RSA, ECDSA**.
- Ed25519 is genereally recommended for modern systems dur to its strong security and smaller key size.
- RSA though remains widely compatible with older systems

*Check the article in sources if you want to know the commands to generate an SSH key-pair, use a specific configuration or a multiple SSH identities.*

#### Sources: [How to Set Up SSH Keys on Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys-on-ubuntu-20-04)