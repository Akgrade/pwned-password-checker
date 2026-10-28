# Check My Pass

A Python script that checks if your password has been exposed in a data breach using the [Have I Been Pwned](https://haveibeenpwned.com/Passwords) API. 

This script uses the **k-Anonymity** model. It securely hashes your password locally using SHA-1, sends only the first 5 characters of the hash to the API, and checks the remaining part locally. Your actual password is never sent over the internet.

## Usage

Run the script from your terminal and pass one or multiple passwords as arguments:

```bash
python3 checkmypass.py password123 hello qwerty