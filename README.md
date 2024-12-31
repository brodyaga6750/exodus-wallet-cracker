# Decrypt File Script

## Overview

The **Decrypt File Script** is a Python tool designed to decrypt a file by attempting various passphrases from a wordlist. This script uses the Fernet encryption scheme from the `cryptography` library as a placeholder. Be sure to replace the encryption mechanism if a different encryption type is used.

### Features

- **Iterates through Passphrases**: Tries each passphrase from the provided wordlist to decrypt the data file.
- **Efficient and Secure**: Reads file contents and attempts decryption without saving sensitive data to disk.

### Prerequisites

To use this script, you’ll need:

1. Python 3.x
2. Required library: `cryptography`

Install the required library with:

```bash
pip install cryptography
```

### Usage

#### Step 1: Prepare Your Encrypted File and Wordlist

Place your encrypted file and wordlist file in the same directory as the script (or specify the full paths when running the script).

#### Step 2: Run the Script

Run the script by specifying the paths to the encrypted file and the wordlist file.

```bash
py decrypt_file.py <encrypted_file> <wordlist_file>
```

Replace `<encrypted_file>` and `<wordlist_file>` with the actual file names. 

#### Step 3: View Output

If a correct passphrase is found, the script will output:

```
PASSWORD IS: <correct_password>
```

Otherwise, it will print each attempted passphrase index and continue until all passphrases are tested.

### Example

```bash
py decrypt_file.py secret_data.enc wordlist.txt
```

### Limitations

- **Encryption Method**: This example uses `cryptography.Fernet`. Update the script if your file uses a different encryption standard.
- **Wordlist Size**: Processing large wordlists may be slow; use optimized methods or reduce the wordlist size if possible.

### Security Note

Handle decrypted data securely. Store passphrases and sensitive files in secure locations, and avoid sharing or exposing the wordlist to unauthorized access.

---

Let me know if you'd like further customization or have questions about encryption standards!
xncxsguq