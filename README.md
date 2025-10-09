# ghcptest

![.NET Console App CI](https://github.com/pdebruin/ghcptest/workflows/.NET%20Console%20App%20CI/badge.svg)

A simple .NET console application for testing GitHub Copilot.

## Building the Application

To build the application, run:

```bash
dotnet build src/ConsoleApp/ConsoleApp.csproj
```

## Running the Application

To run the application, use:

```bash
dotnet run --project src/ConsoleApp/ConsoleApp.csproj
```

## Requirements

- .NET 9.0 SDK or later
Welcome to **ghcptest** - a test repository for GitHub Copilot! 👋

## 📖 Project Description

This repository serves as a testing ground for GitHub Copilot features and capabilities. It's designed to help developers explore, experiment with, and validate GitHub Copilot's code generation, completion, and assistance features in a safe, dedicated environment.

Whether you're new to GitHub Copilot or an experienced user looking to test specific scenarios, this repository provides a space to learn and experiment.

## 🚀 Getting Started

### Prerequisites

- Git installed on your local machine
- A GitHub account
- GitHub Copilot subscription (optional, but recommended for full functionality)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/pdebruin/ghcptest.git
   cd ghcptest
   ```

2. You're ready to start experimenting!

## 💡 Usage Instructions

This repository can be used to:

- **Test GitHub Copilot suggestions**: Create new files and see how Copilot assists with code completion
- **Experiment with different programming languages**: Try various languages to see how Copilot adapts
- **Practice prompt engineering**: Learn how to write better comments and prompts for Copilot
- **Validate workflows**: Test GitHub Copilot integration with your development workflow

### Example Workflow

1. Create a new file in your preferred programming language
2. Write a descriptive comment about what you want to build
3. Let GitHub Copilot suggest implementations
4. Review, modify, and iterate on the suggestions

## 🎬 Marp Presentation

This repository includes a Marp presentation demonstrating the project. The presentation is automatically built and deployed to GitHub Pages.

- **Presentation source**: [`marp/slides.md`](marp/slides.md)
- **View online**: [https://pdebruin.github.io/ghcptest/](https://pdebruin.github.io/ghcptest/)
- **Learn more**: See the [Marp README](marp/README.md) for details

To build the presentation locally:

```bash
npx @marp-team/marp-cli@latest marp/slides.md --theme marp/theme.css -o dist/index.html
```

## 🤝 Contributing

We welcome contributions to make this test repository even more useful! 

Please see our [Contributing Guidelines](CONTRIBUTING.md) for detailed information on:
- How to submit issues and pull requests
- Code style guidelines
- Testing requirements
- Development best practices

## 📝 Best Practices

For development best practices, code style guidelines, and testing standards, please refer to our [Contributing Guidelines](CONTRIBUTING.md).

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🔒 Security

If you discover a security vulnerability, please follow our [Security Policy](SECURITY.md) for responsible disclosure.

## 🙋 Getting Help

If you have questions or need assistance:

- Open an issue in this repository
- Check existing issues for similar questions
- Reach out to the maintainers

## 🌟 Acknowledgments

Thanks to all contributors who help make this testing repository a valuable resource for the GitHub Copilot community!

---

Happy coding with GitHub Copilot! 🚀
