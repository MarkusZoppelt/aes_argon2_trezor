# AES with Argon2id and Trezor

Use AES with key generated from Argon2id (password + random salt).
Entropy is generated from Trezor hardware device.

Please look at the [jupyter notebook](aes_argon2_trezor.ipynb) for more explanation.

Contents:

1. Connecting to Trezor hardware device & getting entropy from the device
2. Using Argon2id as a key derivation function (KDF) to generate a 32 byte password hash
3. Initializing AES with the password hash as a symmetric encryption key.