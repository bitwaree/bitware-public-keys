# BITWARE PUBLIC KEYS

**This** is the official PGP key repo for bitware, this repo contains latest the keys for signing and encryption purposes. Almost every sensitive binary file distribution from bitware should have a detached signature file, it's always recommended to verify the PGP signature as an extra authenticity measure.  

Please make sure to visit https://github.com/bitwaree/bitware-public-keys to get the latest key.

## To verify a file's authenticity
- ### Download and import the latest key:
    ```bash
    curl -o BITWARE-CURRENT-PUBLIC.txt https://raw.githubusercontent.com/bitwaree/bitware-public-keys/master/BITWARE-CURRENT-PUBLIC.txt
    gpg --import BITWARE-CURRENT-PUBLIC.txt
    ```
- Verify the target file you want:
    ```bash
    gpg --verify <file>
    ```
  
*NOTE*: One should trust the file only if they see:
  ```
  gpg: Good signature from "bitwaree (Please visit https://github.com/bitwaree/bitware-public-keys to get the latest key.) <bitware@duck.com>"
  ```
  with the fingerprint: `5BC6 990A 3B9A DE07 5691  3091 47CA 6351 A62B 1B0A`, that matches [current fingerprint](./BITWARE-CURRENT-FINGERPRINT.txt).

## NOTICEs
- I am creating this repo just to upload keys and make them publically avalible.
- I will not hold responsible for any damage made by untrusted files.
- In case of no circumstances, a key should have a validity of 3 years. After the expiration a new key will be released.
- Expired keys will have their backup too for future verification.

