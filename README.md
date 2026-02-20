# Advanced Object-Oriented Concepts - Labs Template

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/danielcregg/aooc-labs-template?style=flat-square)

A starter template for the **Advanced Object-Oriented Concepts (AOOC)** lab series. Designed for use with **GitHub Codespaces** and **GitHub Copilot**, it provides a pre-configured Java development environment so students can begin coding immediately.

---

## Prerequisites

- A [GitHub](https://github.com) account with access to **GitHub Codespaces**
- **GitHub Copilot** enabled on your account (recommended)
- Basic knowledge of Java

---

## Getting Started

1. **Create a Codespace** -- Click the **Code** button on the repository page and select **Create codespace on main**.
2. **Wait for Setup** -- The dev container will automatically provision a Java environment with the required VS Code extensions.
3. **Start Coding** -- The file `src/ie/atu/testpackage/Main.java` opens automatically. Follow the lab instructions in class or in your course materials.

### Verify Your Environment

After the Codespace starts, confirm Java is available:

```bash
java --version
javac --version
```

---

## Project Structure

```
aooc-labs-template/
├── src/
│   └── ie/atu/testpackage/
│       └── Main.java            # Entry point (Hello World starter)
├── .devcontainer/
│   └── devcontainer.json        # Codespace configuration (Java, Copilot, extensions)
├── .vscode/
│   ├── settings.json            # Editor and Java project settings
│   └── tasks.json               # Auto-open Main.java on folder open
├── README.md
└── LICENSE
```

---

## Usage

### Compile and Run

From the project root:

```bash
javac -d out src/ie/atu/testpackage/Main.java
java -cp out ie.atu.testpackage.Main
```

Alternatively, use the **Run** button in VS Code with the Red Hat Java extension.

---

## Dev Container

The included `.devcontainer/devcontainer.json` sets up:

- **Java** (latest, via `mcr.microsoft.com/devcontainers/java`)
- **VS Code Extensions**: Red Hat Java, Java Debugger, Java Dependency Viewer, IntelliCode, GitHub Copilot, Markdown Mermaid

---

## License

This project is licensed under the [MIT License](LICENSE).
