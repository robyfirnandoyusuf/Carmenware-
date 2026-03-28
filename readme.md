# Carmenware - Carmen Ransomware
**© 2026 - greycat**

---


> This project is dedicated to **Carmen** from **Heart2Heart** in celebration of her birthday.
> Happy Birthday, Carmen!

---

<img src="https://i.pinimg.com/736x/5c/d4/2f/5cd42f50a3a602bd80186f6ebed3fe60.jpg" width="400px">

>  This source code is for research purpose only, the use of this code is YOUR RESPONSIBILITY
>  I take NO responsibility and/or liability for how you choose to use any of this source code. 
>  By using of this file, you understand that you are AGREEING TO USE AT YOUR OWN RISK. Once again, 
>  Source code available is for EDUCATION and/or RESEARCH purposes ONLY.

>  Any actions and/or activities related to the material contained within this source code is solely your responsability. Misuse of the information in this source code can result in criminal charges being brought against the persons in question. I will not be held responsible in the event any criminal charges are brought against any individuals misuing the code in this source code to break the law.


A simple Rust ransomware to encrypt files inside image containers and restore them.
This tool appends encrypted data to an image file, allowing the image to remain viewable while secretly storing another file inside it.

# Features

- Hide files inside image containers
- Restore hidden files
- Batch hide/unhide mode
- Custom output image extension
- Automatic file name restoration
- Optional password-based XOR obfuscation
- CLI interface

---

# Installation

Make sure you have **Rust** installed.

https://rustup.rs

Then clone the repository and build:

```bash
git clone https://github.com/robyfirnandoyusuf/Carmenware.git
cd file_hider
cargo build --release
```

Binary will be located at:
`
target/release/Carmenware
`

## Usage
### encrypt files
`Carmenware.exe hide --path .\directory --cover cover.jpg --key <key>`

### decrypt files
`Carmenware.exe unhide --path .\directory --key <key>`
