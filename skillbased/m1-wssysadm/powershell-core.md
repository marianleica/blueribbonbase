
### PowerShell Core

PowerShell Core is a cross-platform (Windows, macOS, and Linux) automation and configuration management framework. It is an open-source project built on .NET Core, providing a powerful scripting language and command-line shell for managing and automating tasks.

#### Features

PowerShell Core offers several features that enhance the scripting and automation experience:

- **Cross-Platform**: Runs on Windows, macOS, and Linux, allowing for consistent automation across different operating systems.
- **Open Source**: Developed as an open-source project, enabling community contributions and transparency.
- **Built on .NET Core**: Leverages the performance and capabilities of .NET Core, providing a modern and efficient runtime.
- **Powerful Scripting Language**: Supports advanced scripting capabilities, including functions, loops, and error handling.
- **Extensible**: Allows for the creation of custom cmdlets, modules, and scripts to extend functionality.

#### Installation

To install PowerShell Core, follow these steps:

1. **Windows**:
   - Download the latest PowerShell Core installer from the [GitHub releases page](https://github.com/PowerShell/PowerShell/releases).
   - Run the installer and follow the on-screen instructions.

2. **macOS**:
   - Open Terminal.
   - Install PowerShell Core using Homebrew:
     ```
     brew install --cask powershell
     ```

3. **Linux**:
   - Open Terminal.
   - Follow the installation instructions for your specific Linux distribution from the [PowerShell GitHub repository](https://github.com/PowerShell/PowerShell).

#### Usage

To use PowerShell Core, follow these steps:

1. Open PowerShell Core:
   - On Windows, search for "pwsh" in the Start menu.
   - On macOS and Linux, open Terminal and type `pwsh`.

2. The PowerShell Core prompt will open, allowing you to execute commands and scripts.

#### Examples

Here are some common tasks you can perform using PowerShell Core:

- **List Files in a Directory**: To display a list of files in the current directory, type the following command and press `Enter`:
  ```powershell
  Get-ChildItem
  ```

- **Get System Information**: To display detailed information about the system, type the following command and press `Enter`:
  ```powershell
  Get-ComputerInfo
  ```

- **Create a New File**: To create a new text file, type the following command and press `Enter`:
  ```powershell
  New-Item -Path "example.txt" -ItemType "File"
  ```

#### Additional Information

PowerShell Core is a versatile and powerful tool for automating and managing tasks across different platforms. It provides a consistent scripting environment, making it easier to develop and run scripts on various operating systems. As an open-source project, PowerShell Core continues to evolve with contributions from the community, ensuring it remains a cutting-edge automation framework.
