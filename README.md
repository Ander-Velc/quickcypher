# quickcypher
QuickCypher is a lightweight command-line tool written in Python that allows users to quickly encrypt and decrypt text using Fernet, a secure symmetric encryption scheme based on AES.

## 🚀 Use cases
- Quick encryption of sensitive information
- Learning practical cryptography concepts
- Simple automation from Bash scripts


## Usage:

- Encrypt text
`python3 quickcypher.py --text "secret message"`

- Decrypt text
`python3 quickcypher.py --decrypt "<encrypted_token>" --key "<encryption_key>"`

You can also add this tool in your bashrc to make it easier to use:
```bash
function encrypt() {
        python3 $PATH --text "$1"
}

function decrypt() {
        echo -n "Enter key: "
        read -r key
        python3 $PATH -d "$1" -k $key
}
````
<img width="2252" height="208" alt="image" src="https://github.com/user-attachments/assets/0afcebea-2ae0-4a48-b574-d1ed77808fc5" />

<img width="2282" height="174" alt="image" src="https://github.com/user-attachments/assets/9f0660c4-7349-405e-b8e4-f79b17109c8e" />



## ⚙️ Requirements
- Python 3.8+
- `cryptography` library

## 📦 Installation
```bash
pip install -r requirements.txt
