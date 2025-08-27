Python2Go Transpiler

Python2Go is a blazing-fast transpiler written in Rust that converts Python code into equivalent Go code. It’s designed for developers who want to migrate Python projects to the Go ecosystem without rewriting everything manually.

This project is fully open-source under the Apache 2.0 license, and precompiled binaries are available in the Releases section.

---

✨ Features

- 🔁 Translates core Python syntax to idiomatic Go
- 🧠 Supports functions, conditionals, loops, and variable assignments
- 🧩 Modular architecture for easy extension
- ⚡ High performance powered by Rust
- 📄 Clean and readable Go output

---

📦 Installation

Option 1: Download from Releases

Visit the Releases page and download the binary for your platform.

Option 2: Build from Source

`bash
git clone https://github.com/yourusername/python2go
cd python2go
cargo build --release
`

The compiled binary will be located at target/release/python2go.

---

🚀 Usage

`bash
./python2go path/to/script.py -o output.go
`

- path/to/script.py: Path to your Python source file
- -o output.go: Destination file for the generated Go code

---

📖 Example

Input (Python):

`python
def greet(name):
    print("Hello, " + name)

greet("Matin")
`

Output (Go):

`go
package main

import "fmt"

func greet(name string) {
    fmt.Println("Hello, " + name)
}

func main() {
    greet("Matin")
}
`

---

🧠 Project Structure

| File           | Purpose                                  |
|----------------|------------------------------------------|
| parser.rs    | Parses Python code into an AST           |
| transpiler.rs| Converts AST into Go code                |
| cli.rs       | Handles command-line interface and I/O   |

---

🔭 Roadmap

- ✅ Class and inheritance support
- ✅ List and dictionary translation
- ⏳ Exception handling
- ⏳ Async/await conversion
- ⏳ Unit tests and improved documentation

---

🤝 Contributing

We welcome contributions from the community! To get started:

1. Fork the repository
2. Create your feature branch (git checkout -b feature/foo)
3. Commit your changes (git commit -am 'Add new feature')
4. Push to the branch (git push origin feature/foo)
5. Create a new Pull Request

---

📄 License

This project is licensed under the Apache License 2.0.  
You are free to use, modify, and distribute this software under the terms of the license.  
See the LICENSE file for full details.

---

💬 Contact

For questions, suggestions, or collaboration ideas, feel free to open an issue or reach out via Telegram.

---

Made with ❤️ in Rust by Matin.
