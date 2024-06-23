# CaughtMe v0.1

**CaughtMe** is a simple Bash tool for encrypting and decrypting files using AES-256 encryption. It provides an easy-to-use command-line interface to secure your files with password protection.

## Features

- Encrypt `.txt` (current version) to `.tru` (encrypted) format.
- Decrypt `.tru` (encrypted) files back to their original format.
- Optional password protection for encryption and decryption.
- User-friendly ASCII art interface.

## Requirements

- Linux (Bash shell) or Termux on Android
- OpenSSL command-line tool (`openssl`)

## Installation

### On Linux

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/sameerahmad005/CaughtMe.git
   cd CaughtMe
   ```

2. **Make the Script Executable:**

   ```bash
   chmod +x CaughtMe
   ```

3. **Install OpenSSL (if not already installed):**

   - Debian/Ubuntu:

     ```bash
     sudo apt-get update
     sudo apt-get install openssl
     ```

   - CentOS/RHEL:

     ```bash
     sudo yum install openssl
     ```

4. **Run the Script:**

   ```bash
   ./CaughtMe
   ```

### On Termux (Android)

1. **Install Termux:**

   Install [Termux](https://termux.com/) from the Google Play Store or F-Droid.

2. **Install Required Packages:**

   Open Termux and install OpenSSL:

   ```bash
   pkg install openssl
   ```

3. **Clone the Repository:**

   ```bash
   git clone https://github.com/sameerahmad005/CaughtMe.git
   cd CaughtMe
   ```

4. **Make the Script Executable:**

   ```bash
   chmod +x CaughtMe
   ```

5. **Run the Script:**

   ```bash
   ./CaughtMe
   ```

## Usage

1. **Follow the On-Screen Instructions:**

   - Choose `1` to encrypt a file. You will be prompted to enter the file location and optionally set a password.
   - Choose `2` to decrypt a file. You will be prompted to enter the file location and, if password-protected, the decryption password.
   - Choose `3` to exit the tool.

2. **Notes:**

   - Ensure to provide valid file paths compatible with your operating system.
   - Passwords are required for decryption only if the file was password-protected during encryption.

## Contributing

Contributions are welcome! Feel free to fork the repository, make improvements, and submit pull requests. If you have suggestions or encounter issues, please open an issue on GitHub.

## Future Plans

- Additional file formats for encryption.
- Improved error handling and user feedback.
- Support for more advanced encryption options.

## Example

Encrypting a file:

```
$ ./CaughtMe

 ██████╗ █████╗ ██╗   ██╗ ██████╗ ██╗  ██╗████████╗    ███╗   ███╗███████╗    
██╔════╝██╔══██╗██║   ██║██╔════╝ ██║  ██║╚══██╔══╝    ████╗ ████║██╔════╝    
██║     ███████║██║   ██║██║  ███╗███████║   ██║       ██╔████╔██║█████╗      
██║     ██╔══██║██║   ██║██║   ██║██╔══██║   ██║       ██║╚██╔╝██║██╔══╝      
╚██████╗██║  ██║╚██████╔╝╚██████╔╝██║  ██║   ██║       ██║ ╚═╝ ██║███████╗    
 ╚═════╝╚═╝  ╚═╝ ╚═════╝  ╚═════╝ ╚═╝  ╚═╝   ╚═╝       ╚═╝     ╚═╝╚══════╝    
 BY SAMEER                                                                       

Choose an action: 
1. Encrypt a file
2. Decrypt a file
3. Exit
Enter 1, 2, or 3: 1

Enter the location of the file to encrypt or 'back' to return: /path/to/your/file
Do you want to add password protection? (yes/no): yes
Enter password for encryption: 
Confirm password: 
File encrypted successfully to /path/to/your/file.tru
Press Enter to return to the main menu.
```

Decrypting a file:

```
$ ./CaughtMe

 ██████╗ █████╗ ██╗   ██╗ ██████╗ ██╗  ██╗████████╗    ███╗   ███╗███████╗    
██╔════╝██╔══██╗██║   ██║██╔════╝ ██║  ██║╚══██╔══╝    ████╗ ████║██╔════╝    
██║     ███████║██║   ██║██║  ███╗███████║   ██║       ██╔████╔██║█████╗      
██║     ██╔══██║██║   ██║██║   ██║██╔══██║   ██║       ██║╚██╔╝██║██╔══╝      
╚██████╗██║  ██║╚██████╔╝╚██████╔╝██║  ██║   ██║       ██║ ╚═╝ ██║███████╗    
 ╚═════╝╚═╝  ╚═╝ ╚═════╝  ╚═════╝ ╚═╝  ╚═╝   ╚═╝       ╚═╝     ╚═╝╚══════╝    
 BY SAMEER                                                                       

Choose an action: 
1. Encrypt a file
2. Decrypt a file
3. Exit
Enter 1, 2, or 3: 2

Enter the location of the file to decrypt or 'back' to return: /path/to/your/file.tru
File decrypted successfully to /path/to/your/file
Press Enter to return to the main menu.
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
