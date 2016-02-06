# PHP Identity and Data Security

### Jonathan LeBlanc | @jcleblanc | book: bit.ly/idatasecurity

## Protecting Against Password Attacks

* **Brute Force Attack**

    * Calculate all key variations within a given length, then trying one until password is guessed.

    * **Protect via: Key stretching, CAPTCHA, 2 factor Auth**

* **Dictionary Attacks**

    * Use a list of predetermined words/phrase to guess password.

    * **Protect via: Salting**

* **Rainbow Table**

    * Use precalculated password hashes to break encryption

    * **Protech via: Salting**

## Considerations when using Salts

* **Storing Salts**

    * Store alongside the hash

* **Salt reuse**

    * Salts should be unique per password

* **Salt Length**

    * Same size as hash? 128bits is ideal

## Password Encryption Algorithms

* **bcrypt**

    * designed for password security, base on the blowfish cipher, CPU & RAM intensive.

* **PBKDF2**

    * Comes from RSA laboratories, performs the HMAC (hash + key) over a specific number of iterations.

* **scrypt**

    * Designed to make costly to perform large-scale hardware attacks by requiring large amounts of memory. 

SLIDES: http://bit.ly/ssphp_id_data

